---
title: JavaScript-code voor [!DNL Analytics for Advertising Cloud]
description: JavaScript-code voor [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 184508ce-df8d-4fa0-b22b-ca0546a61d58
source-git-commit: 56ac178bf10d8c934297521ca3075783e1bc2c36
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# JavaScript-code voor [!DNL Analytics for Advertising Cloud]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Adverteerders met alleen Advertising Cloud DSP*

Voor Advertising Cloud DSP houdt de integratie [!DNL Analytics for Advertising Cloud] de weergave en doorklikinteracties van de site bij. Doorklikbezoeken worden bijgehouden aan de hand van de standaard Adobe Analytics-code op uw webpagina&#39;s. Met de code [!DNL Analytics] worden de parameters AMO ID en EF ID in de URL van de landingspagina vastgelegd en in hun respectievelijke gereserveerde eVars bijgehouden. U kunt doorkijkbezoeken volgen door twee lijnen van code JavaScript in uw webpagina&#39;s op te stellen.

In de eerste paginaweergave van een bezoek aan de site controleert de Advertising Cloud JavaScript-code of de bezoeker een advertentie heeft gezien of erop heeft geklikt. Als de gebruiker eerder via een doorklik de site is binnengekomen of geen advertentie heeft gezien, wordt de bezoeker genegeerd. Als de bezoeker een advertentie heeft gezien en de site niet is binnengekomen via een doorklik tijdens het [click lookback venster](/help/integrations/analytics/prerequisites.md#lookback-a4adc) dat in Advertising Cloud is ingesteld, gebruikt de Advertising Cloud JavaScript-code [Experience Cloud ID Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) om een aanvullende id (`SDID`) te genereren, die wordt gebruikt om gegevens van Advertising Cloud aan de Adobe Analytics-hit van de bezoeker te koppelen. Adobe Analytics vraagt vervolgens Advertising Cloud om de AMO-id en EF-id die aan de advertentie zijn gekoppeld. De AMO-id en EF-id&#39;s worden vervolgens in hun respectieve eVars ingevuld. Deze waarden blijven gedurende een bepaalde periode bestaan (standaard 60 dagen).

[!DNL Analytics] verzendt de metriek van het plaatsverkeer (zoals paginameningen, bezoeken, en bestede tijd) en om het even welke  [!DNL Analytics]  douane of standaardevenementen naar Advertising Cloud per uur, gebruikend EF identiteitskaart als sleutel. Deze [!DNL Analytics] metriek loopt dan door het attributiesysteem van Advertising Cloud om de omzettingen aan de klik en de belichtingsgeschiedenis aan te sluiten.

>[!NOTE]
>
>De JavaScript-traceringslogica van Advertising Cloud vindt plaats aan de Adobe-zijde en heeft dus vrijwel geen invloed op de laadtijd van de pagina.
>
>De logica voor de [!DNL DCM] gegevensconnector naar [!DNL Analytics] (met [!DNL Google Campaign Manager 360]) voor Advertising Cloud DSP daarentegen vindt plaats aan de clientzijde. Door stitching aan de clientzijde wordt de pagina langzamer geladen en neemt het risico op gegevensverlies toe. Dit komt voor omdat [!DNL Analytics] JavaScript [!DNL DoubleClick] moet pingelen en op [!DNL DoubleClick] moet wachten om de laatste klik/de impeilingsgegevens aan [!DNL Analytics] terug te geven. Wanneer uw [!DNL DSP] team de [!DNL DCM] gegevensschakelaar opstelt, moet u specificeren hoe lang u bereid bent om de pagina te vertragen.

## JavaScript-code implementeren

De JavaScript-bibliotheek bestaat uit twee regels waarmee [!DNL Analytics] en Advertising Cloud met elkaar kunnen communiceren. Als de [!DNL Analytics for Advertising Cloud] integratie tijdens de implementatie van Advertising Cloud werd voltooid, dan zou u deze code met instructies op moeten ontvangen hoe te om het op te stellen.

Als u nog geen code hebt, neemt u contact op met het Advertising Cloud-ondersteuningsteam.

### Plaats de code

De JavaScript-functie [!DNL Analytics for Advertising Cloud] moet na de Experience Cloud ID-service komen, maar voordat de code voor meting van de Analytics App wordt uitgevoerd, zodat de aanvullende id (`SDID`) kan worden opgenomen in de oproep Analytics.

![Codeplaatsing](/help/integrations/assets/a4adc-code-placement.png)

### Implementatie van code valideren

U kunt validatie uitvoeren met elk pakketsniffertype (zoals [!DNL Charles], [!DNL Fiddler] of [!DNL Chrome Developer Tools]) door de waarden van de vier id&#39;s te vergelijken tussen de aanvraag die naar Advertising Cloud gaat en de aanvraag die naar [!DNL Analytics] gaat, zoals hieronder wordt beschreven.

#### Hoe te om de Code met [!DNL Chrome Developer Tools] te bevestigen {#validate-js-chrome}

1. Open [!DNL Chrome Developer Tools] en klik **Netwerk** tabel.
1. Laad een websitepagina die de JavaScript [!DNL Analytics for Advertising Cloud] bevat.
1. Filter de tab [!UICONTROL Network] met `last` en bekijk twee rijen:

   ![Filteren op laatste](/help/integrations/assets/a4adc-code-validation-filter-last.png)

   * De eerste rij is de aanroep naar de JavaScript-bibliotheek en krijgt de naam `last-event-tag-latest.min.js`.
   * De tweede rij is de vraag die het verzoek naar Advertising Cloud verzendt. Het begint als volgt: `_les_imsOrgId=[your_imsOrgId_here]&_les_url=[your_encoded_url]`

      Als u de oproep aan Advertising Cloud niet ziet, is het mogelijk niet de eerste paginaweergave van uw bezoek. Voor testdoeleinden kunt u de cookie verwijderen zodat de volgende aanroep de eerste paginaweergave voor het bijbehorende bezoek wordt:

      1. Zoek op het tabblad Toepassing naar het cookie `adcloud` en controleer of het cookie `_les_v` (laatste bezoek) bevat met de waarde `y` en een tijdstempel voor UTC-tijdperk die in 30 minuten vervalt.
      1. Verwijder het cookie `ad cloud` en vernieuw de pagina.
1. Filter op `/b/ss` om de treffer voor Analytics te zien.

   ![Filteren op  `/b/ss`](/help/integrations/assets/a4adc-code-validation-filter-bss.png)

1. Vergelijk de id-waarden tussen de twee treffers. Alle waarden zullen in de parameters van het vraagkoord behalve rapportreeks identiteitskaart in de Bevolking van Analytics zijn, die de weg URL onmiddellijk na `/b/ss/` is.

   | ID | Parameter Analytics | Advertising Cloud-parameter |
   |--- |--- |--- |
   | Experience Cloud IMS Org | `mcorgid` | `_les_imsOrgid` |
   | Aanvullende gegevens-id | sdid | `_les_sdid` |
   | Analyserapportsuite | De waarde na `/b/ss/` | `_les_rsid` |
   | Experience Cloud-bezoeker-id | midden | `_les_mid` |

   Als de id-waarden overeenkomen, wordt de JavaScript-implementatie bevestigd. Advertising Cloud stuurt de [!DNL Analytics]-server alle eventuele doorklikgegevens of doorkijkgegevens.

#### Hoe te om de Code met [!DNL Adobe Experience Cloud Debugger] te bevestigen

1. Open [[!DNL Adobe Experience Cloud Debugger]](https://experienceleague.adobe.com/docs/debugger/using/run-debugger.html) op uw homepage.
1. Ga naar het tabblad [!UICONTROL Network].
1. Klik op [!UICONTROL Solutions Filter] op de werkbalk [!UICONTROL Advertising Cloud] en [!UICONTROL Analytics].
1. Zoek in de parameterrij [!UICONTROL Request URL – Hostname] `lasteventf-tm.everesttech.net`.
1. In [!UICONTROL Request – Parameters*] rij, controle de gegenereerde signalen, gelijkend op Stap 3 in &quot;[hoe te om de Code met [!DNL Chrome Developer Tools]](#validate-js-chrome) te bevestigen.&quot;
   * Controleer of de parameter `SDID` overeenkomt met `Supplemental Data ID` in het Adobe Analytics-filter.
   * Als de code niet genereert, controleert u of het Advertising Cloud-cookie is verwijderd op het tabblad [!UICONTROL Application]. Nadat de pagina is verwijderd, vernieuwt u de pagina en herhaalt u het proces.

   ![JavaScript- [!DNL Analytics for Advertising Cloud] code controleren in  [!DNL Experience Cloud Debugger]](/help/integrations/assets/a4adc-js-audit-debugger.png)

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]](prerequisites.md)

