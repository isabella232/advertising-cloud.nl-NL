---
title: JavaScript-code voor [!DNL Analytics for Advertising Cloud]
description: JavaScript-code voor [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 184508ce-df8d-4fa0-b22b-ca0546a61d58
source-git-commit: 594854f27d6a451167c90116b640781bbea11b63
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# JavaScript-code voor [!DNL Analytics for Advertising Cloud]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Adverteerders met alleen Advertising Cloud DSP*

Voor Advertising Cloud DSP: [!DNL Analytics for Advertising Cloud] de integratie houdt mening-door en klik-door plaatsinteractie. Doorklikbezoeken worden bijgehouden aan de hand van de standaard Adobe Analytics-code op uw webpagina&#39;s. de [!DNL Analytics] De parameters AMO ID en EF ID worden in de URL van de bestemmingspagina vastgelegd en in hun respectieve gereserveerde eVars bijgehouden. U kunt doorkijkbezoeken volgen door twee lijnen van code JavaScript in uw webpagina&#39;s op te stellen.

In de eerste paginaweergave van een bezoek aan de site controleert de Advertising Cloud JavaScript-code of de bezoeker een advertentie heeft gezien of erop heeft geklikt. Als de gebruiker eerder via een doorklik de site is binnengekomen of geen advertentie heeft gezien, wordt de bezoeker genegeerd. Als de bezoeker een advertentie heeft gezien en de site niet via een doorklikverbinding heeft betreden tijdens het [klik terugkijkvenster](/help/integrations/analytics/prerequisites.md#lookback-a4adc) ingesteld in Advertising Cloud, gebruikt de Advertising Cloud JavaScript-code a) de [Experience Cloud ID-service](https://experienceleague.adobe.com/docs/id-service/using/home.html) om een aanvullende id te genereren (`SDID`) of b) gebruikt de Adobe Experience Platform [!DNL Web SDK] om een `[!DNL StitchID]`. Een van beide id&#39;s wordt gebruikt om gegevens van Advertising Cloud aan te sluiten op de hit Adobe Analytics van de bezoeker. Adobe Analytics vraagt vervolgens Advertising Cloud om de AMO-id en EF-id die aan de advertentie zijn gekoppeld. De AMO-id en EF-id&#39;s worden vervolgens in hun respectieve eVars ingevuld. Deze waarden blijven gedurende een bepaalde periode bestaan (standaard 60 dagen).

[!DNL Analytics] verzendt de metriek van het plaatsverkeer (zoals paginameningen, bezoeken, en bestede tijd) en om het even welk [!DNL Analytics] aangepaste of standaardgebeurtenissen naar Advertising Cloud-uur, waarbij de EF-id als sleutel wordt gebruikt. Deze [!DNL Analytics] De metriek loopt dan door het attributiesysteem van Advertising Cloud om de omzettingen aan de klik en de blootstellingsgeschiedenis aan te sluiten.

>[!NOTE]
>
>De JavaScript-traceringslogica van Advertising Cloud vindt plaats aan de Adobe-zijde en heeft dus vrijwel geen invloed op de laadtijd van de pagina.
>
>De logica voor de [!DNL DCM] gegevensaansluiting naar [!DNL Analytics] (gebruiken [!DNL Google Campaign Manager 360]) voor Advertising Cloud DSP wordt op de client uitgevoerd. Door stitching aan de clientzijde wordt de pagina langzamer geladen en neemt het risico op gegevensverlies toe. Dit gebeurt omdat de [!DNL Analytics] JavaScript moet pingelen [!DNL DoubleClick] en wachten op [!DNL DoubleClick] om de laatste klik-/afbeeldingsgegevens door te geven aan [!DNL Analytics]. Wanneer uw [!DNL DSP] team stelt [!DNL DCM] gegevensconnector, moet u opgeven hoe lang u de pagina wilt vertragen.

## JavaScript-code implementeren

De JavaScript-bibliotheek bestaat uit twee regels die [!DNL Analytics] en Advertising Cloud om met elkaar te communiceren. Als de [!DNL Analytics for Advertising Cloud] de integratie is voltooid tijdens de Advertising Cloud-implementatie, dan had u deze code moeten ontvangen met instructies voor het implementeren ervan.

Als u nog geen code hebt, neemt u contact op met het Advertising Cloud-ondersteuningsteam.

### Plaats de code

De [!DNL Analytics for Advertising Cloud] De JavaScript-functie moet na de Experience Cloud-id-service komen, maar voordat de code voor metingen van de Analytics App wordt uitgevoerd, zodat de aanvullende id (`SDID`) of `[!DNL StitchID]` kan in uw vraag van Analytics worden omvat.

![Codeplaatsing](/help/integrations/assets/a4adc-code-placement.png)

### Implementatie van code valideren

U kunt validatie uitvoeren met elk pakketsniffertype (zoals [!DNL Charles], [!DNL Fiddler], of [!DNL Chrome Developer Tools]) door de waarden van de vier id&#39;s te vergelijken tussen de aanvraag die naar Advertising Cloud gaat en de aanvraag die naar [!DNL Analytics], zoals hieronder beschreven.

#### De code bevestigen met [!DNL Chrome Developer Tools] {#validate-js-chrome}

1. Openen [!DNL Chrome Developer Tools] en klik op de knop **Netwerk** tab.
1. Een websitepagina laden die de [!DNL Analytics for Advertising Cloud] JavaScript.
1. Filter de [!UICONTROL Network] tab by `last` en bekijk twee rijen:

   ![Filteren op laatste](/help/integrations/assets/a4adc-code-validation-filter-last.png)

   * De eerste rij is de aanroep naar de JavaScript-bibliotheek en krijgt de naam `last-event-tag-latest.min.js`.
   * De tweede rij is de vraag die het verzoek naar Advertising Cloud verzendt. Het begint als volgt: `_les_imsOrgId=[your_imsOrgId_here]&_les_url=[your_encoded_url]`

      Als u de oproep aan Advertising Cloud niet ziet, is het mogelijk niet de eerste paginaweergave van uw bezoek. Voor testdoeleinden kunt u de cookie verwijderen zodat de volgende aanroep de eerste paginaweergave voor het bijbehorende bezoek wordt:

      1. Zoek op het tabblad Toepassing naar het tabblad `adcloud` cookie, en controleer of de cookie `_les_v` (laatste bezoek) met een waarde van `y` en een tijdstempel voor UTC-tijdperk die over 30 minuten verloopt.
      1. Verwijder de `ad cloud` cookie maken en de pagina vernieuwen.
1. Filter op `/b/ss` om de Analytics-hit te zien.

   ![Filteren op `/b/ss`](/help/integrations/assets/a4adc-code-validation-filter-bss.png)

1. Vergelijk de id-waarden tussen de twee treffers. Alle waarden worden opgenomen in parameters van queryreeksen, behalve de id van de rapportsuite in de hit Analytics. Dit is het URL-pad dat onmiddellijk volgt `/b/ss/`.

   | ID | Parameter Analytics | Advertising Cloud-parameter |
   |--- |--- |--- |
   | Experience Cloud IMS Org | `mcorgid` | `_les_imsOrgid` |
   | Aanvullende gegevens-id | sdid | `_les_sdid` |
   | Analyserapportsuite | De waarde na `/b/ss/` | `_les_rsid` |
   | Experience Cloud-bezoeker-id | midden | `_les_mid` |

   Als de id-waarden overeenkomen, wordt de JavaScript-implementatie bevestigd. Advertising Cloud stuurt de [!DNL Analytics] eventuele doorklikgegevens of doorlopende trackinggegevens op de server te plaatsen.

#### De code bevestigen met [!DNL Adobe Experience Cloud Debugger]

1. Open de [[!DNL Adobe Experience Cloud Debugger]](https://experienceleague.adobe.com/docs/debugger/using/run-debugger.html) op je homepage.
1. Ga naar de [!UICONTROL Network] tab.
1. In de [!UICONTROL Solutions Filter] werkbalk, klikt u op [!UICONTROL Advertising Cloud] en [!UICONTROL Analytics].
1. In de [!UICONTROL Request URL – Hostname] parameterrij, zoeken `lasteventf-tm.everesttech.net`.
1. In de [!UICONTROL Request – Parameters] rij, controleer de geproduceerde signalen, gelijkend op Stap 3 in &quot;[De code bevestigen met [!DNL Chrome Developer Tools]](#validate-js-chrome).&quot;
   * Controleer of de `SDID` parameter komt overeen met `Supplemental Data ID` in het Adobe Analytics-filter.
   * Als de code niet wordt gegenereerd, controleert u of de Advertising Cloud-cookie is verwijderd in het dialoogvenster [!UICONTROL Application] tab. Nadat de pagina is verwijderd, vernieuwt u de pagina en herhaalt u het proces.

   ![Controle [!DNL Analytics for Advertising Cloud] JavaScript-code in [!DNL Experience Cloud Debugger]](/help/integrations/assets/a4adc-js-audit-debugger.png)

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]](prerequisites.md)

