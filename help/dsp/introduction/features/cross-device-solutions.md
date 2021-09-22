---
title: Apparaatoplossingen
description: Meer informatie over functies voor verschillende apparaten.
feature: DSP Introduction
exl-id: 29f8ec41-35a6-4a29-a638-82a2929a8fe6
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# Apparaatoplossingen

Dankzij de Advertising Cloud DSP-integratie met [!DNL LiveRamp] en [!DNL Adobe Device Co-op] kunt u uw publiek uitbreiden naar alle bekende apparaten van een persoon, en niet alleen naar de apparaten die uw merk heeft bijgehouden. De integraties bieden ook frequentietoewijzing en attributiemeting op alle apparaten.

Wanneer u een ondersteunde apparaatgrafiek gebruikt, kunt u:

* Stem het publiek af via kanalen en apparaten om advertenties te leveren aan mensen en huishoudens in plaats van aan apparaten.
* Balans en blootstelling door inzicht te krijgen in de frequentie van de begrenzing van personen.
* Teststrategieën die publiek toegankelijk maken ten opzichte van publiek converteren naar kanalen of apparaten.

## Voordelen van elke apparaatgrafiek

* [!DNL Adobe Device Co-op]:
   * Biedt een opt-in-pool van deterministische en probabilistische gegevens van deelnemende Adobe-adverteerders
   * Biedt sterke cookie-id-verbindingen, aangedreven door desktopbezoekers en mobiele webbezoekers
   * Omvat gegevens voornamelijk uit de Verenigde Staten en Canada
   * Heeft geen gebruikskosten

* [!DNL LiveRamp] apparaatgrafiek:
   * Verstrekt een deterministische gegevenspool, met inbegrip van off-line klantengegevens
   * Biedt een gelijkmatige dekking tussen cookie-id&#39;s en mobiele apparaat-id&#39;s
   * Inclusief gegevens voornamelijk uit de Verenigde Staten
   * Is gratis voor frequentiecalfakanalen en attribuutmetingen
   * Geprijsd bij $0.35 CPM voor uitgebreide beelden (indrukkingen die uitsluitend door de [!DNL LiveRamp] apparatengrafiek te gebruiken eerder dan op apparaten worden geleverd die binnen de gerichte publiekssegmenten worden gevonden)

      De snelheid wordt weergegeven op je creditcard met accounttarieven.

## Personeelsgebaseerd frequentiebeheer

Met op personen gebaseerd frequentiebeheer kunt u frequentiecappen op persoonlijk niveau in plaats van op apparaatniveau opgeven voor een werkelijke controle van de mediablootstelling.

### Frequentiebeheer op basis van personen activeren

* **Campagnes:** Wanneer u een nieuwe campagne maakt, kunt u een  [!UICONTROL Cross-Device Level] instelling opgeven. Schakel &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People]&quot; in en selecteer een apparaatgrafiek. De gespecificeerde apparatengrafiek wordt gebruikt voor zowel dwars-apparaat richtend op het plaatsingsniveau als voor op mensen-gebaseerd frequentiebeheer op de campagne, het pakket, en plaatsingsniveau. De frequentiecaps zijn van toepassing op alle bekende apparaten van een persoon.

Zie [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md) voor meer informatie.

Wanneer u een campagne hebt opgeslagen, kunt u de instelling [!UICONTROL Cross Device Level] niet meer wijzigen.

* **Pakketten:**  U kunt desgewenst extra frequentiecappen op pakketniveau plaatsen. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

* **Plaatsen:** U kunt desgewenst extra frequentiecappen instellen op plaatsingsniveau. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

## Personeelsgericht

Door op mensen gebaseerde doelgroepen te kiezen, kunt u klanten zoeken op verschillende desktops en mobiele apparaten.

### Activeren op basis van personen

* **Campagnes:** Wanneer u een nieuwe campagne maakt, kunt u een  [!UICONTROL Cross-Device Level] instelling opgeven. Schakel &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People]&quot; in en selecteer een apparaatgrafiek. De gespecificeerde apparatengrafiek wordt gebruikt voor zowel dwars-apparaat richtend op het plaatsingsniveau als voor op mensen-gebaseerd frequentiebeheer.

Zie [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md) voor meer informatie.

* **Plaatsen:** Wanneer u publieksdoelstellingen voor een plaatsing in een campagne met een gespecificeerde apparatengrafiek selecteert, staat een  [!UICONTROL Cross-Device Targeting] optie u toe om uw het richten over alle bekende apparaten van een persoon (per de apparatengrafiek uit te breiden die in de campagnemontages wordt gespecificeerd), zelfs apparaten die niet in de gespecificeerde segmenten zijn.

### Rapportage instellen voor op mensen gebaseerde doelen

U kunt de volgende metriek in douanerapporten omvatten:

* **Uitgebreide indrukkingen:** (In de  [!UICONTROL Build Your Report] sectie onder  [!UICONTROL Metrics] >  [!UICONTROL Std. Metrics]) Het volume van incrementele indrukkingen die worden geleverd door een apparaatgrafiek te gebruiken (en die niet worden gevonden binnen de oorspronkelijke publiekssegmenten). Deze maatstaf wordt ook gebruikt voor de berekening van de toepasselijke vergoedingen voor het gebruik van een apparaatgrafiek van derden.

   Om de kosten van uw uitgebreide indrukkingen tijdens een tijdspanne te bepalen, stel een douanerapport in dat [!UICONTROL Extended Impressions] kolom omvat, en vermenigvuldig dan het totale aantal uitgebreide indrukkingen met $0.0035 ($0.35/1000 beelden).

   De geaggregeerde kosten worden ook opgenomen in de kolom [!UICONTROL Billable Other Net Spend] (onder [!UICONTROL Metrics] > [!UICONTROL Spend]), hoewel die metrische waarde ook andere campagnekosten omvat die u mogelijk hebt toegevoegd.

* **Apparaatgrafiek:** (in de  [!UICONTROL Build Your Report] sectie onder  [!UICONTROL Dimensions] >  [!UICONTROL Campaign]) De geselecteerde apparaatgrafiek voor een bepaalde campagne, een bepaald pakket of een bepaalde plaatsing.

## Meting van op personen gebaseerde kenmerk

*Adverteerders met alleen Advertising Cloud Conversion Tracking*

Met op mensen gebaseerde attributie, kunt u omzettingen verklaren die op een verschillend apparaat dan het apparaat plaatsvonden waarop de media blootstelling voorkwam. Over DSP, Advertising Cloud Search en Advertising Cloud Creative is een maatstaf voor individuele toewijzingen beschikbaar voor adverteerders die Advertising Cloud-conversiepixels op hun sites hebben geïmplementeerd.

### Meting van op personen gebaseerde kenmerken inschakelen

Neem contact op met de accountmanager van de Adobe als u maten voor apparaattoewijzing wilt activeren. Voor [!DNL Adobe Device Co-op] accounts, zult u uw ondertekende [!DNL Adobe Device Co-op] contract en Experience Cloud [!DNL Organization ID] (vroeger genoemd [!DNL IMS org ID]) moeten verstrekken.

Om te zien of wordt een adverteerderaccount gevormd om een apparatengrafiek voor attributitemeting te gebruiken:

1. Klik in het hoofdmenu op **[!UICONTROL Settings]>[!UICONTROL Advertiser]**.
1. Plaats de cursor op de rij van de adverteerder en klik **[!UICONTROL Edit]**.
1. Controleer in de sectie [!UICONTROL Integrations] van de advertentiemontages of de [!UICONTROL Cross-Device Attribution]-instelling actief is.

   Voor actieve integratie wordt de apparaatgrafiek aangegeven.

### Conversierapporten instellen voor kenmerk voor apparaatconversie

#### Instellingen omzettingsrapport

Wanneer een apparatengrafiek voor attributitemeting wordt toegelaten, omvat [!UICONTROL Conversion] het Rapport [!UICONTROL Cross-Device Breakout] het plaatsen, die u toestaat om maximaal drie afzonderlijke kolommen voor elke omzettingsmetrisch te omvatten:

* &lt;>Conversie *>[!UICONTROL (tp)]: Omvat de totale omzettingen (totaal aantal personen), die zowel de omzettingen van hetzelfde apparaat als de omzettingen van het apparaat (indien van toepassing) omvatten.* In het rapport wordt &quot;[!UICONTROL (tp)]&quot;toegevoegd aan de metrische naam van de omzetting, regeltype, en omzettingstypes in de omzettingsweg (bijvoorbeeld, &quot;Reacties (le)(tl)(tp)).

* &lt;>Conversie *>[!UICONTROL (sd)]: (Optioneel) Omvat alleen omzettingen waarvoor in het conversiepad slechts één apparaat is bijgehouden.* In het rapport wordt &quot;[!UICONTROL (sd)]&quot;toegevoegd aan de metrische naam van de omzetting, regeltype, en omzettingstypes in de omzettingsweg (bijvoorbeeld, &quot;Reacties (le)(tl)(sd))).

* &lt;>Conversie *>[!UICONTROL (xd)]: (Optioneel) Omvat alleen omzettingen waarvoor meer dan één apparaat is bijgehouden in het conversiepad.* In het rapport wordt &quot;[!UICONTROL (xd)]&quot;toegevoegd aan de metrische naam van de omzetting, regeltype, en omzettingstypes in de omzettingsweg (bijvoorbeeld, &quot;Reacties (le)(tl)(xd)).

#### Hoe te om het Rapport van de Omzetting te interpreteren

Als u het percentage van totale omzettingen sorteert die dwars-apparaat ([!UICONTROL (xd)]/[!UICONTROL (tl)]) van hoog aan laag zijn, zult u begrijpen wat boven-gemiddelde dwars-apparatenomzettingen drijft. U kunt dit gebruiken om uw creatieve of het richten strategie te informeren om overseinen en kanaalinvestering aan gebruikersgedrag aan te passen.

* Pakketten - Zie welke pakketten de meeste totale omzettingen drijven, en welke degenen een hoog percentage van dwars-apparatenomzettingen hebben. Dit kan u helpen begrijpen waar te om uitgaven te concentreren.

* Plaatsen - Vergelijk plaatsingsprestaties en attributie (bijvoorbeeld, een mobiele Web en kan omzettingen op Desktop drijven). Zonder apparaatgrafiek voor attributie kunt u de invloed van een mobiele webplaatsing op desktopconversies missen. Het is ook mogelijk dat deze wordt begraven als de meeste gebruikers de conversie op het bureaublad en niet op het mobiele web uitvoeren.

* Advertenties - Ontdek welke advertenties tot hogere omzettingen leiden, en kwantificeer hun waarde en effect in zowel webbrowsers als mobiele toepassingsomgevingen.

* Sites - Optimaliseren voor alle sites in plaats van sites handmatig uit te sluiten. Als een website conversies tussen apparaten aandrijft, dan kunt u zien op welke apparaten dit gedrag voorkomt.

* Deals - Verbeter handmatige optimalisering door te controleren welke inventarisovereenkomsten de omzettingen van verschillende apparaten leveren, en dan te beslissen of u uw richten zou moeten uitbreiden om meer apparaten en kanalen in die overeenkomsten te omvatten.

>[!MORELIKETHIS]
>
>* [Rapportinstellingen](/help/dsp/reports/report-settings.md)
>* [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

