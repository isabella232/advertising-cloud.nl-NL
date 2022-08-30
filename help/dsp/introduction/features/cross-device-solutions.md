---
title: Apparaatoplossingen
description: Meer informatie over functies voor verschillende apparaten.
feature: DSP Introduction
exl-id: 29f8ec41-35a6-4a29-a638-82a2929a8fe6
source-git-commit: d7afcc2200adc41e583d21712226cb25f35aab66
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Apparaatoplossingen

De integratie van Advertising Cloud DSP met [!DNL LiveRamp] Hiermee kunt u uw publiek uitbreiden naar alle bekende apparaten van een persoon, en niet alleen naar de apparaten die uw merk heeft bijgehouden. De integratie biedt ook frequentiecapping en attributie-meting voor alle apparaten.

Wanneer u een ondersteunde apparaatgrafiek gebruikt, kunt u:

* Stem het publiek af via kanalen en apparaten om advertenties te leveren aan mensen en huishoudens in plaats van aan apparaten.
* Balans en blootstelling door inzicht te krijgen in de frequentie van de begrenzing van personen.
* Teststrategieën die publiek toegankelijk maken ten opzichte van publiek converteren naar kanalen of apparaten.

## De voordelen van de [!DNL LiveRamp] Apparaatgrafiek

* Verstrekt een deterministische gegevenspool, met inbegrip van off-line klantengegevens

* Biedt een gelijkmatige dekking tussen cookie-id&#39;s en mobiele apparaat-id&#39;s

* Inclusief gegevens voornamelijk uit de Verenigde Staten

* Is gratis voor frequentiecalfakanalen en attribuutmetingen

* Geprijseerd bij $0.35 CPM voor uitgebreide beelden (indrukkingen die uitsluitend door het gebruiken van worden geleverd [!DNL LiveRamp] apparaatgrafiek in plaats van op apparaten die worden gevonden binnen de doelpubliekssegmenten)

   De snelheid wordt weergegeven op je creditcard met accounttarieven.

## Personeelsgebaseerd frequentiebeheer

Met op personen gebaseerd frequentiebeheer kunt u frequentiecappen op persoonlijk niveau in plaats van op apparaatniveau opgeven voor een werkelijke controle van de mediablootstelling.

### Frequentiebeheer op basis van personen activeren

* **Campagnes:** Wanneer u een nieuwe campagne maakt, kunt u een [!UICONTROL Cross-Device Level] instellen. &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People],&quot; en selecteert u een apparaatgrafiek. De gespecificeerde apparatengrafiek wordt gebruikt voor zowel dwars-apparaat richtend op het plaatsingsniveau als voor op mensen-gebaseerd frequentiebeheer op de campagne, het pakket, en plaatsingsniveau. De frequentiecaps zijn van toepassing op alle bekende apparaten van een persoon.

Zie voor meer informatie [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md).

Als u een campagne eenmaal hebt opgeslagen, kunt u de campagne niet meer wijzigen [!UICONTROL Cross Device Level] instellen.

* **Pakketten:**  U kunt desgewenst extra frequentiecappen op pakketniveau instellen. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

* **Plaatsen:** U kunt desgewenst extra frequentiecappen instellen op plaatsingsniveau. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

## Personeelsgericht

Door op mensen gebaseerde doelgroepen te kiezen, kunt u klanten zoeken op verschillende desktops en mobiele apparaten.

### Activeren op basis van personen

* **Campagnes:** Wanneer u een nieuwe campagne maakt, kunt u een [!UICONTROL Cross-Device Level] instellen. &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People],&quot; en selecteert u een apparaatgrafiek. De gespecificeerde apparatengrafiek wordt gebruikt voor zowel dwars-apparaat richtend op het plaatsingsniveau als voor op mensen-gebaseerd frequentiebeheer.

Zie voor meer informatie [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md).

* **Plaatsen:** Wanneer u doelpubliek selecteert voor een plaatsing in een campagne met een opgegeven apparaatgrafiek, kunt u een [!UICONTROL Cross-Device Targeting] Met deze optie kunt u uw doelversie uitbreiden naar alle bekende apparaten van een persoon (volgens de apparaatgrafiek die is opgegeven in de campagnemontages), zelfs naar apparaten die zich niet in de opgegeven segmenten bevinden.

### Rapportage instellen voor op mensen gebaseerde doelen

U kunt de volgende metriek in douanerapporten omvatten:

* **Uitgebreide afbeeldingen:** (In de [!UICONTROL Build Your Report] deel onder [!UICONTROL Metrics] > [!UICONTROL Std. Metrics]) Het volume van incrementele indrukkingen dat wordt geleverd door een apparaatgrafiek te gebruiken (en dat niet wordt gevonden in de oorspronkelijke publiekssegmenten). Deze maatstaf wordt ook gebruikt voor de berekening van de toepasselijke vergoedingen voor het gebruik van een apparaatgrafiek van derden.

   Om de kosten van uw uitgebreide beelden tijdens een tijdspanne te bepalen, stel een douanerapport in werking dat omvat [!UICONTROL Extended Impressions] en vermenigvuldigt u vervolgens het totale aantal uitgebreide afdrukken met $0,00035 ($0,35/1000 afbeeldingen).

   De geaggregeerde kosten worden ook opgenomen in de [!UICONTROL Billable Other Net Spend] kolom (onder [!UICONTROL Metrics] > [!UICONTROL Spend]), hoewel die maatstaf ook andere campagnekosten omvat die u wellicht hebt toegevoegd.

* **Apparaatgrafiek:** (In de [!UICONTROL Build Your Report] deel onder [!UICONTROL Dimensions] > [!UICONTROL Campaign]) De geselecteerde apparaatgrafiek voor een bepaalde campagne, een bepaald pakket of een bepaalde plaatsing.

## Meting van op personen gebaseerde kenmerk

*Adverteerders met alleen Advertising Cloud Conversion Tracking*

Met op mensen gebaseerde attributie, kunt u omzettingen verklaren die op een verschillend apparaat dan het apparaat plaatsvonden waarop de media blootstelling voorkwam. Over DSP, Advertising Cloud Search en Advertising Cloud Creative is een maatstaf voor individuele toewijzingen beschikbaar voor adverteerders die Advertising Cloud-conversiepixels op hun sites hebben geïmplementeerd.

### Meting van op personen gebaseerde kenmerken inschakelen

Neem contact op met uw [!DNL Adobe] accountteam.

### Conversierapporten instellen voor kenmerk voor apparaatconversie

#### Instellingen omzettingsrapport

Wanneer een apparaatgrafiek is ingeschakeld voor attributiemeting, wordt [!UICONTROL Conversion] Rapport bevat een [!UICONTROL Cross-Device Breakout] het plaatsen, dat u toestaat om maximaal drie afzonderlijke kolommen voor elke omzettingsmetrisch te omvatten, die omvatten:

* &lt;*Conversie*>[!UICONTROL (tp)]: Omvat de totale omzettingen (totaal aantal personen), die zowel de omzettingen van hetzelfde apparaat als de omzettingen van het apparaat (indien van toepassing) omvatten. In het verslag[!UICONTROL (tp)]&quot; wordt toegevoegd aan de metrische naam, het regeltype en de omzettingstypen in het conversiepad (bijvoorbeeld &quot;Reacties(le)(tl)(tp)).

* &lt;*Conversie*>[!UICONTROL (sd)]: (Optioneel) Omvat alleen omzettingen waarvoor in het conversiepad slechts één apparaat is bijgehouden. In het verslag[!UICONTROL (sd)]&quot; wordt toegevoegd aan de metrische naam, het regeltype en de omzettingstypen in het conversiepad (bijvoorbeeld &quot;Reacties(le)(tl)(sd)).

* &lt;*Conversie*>[!UICONTROL (xd)]: (Optioneel) Omvat alleen omzettingen waarvoor meer dan één apparaat is bijgehouden in het conversiepad. In het verslag[!UICONTROL (xd)]&quot; wordt toegevoegd aan de metrische naam, het regeltype en de omzettingstypen in het conversiepad (bijvoorbeeld &quot;Reacties(le)(tl)(xd)).

#### Hoe te om het Rapport van de Omzetting te interpreteren

Als u het percentage van totale omzettingen sorteert die dwars-apparaat zijn ([!UICONTROL (xd)]/[!UICONTROL (tl)]) van hoog naar laag, zult u begrijpen wat drijft boven-gemiddelde dwars-apparatenomzettingen. U kunt dit gebruiken om uw creatieve of het richten strategie te informeren om overseinen en kanaalinvestering aan gebruikersgedrag aan te passen.

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

