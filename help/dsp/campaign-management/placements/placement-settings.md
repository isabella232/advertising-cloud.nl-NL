---
title: Plaatsingsinstellingen
description: Zie beschrijvingen van de beschikbare plaatsingsmontages.
feature: DSP Placements
exl-id: 36097132-e589-4d49-bf86-54f61eae5b67
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '3418'
ht-degree: 0%

---

# Plaatsingsinstellingen

## [!UICONTROL Basics]

**[!UICONTROL Placement name]** De plaatsingsnaam.

>[!TIP]
>Gebruik een naamgevingsconventie die voor uw situatie zinnig is. Eén voorgestelde naamgevingsconventie is &quot;*\&lt;campaign name=&quot;&quot;>: \&lt;ad unit=&quot;&quot;>: \&lt;duration>: \&lt;targeting>*.&quot;

**[!UICONTROL Status]:** De plaatsingsstatus: *[!UICONTROL Active]* (de standaardwaarde) of *[!UICONTROL Paused]*.

>[!TIP]
>De beste manier is om de plaatsing te pauzeren tot u bereid bent om het te lanceren.

**[!UICONTROL Details]:** (Alleen-lezen) Het toepasselijke advertentietype, de account die de plaatsing maakt of heeft gemaakt, en de bovenliggende campagne. Klik op **[!UICONTROL Show more]**.

**[!UICONTROL Templates]:** Hiermee opent u een lijst met bestaande plaatsingssjablonen. Als u doelinstellingen automatisch wilt invullen vanuit een sjabloon:

1. Voer een van de volgende handelingen uit:

   * Als u al het doel uit een sjabloon opnieuw wilt gebruiken, schakelt u het selectievakje naast de sjabloonnaam in.

   * Als u afzonderlijke doeltypen uit een sjabloon opnieuw wilt gebruiken, vouwt u de sjabloonnaam uit en schakelt u het selectievakje in naast de doeltypen die u opnieuw wilt gebruiken.

1. Klik op **[!UICONTROL Apply]**.

**[!UICONTROL Ad specs for forecast]:** (Alleen video en indelingen) De duur en/of specificaties van de advertentie, die worden gebruikt om de voorspelde projectie aan de rechterkant te berekenen. De velden verschillen per advertentietype.

**[!UICONTROL Environment]:** (Alleen Universal Video ad-indeling) De apparaatomgevingen (Computer, Mobiel, Connected TV) die als doelen in de plaatsing moeten worden opgenomen.

**[!UICONTROL Placement tags]:** (Optioneel) Trefwoorden of bijnamen om u te helpen deze plaatsing te vinden.

## Doelen

**[!UICONTROL Package]:** (Optioneel) Een pakket waaraan de plaatsing is toegewezen. Klikken ![Bewerken](/help/dsp/assets/edit.png) om een bestaand pakket te selecteren of te maken. Wanneer u de plaatsing aan een pakket toewijst, [!UICONTROL Goals] wordt bijgewerkt met de vluchtdata, de leveringsdoelstelling en het budget uit het pakket.

**[!UICONTROL Flight Dates]:** De begindatum en einddatum voor de plaatsing. Goedgekeurde advertenties komen in aanmerking om tijdens de vlucht te worden uitgevoerd wanneer de plaatsing actief is en wordt toegewezen aan een actief pakket of een actieve campagne.

De datums voor het pakket (indien van toepassing) of de campagne worden standaard automatisch ingevuld.

>[!NOTE]
>
>* De vluchtdata moeten worden opgenomen in de campagnevluchtdata en de pakketvliegdata.


### Plaatsen die aan Pakketten met pakket-vlakke Tussenruimte worden toegewezen

**[!UICONTROL Placement Funding]:** Hoe te om voor de plaatsing te begroten:

* *[!UICONTROL Optimize based on performance]:* Beheert de begroting op pakketniveau.
* *[!UICONTROL Set a fixed budget cap]:* Hiermee kunt u een budget voor dagelijkse, wekelijkse, maandelijkse of volledige plaatsing instellen. Voer een waarde en de duur in (*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Max Bid]:** Het maximum dat voor 1000 beelden moet worden betaald.

**[!UICONTROL Placement Pre-bid Filters]:** Maximaal vijf KPI-drempels (zoals een minimale weergavemetrisch of doorkliksnelheid) die moeten worden gehaald om te kunnen bieden. U kunt voorbiedingsfilters gebruiken als optimalisatietactiek, maar u weet dat elke regel de mogelijkheden waarop deze plaatsing kan bieden, kan beperken. Filters toevoegen of bewerken:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een filter toevoegen:
      1. Klik op **[!UICONTROL Add Filter]**.
      1. Volgende tot **[!UICONTROL Only bid if]** selecteert u een metrische waarde en voert u een waarde in.
   * Als u een filter wilt verwijderen, klikt u op **[!UICONTROL X]** in de filterrij.
1. Klik op **[!UICONTROL Save]**.

Zie de beschrijvingen van elk vooraf biedende filter op &quot;[Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken](/help/dsp/optimization/optimization-pre-bid-filters.md).&quot;

### Alle andere plaatsen

**[!UICONTROL Budget Goal]:** Het bruto-begrotingsmaximum en het begrotingsinterval (*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Gross Budget Goal]:** (Plaatsen in campagnes met alleen margebeheer) Het bruto-begrotingsmaximum en het begrotingsinterval (*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Optimization Goal]:**  De optimalisatiedoelstelling voor het pakket. Zie beschrijvingen van elk optimalisatiedoel op &quot;[Optimalisatiedoelstellingen en hoe deze te gebruiken](/help/dsp/optimization/optimization-goals.md)&quot;.

**[!UICONTROL Target Goal]:** Het doeldoel, dat wordt gebruikt om prestaties te volgen.

>[!NOTE]
>
>Dit veld is alleen een benchmark en wordt niet gebruikt voor beslissingen.

**[!UICONTROL Pace on]:** Waarop wordt de pakketindeling gebaseerd:

* **[!UICONTROL Budget goal]:** (Standaardinstelling) Met deze optie krijgt u zoveel mogelijk indruk binnen het toegewezen budget.

* **[!UICONTROL Impressions]:** Met deze optie worden afbeeldingen afgedrukt totdat een opgegeven hoeveelheid binnen een opgegeven interval wordt bereikt. Wanneer u deze optie selecteert, geeft u het aantal afbeeldingen en het interval op: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Max Bid]:** Het maximum dat voor 1000 beelden moet worden betaald.

**[!UICONTROL Flight pacing]:** (Plaatsen met plaatsing-vlakke slechts het verpakken) Hoe te plaats en levering:

* *[!UICONTROL Even]:* (De standaardinstelling) Hiermee wordt de levering op uniforme wijze gedurende elke vlucht uitgevoerd, met als doel 50% van de levering tijdens de eerste helft van de vlucht.

* *[!UICONTROL Slightly Ahead]:* (De standaardwaarde) versnelt de levering zodat deze 55-65% volledig halverwege de vliegduur is.

* *[!UICONTROL Frontload]:* Versnelt de levering zodat deze 65-75% volledig halverwege de vlucht is.

* *[!UICONTROL Aggressive Frontload]:* Versnelt de levering zodat deze 75-85% volledig halverwege de vlucht is.

**[!UICONTROL Intraday pacing]:** (Plaatsen met alleen plaatsing op plaatsingsniveau) Hoe plaatst en levert u de levering over elke dag in de vlucht:

* *[!UICONTROL Even]:* (De standaardinstelling) Schaalt de levering op basis van de beschikbaarheid van de voorraad. Over het algemeen worden meer advertenties overdag per uur geleverd, wanneer het veilingsvolume hoger is en er minder advertenties &#39;s ochtends en &#39;s avonds worden geleverd.

* *[!UICONTROL ASAP]:* (De standaardwaarde) versnelt de levering tot tweemaal de snelheid van *Even*.

   >[!CAUTION]
   >
   >Deze optie kan de prestaties negatief beïnvloeden. Gebruik dit alleen als u volledige prioriteit geeft aan levering en meer geld besteedt aan optimalisatie van prestaties.

**[!UICONTROL Placement Pre-bid Filters]:** (Optioneel) Maximaal vijf filters waaraan moet worden voldaan om te kunnen bieden. U kunt voorbiedingsfilters gebruiken als optimalisatietechniek, maar houd er rekening mee dat elke regel de mogelijkheden waarop deze plaatsing kan bieden, kan beperken. Filters toevoegen of bewerken:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een filter toevoegen:
      1. Klik op **[!UICONTROL Add Filter]**.
      1. Volgende tot **[!UICONTROL Only bid if]** selecteert u een metrische waarde en voert u een waarde in.
   * Als u een filter wilt verwijderen, klikt u op **[!UICONTROL X]** in de filterrij.
1. Klik op **[!UICONTROL Save]**.

## [!UICONTROL Geo-Targeting]

**[!UICONTROL Audience Location]:** (Optioneel) Specifieke locaties waar advertenties in de plaatsing moeten worden opgenomen of uitgesloten. Als u geen plaatsen specificeert, worden alle plaatsen gericht.

>[!NOTE]
>
>De plaatsen van de Stad en DMA zijn niet beschikbaar voor Plaatsen Roku.

Locaties opgeven:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een land, een staat, een stad, een DMA, een federaal wetsdistrict of een wetsdistrict van een staat op te nemen of uit te sluiten:
      1. Selecteer het locatietype in de linkerkolom.
      1. (Indien nodig) Klik op een locatie om deze uit te vouwen.
      1. Klik naast de locatie op *[!UICONTROL Include]* om het als doel op te nemen of *[!UICONTROL Exclude]* om het als doel uit te sluiten.
   * U kunt als volgt naar een postcode zoeken en alle geselecteerde resultaten opnemen of uitsluiten:
      1. Klik op **[!UICONTROL Search Postal Code]**.
      1. Selecteer het land.
      1. Voer de naam van de stad in en klik op ![Bewerken](/help/dsp/assets/search.png).
      1. Klik op het juiste zoekresultaat.
      1. Klikken *[!UICONTROL Include All]* om alle locaties op te nemen als doelen of *[!UICONTROL Exclude All]* om alle locaties als doelen uit te sluiten.
   * U kunt als volgt postcodes invoeren of plakken en deze allemaal opnemen of uitsluiten:
      1. Klik op **[!UICONTROL Paste Postal Code]**.
      1. Selecteer het land.
      1. Voer maximaal 1000 postcodes in of plak deze.
Neem één postcode per regel op of voer meerdere waarden in, gescheiden door komma&#39;s of tabs.
      1. Klikken *[!UICONTROL Include All]* om alle locaties op te nemen als doelen of *[!UICONTROL Exclude All]* om alle locaties als doelen uit te sluiten.
   * Een locatie verwijderen uit het dialoogvenster [!UICONTROL Included] of [!UICONTROL Excluded] lijst, klikt u op **[!UICONTROL X]** naast de locatie in de rechterkolom.
1. Klik op **[!UICONTROL Done]**.

>[!NOTE]
>
>* Niet alle landen hebben de locatie Staat, de plaats of de postcode.
>* DMA (aangewezen marktgebied), Federal Legislative Districts, en de Wetgevende Districten van de Staat zijn beschikbaar voor de plaatsen van de V.S. slechts.


## [!UICONTROL Inventory Targeting]

**[!UICONTROL Inventory Sources]:** Inventarisatiebronnen die als doel moeten worden opgenomen of uitgesloten. Voor de meeste plaatsingstypen worden alle voorraadtypen en alle bronnen voor elk type standaard opgenomen. Voor [!DNL Roku] U moet het voorraadtype en de bronnen opgeven. U kunt uit de volgende soorten inventaris kiezen:

* [!UICONTROL Public]: (Alle plaatsingstypen behalve Roku) Alle open uitwisselingsvoorraden waartoe DSP toegang heeft. U kunt openbare voorraad opnemen en uitsluiten.

   U kunt de lijst bekijken door bron of door voer. Wanneer u de lijst weergeeft op basis van feed, kunt u zoeken op naam van de feed, op basis van de feed of op basis van een geselecteerde kenmerkende tag.

* [!UICONTROL Private] | [!UICONTROL Roku Private]: Uw bestaande privé overeenkomsten (of bestaande privé [!DNL Roku] deals voor [!DNL Roku] plaatsen) bij uitgevers die u in DSP hebt ingesteld. U kunt een openbare voorraad opnemen, maar niet uitsluiten.

   U kunt de lijst zoeken op trefwoord, sleutel, deal-id of aangepaste tag.

* [!UICONTROL On Demand] | [!UICONTROL Roku On Demand]: Alles [premie, niet gegarandeerd [!UICONTROL On Demand] voorraad](/help/dsp/inventory/on-demand-inventory-about.md) (of [!UICONTROL On Demand] [!DNL] Roku-deals voor [!DNL Roku] plaatsen) waarop u zich hebt geabonneerd [!DNL DSP]. U kunt opnemen en uitsluiten [!UICONTROL On Demand] voorraad.

   U kunt de lijst bekijken door bron of door voer. Wanneer u de lijst op feed weergeeft, kunt u zoeken op naam van feed, feed-sleutel of een geselecteerd uitgeversgebied, een categorietag of een kenmerkende tag.

Opgeven welke inventarisdoelen worden gebruikt:

* Als u een voorraadtype wilt uitsluiten, schakelt u het selectievakje naast de naam uit.
* Een voorraadtype als doel instellen:
   1. Schakel het selectievakje naast de naam van het voorraadtype in.
   1. (Optioneel) Wijzig de bronnen in:
      1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
      1. ([!UICONTROL Public] en [!UICONTROL On Demand] voorraad) Klik *[!UICONTROL *View by Source]** of **[!UICONTROL View by Feed]** om te wijzigen hoe de bronnen worden weergegeven.
      1. (Indien van toepassing) Filter de voorraad naar wens.
      1. Geef de bronnen op die u wilt opnemen en uitsluiten:
         * Als u een [!UICONTROL Public] of [!UICONTROL On Demand] bron, klik **[!UICONTROL Include]** naast de bronnaam.
         * Opnemen [!UICONTROL Private] bronnen:
            * Als u alle voorraad in een deal wilt opnemen, klikt u op **[!UICONTROL Include all]** naast de overeenkomstennaam.
            * Om een individuele inventarisbron te omvatten, breid de overeenkomstennaam uit, en klik dan het controlevakje naast de bronnaam.
         * Een [!UICONTROL Public] of [!UICONTROL On ] bron, klik **[!UICONTROL Exclude]** naast de bronnaam.
   1. (Optioneel) Als u een CSV-bestand met de doelgegevens wilt downloaden naar de downloadlocatie van uw browser, klikt u op **[!UICONTROL Save & Export]**.
   1. Klik op **[!UICONTROL Save]**.

>[!TIP]
>
>Als u zich hebt geabonneerd op [!UICONTROL On Demand] inventariseren, maar de uitgevers of deals kunnen niet worden gevonden als doel, en vervolgens de status van de deals controleren. Voor meer informatie over statussen raadpleegt u [Info [!DNL On Demand] Premium-voorraad](/help/dsp/inventory/on-demand-inventory-about.md).

**[!UICONTROL Exclude out-stream]:** (Alleen videoplaatsingen) Hiermee sluit u het stroomafwaartse verkeer uit.

Outstream-advertenties worden doorgaans als een pop-up of opgevuld in inhoud (in de eigen ervaring) weergegeven in plaats van als gewone videobanden in een videospeler.

## [!UICONTROL Site Targeting]

**[!UICONTROL Traffic type]:** De types van verkeer aan doel. Opties omvatten **[!UICONTROL Websites]** en **[!UICONTROL Apps]**.

**[!UICONTROL Site tier]:** (Beschikbaar als **[!UICONTROL Paste list of targeted sites]** is *[!UICONTROL Off]*) De kwaliteit van de sites waarop u zich wilt richten. Tiers 1-3 zijn allemaal merkveilig en zijn gecontroleerd en goedgekeurd door het DSP-kaartteam.

* *[!UICONTROL Tier 1]:* Premiumsites en -toepassingen die nationaal herkenbaar zijn.
* *[!UICONTROL Tier 2]:* Streefcijfers voor Niveau 1 en kwaliteitsites en toepassingen die minder bekend zijn dan Niveau 1.
* *[!UICONTROL Tier 3]:* Doeltips 1-2 en legitieme en brandveilige sites en toepassingen die geschikt zijn voor een nichepubliek. Gebruik Niveau 3 voor bereik of gegevens die op aankopen gericht zijn.
* *[!UICONTROL All Sites]:* Doeltips 1-3 en nieuwe voorraad die niet is gescreend of gecategoriseerd en die u kunt gebruiken om te bereiken.

>[!NOTE]
>
>Inventaris is specifiek voor de advertentie-eenheden in de plaatsing.

>[!TIP]
>
>Voor prestatiecampagnes moet u *[!UICONTROL All Sites]*.

**[!UICONTROL Site Categories]:** (facultatief; beschikbaar als **[!UICONTROL Paste list of targeted sites]** is *[!UICONTROL Off]*) Sitecategorieën binnen de geselecteerde siteniveaus om deze als doelen op te nemen of uit te sluiten (maar niet beide). Maak een keuze uit verticale sitelijsten die DSP toegewezen op basis van het onderwerp van de site:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sitecategorieën op die u wilt opnemen of uitsluiten:
   * Sitecategorieën opnemen:
      1. Klik op **[!UICONTROL Include categories]**.
      1. Schakel het selectievakje naast elke categorie in die u wilt activeren.
   * Sitecategorieën uitsluiten:
      1. Klik op **[!UICONTROL Exclude categories]**.
      1. Schakel het selectievakje naast elke categorie in die u wilt uitsluiten.
1. (Optioneel) Als u een CSV-bestand met de doelgegevens wilt downloaden naar de downloadlocatie van uw browser, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Exclude Sites]:** (facultatief; beschikbaar als **[!UICONTROL Paste list of targeted sites]** is *[!UICONTROL Off]*) Sites die moeten worden uitgesloten. U kunt zoeken naar sites en deze selecteren, of u kunt domeinnamen invoeren of plakken:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sites op:
   * Ga als volgt te werk om een site te zoeken:
      1. Klik op **[!UICONTROL Search]**.
      1. Voer een trefwoord in, selecteer een sitelaag en/of selecteer een sitecategorie.
      1. Selecteer in de zoekresultaten de sites die u wilt uitsluiten:
         * Als u een afzonderlijke site wilt uitsluiten, schakelt u het selectievakje naast de site in.
         * (Als er meer dan 50 resultaten beschikbaar zijn) Als u de eerste 50 resultaten wilt uitsluiten, klikt u op **[!UICONTROL Exclude these 50]**. Als u alle zoekresultaten wilt uitsluiten, klikt u op **[!UICONTROL Exclude these \<*NN *\>]**.
   * Domeinnamen invoeren:
      1. Klik op **[!UICONTROL Paste]**.
      1. Voer een of meer domeinnamen op afzonderlijke regels in.
      1. Klik op **[!UICONTROL Exclude All]**.
1. Klikken **[!UICONTROL Done]** als je klaar bent.

>[!NOTE]
>
>* Naast de DSP worden ook lijsten met geblokkeerde sites op accountniveau en door adverteerders gebruikt [globaal geblokkeerde sitelijst](/help/dsp/introduction/features/brand-safety-media-quality.md), waaronder plaatsen die onveilig worden geacht voor advertenties.
>* Lijsten met geblokkeerde sites hebben altijd voorrang op lijsten met doelsites. Als een plaatsing zowel het zelfde doel voor een advertentie uitsluit als omvat, dan wordt het doel uitgesloten.


**[!UICONTROL Language]:** (Optioneel) Eén taal waarop u zich wilt richten.

**[!UICONTROL Site List Preview]:** (Alleen-lezen) Alle beoogde en geblokkeerde sites voor de plaatsing.

U kunt de lijst met doelsites en geblokkeerde sites optioneel exporteren als een CSV-bestand (comma-separated values, door komma&#39;s gescheiden waarden). Als u de lijst wilt exporteren, klikt u op **[!UICONTROL Export full site list]** en open of sla het bestand op volgens de normale procedure van uw browser.

**[!UICONTROL Allow unscreened sites]:** (Alleen standaardpresentaties) Hiermee kunt u levering en levering op niet-gecontroleerde sites mogelijk maken. Wanneer de plaatsing privé-inventarisatie als doel heeft, kan deze optie advertenties op geblokkeerde sites leveren.

**[!UICONTROL Paste list of targeted sites]:** Hiermee kunt u alleen specifieke sites als doel instellen. Wanneer u deze optie inschakelt, worden de andere opties voor het instellen van doelen voor de site uitgeschakeld.

**[!UICONTROL Sites]:** (Beschikbaar als **[!UICONTROL Paste list of targeted sites]** is *[!UICONTROL On]*) Sites waarop u zich wilt richten. U kunt zoeken naar sites en deze selecteren, of u kunt domeinnamen invoeren of plakken:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sites op:
   * Ga als volgt te werk om een site te zoeken:
      1. Klik op **[!UICONTROL Search]**.
      1. Voer een trefwoord in, selecteer een sitelaag en/of selecteer een sitecategorie.
      1. Selecteer in de zoekresultaten de sites die u wilt opnemen:
         * Als u een afzonderlijke site wilt uitsluiten, schakelt u het selectievakje naast de site in.
         * (Als er meer dan 50 resultaten beschikbaar zijn) Als u de eerste 50 resultaten wilt opnemen, klikt u op **[!UICONTROL Include these 50]**. Als u alle zoekresultaten wilt opnemen, klikt u op **[!UICONTROL Include these \<*NN *\>]**.
   * Domeinnamen invoeren:
      1. klikken **[!UICONTROL Paste]**.
      1. Voer een of meer domeinnamen op afzonderlijke regels in.
      1. Klik op **[!UICONTROL Include All]**.
1. Klik op **[!UICONTROL Done]**.

## [!UICONTROL Audience Targeting]

**[!UICONTROL Included Audiences]:** Alle publieksdoelen voor de plaatsing, inclusief [segmenten van derden, segmenten van eerste bedrijven, Adobe-segmenten, aangepaste segmenten en opgeslagen doelgroepen](/help/dsp/audiences/audience-settings.md). De totale en actieve gededupliceerde publieksgrootte voor alle geselecteerde segmenten en opgeslagen doelgroepen wordt ook weergegeven. U kunt een bestaand publiek selecteren, een nieuw publiek maken dat u later opnieuw kunt gebruiken of specifieke publiekssegmenten selecteren:

* Als u een bestaand publiek wilt selecteren, klikt u op ![Selecteren](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Included Audiences]en selecteer vervolgens het publiek.
* Als u een nieuw publiek wilt maken, klikt u op ![Selecteren](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Included Audiences]en selecteer vervolgens **[!UICONTROL + Create Audience]**. Zie voor instructies [Een herbruikbaar publiek maken](/help/dsp/audiences/reusable-audience-create.md), te beginnen met Stap 3.
* Om specifieke publiekssegmenten te selecteren, klik **[!UICONTROL Select segments for this placement only]**. Selecteer de segmentlogica. voor instructies, zie Stap 6 in &quot;[Een herbruikbaar publiek maken](/help/dsp/audiences/reusable-audience-create.md).&quot; Als u klaar bent, klikt u op **Opslaan**.

**[!UICONTROL Excluded Audiences]:** Alle soorten publiek die voor de plaatsing moeten worden uitgesloten, inclusief publiek met [segmenten van derden, segmenten van eerste bedrijven, Adobe-segmenten, aangepaste segmenten en opgeslagen doelgroepen](/help/dsp/audiences/audience-settings.md). De totale en actieve gededupliceerde publieksgrootte voor alle uitgesloten doelgroepen wordt ook weergegeven. U kunt een bestaand publiek selecteren of een nieuw publiek maken dat u later opnieuw kunt gebruiken:

* Als u een bestaand publiek wilt selecteren, klikt u op ![Selecteren](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Excluded Audiences]en selecteer vervolgens het publiek.
* Als u een nieuw publiek wilt maken, klikt u op ![Selecteren](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Excluded Audiences]en selecteer vervolgens **+ Publiek maken**. Zie voor instructies [Een herbruikbaar publiek maken](/help/dsp/audiences/reusable-audience-create.md), te beginnen met Stap 3.

**[!UICONTROL Cross Device Targeting]:** (Beschikbaar als u ten minste één segment of publiek selecteert en [campagne is geconfigureerd voor apparaatspecifieke doelgroepen](/help/dsp/campaign-management/campaigns/campaign-settings.md). Staat u toe om uw het richten over alle bekende apparaten van een persoon (per de apparatengrafiek uit te breiden die in de campagnemontages wordt gespecificeerd), zelfs apparaten die niet in de gespecificeerde segmenten zijn. De kosten kunnen van toepassing zijn afhankelijk van de grafiek die voor de campagne wordt gespecificeerd. Apparaatgrafiekgegevens zijn momenteel alleen beschikbaar in Noord-Amerika.

**[!UICONTROL Placement Cap]:** (Optioneel) Het aantal keren dat een uniek apparaat of een unieke persoon (afhankelijk van het opgegeven apparaat of de opgegeven persoon) [!UICONTROL Cross Device Level] voor de campagne ) worden advertenties aangeboden vanaf de plaatsing . Opties omvatten *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand.

>[!NOTE]
>
> U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

**[!UICONTROL Secondary Cap]:** (facultatief; beschikbaar wanneer u een numerieke waarde toevoegt [!UICONTROL Placement Cap]) Een extra beperking binnen de grenzen van de primaire plaatsingsdop. Selecteer het aantal afbeeldingen en de tijdsperiode (bijvoorbeeld 3 per 12 uur).

**[!UICONTROL Day Parting]:** (Optioneel) Specifieke dagen van de week en het tijdstip van de dag waarop advertenties kunnen worden uitgevoerd. De zomerintervallen opgeven:
1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Selecteer de toepasselijke tijdzone.
1. Geef de intervallen op:
   * Klik op een van de intervalknoppen om een vooraf ingesteld interval te selecteren. Opties zijn *[!UICONTROL Weekends]**, *[!UICONTROL Weekdays]*, *[!UICONTROL Morning]*, *[!UICONTROL Lunch]*, *[!UICONTROL Dinner]*, of *[!UICONTROL Prime]* (primetime).
   * Als u handmatig een interval wilt selecteren, klikt u in een cel en sleept u optioneel om het interval te selecteren.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Topic Targeting]:** (facultatief; beschikbaar voor adverteerders die zijn geconfigureerd met [!DNL Comscore] en [!DNL Grapeshot] segmenten) Specifieke segmentnamen of id&#39;s van [!DNL Comscore] en [!DNL Grapeshot] op te nemen als streefcijfers. Voor deze functie kunnen extra kosten in rekening worden gebracht. Neem contact op met uw [!DNL Adobe] accountteam.

Onderwerpgerichte onderwerpen opgeven:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de gewenste segmenten op:
   1. Selecteer in de linkerkolom de partner (*[!UICONTROL Comscore]* of *[!UICONTROL Grapeshot]*).
   1. Voer in het invoerveld de segmentnamen of segment-id&#39;s in.
1. (Optioneel) Als u een CSV-bestand met de onderwerpgegevens wilt downloaden naar de downloadlocatie van uw browser, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

>[!TIP]
>
>* Objectgerichte aanbiedingen beperken de voorraad waarop de plaatsing kan bieden. Gebruik daarom onderwerpen die voor slechts een klein percentage van de totale aankoop zijn bestemd.
>
>* Stel eventuele negatieve doelen in binnen het segment op [!DNL Comscore] of [!DNL Grapeshot].


**[!UICONTROL Device Targeting]:** (Optioneel) Specifieke apparaatinformatie, zoals apparaattypen, fabrikanten, besturingssystemen, browsers en connectiviteitstypen, om deze op te nemen en uit te sluiten als doel. Apparaatdoelframes opgeven:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de apparaatdetails op die u wilt opnemen en uitsluiten:
   1. Selecteer de categorie in de linkerkolom.
   1. Doelstelling opgeven:
      * Als u een waarde wilt opnemen, klikt u op **[!UICONTROL Include]** naast de naam van de waarde.
      * Als u een waarde wilt uitsluiten, klikt u op **[!UICONTROL Exclude]** naast de naam van de waarde.
1. (Optioneel) Als u een CSV-bestand met de doelgegevens van het apparaat wilt downloaden naar de downloadlocatie van uw browser, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL ISP Targeting]:** (Optioneel) Specifieke internetserviceproviders (ISP&#39;s) om deze als doel op te nemen of uit te sluiten (maar niet beide). Om ISP het richten te specificeren:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Specificeer ISPs om te omvatten of uit te sluiten:
   * ISPs omvatten:
      1. Klik op **[!UICONTROL Include ISPs]**.
      1. (Optioneel) Filter de lijst op trefwoord.
      1. Selecteer de controledoos naast elke ISP aan doel.
   * ISPs uitsluiten:
      1. Klik op **[!UICONTROL Exclude ISPs]**.
      1. (Optioneel) Filter de lijst op trefwoord.
      1. Selecteer de controledoos naast elke ISP om uit te sluiten.
1. (Optioneel) Als u een CSV-bestand met de ISP-doelgegevens wilt downloaden naar de downloadlocatie van uw browser, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

## [!UICONTROL Brand Safety and Media Targeting]

**[!UICONTROL Contextual filtering]:** Typen [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39] contextafhankelijke filters die moeten worden toegepast. De standaardinstellingen op adverteerderniveau worden geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een of meer typen voorraadcontext die standaard worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Peer 39]:

   * **Doelsites:** (Optioneel) Een of meer typen voorraadkenmerken die standaard als doel moeten worden ingesteld. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL ComScore]:

   * **Bloksites die zijn:** (Optioneel) Een of meer typen voorraadkenmerken die standaard moeten worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Integral Ad Science]

   * **[!UICONTROL Adult Content]:** (Optioneel) De mate van inhoud voor volwassenen waarvoor advertenties standaard worden geblokkeerd: *[!UICONTROL Do Not Block]* (standaard), *[!UICONTROL Standard]*, of *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

   * **[!UICONTROL Alcohol Content]:** (Optioneel) Het alcoholgehalte waarvoor standaard advertenties worden geblokkeerd: *[!UICONTROL Do Not Block]* (standaard), *[!UICONTROL Standard]*, of *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Pre-bid fraud blocking]:** Soorten sites die moeten worden geblokkeerd op basis van frauduleus verkeer en verdachte activiteiten, gemeten via [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39]. De standaardinstellingen op adverteerderniveau worden geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** Door gebrek, blokkeert al 100% ongeldig verkeer, met inbegrip van verkeer op benadrukte apparaten, voor nieuwe plaatsen. Er kunnen extra kosten van toepassing zijn.

   * **[!UICONTROL Also block sites with]:** (Optioneel) Een extra niveau van fraude en ongeldig verkeer waardoor DSP standaard advertenties blokkeert:  *[!UICONTROL None]* (het gebrek, dat geen extra verkeer blokkeert), *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*, *[!UICONTROL >4% Average Fraud/IVT levels]*, *[!UICONTROL >6% Average Fraud/IVT levels]*, *[!UICONTROL >10% Average Fraud/IVT levels]*, of *[!UICONTROL >25% Average Fraud/IVT levels]*. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Peer 39]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een of meer soorten fraude waardoor DSP standaard advertenties blokkeert: *[!UICONTROL Fraud]* (die alle sites blokkeert met fraude), *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]*, en/of *[!UICONTROL Fraud: Zero Ads]*. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Integral Ad Science]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een type verdachte website- of app-activiteit waardoor DSP standaard advertenties blokkeert: *[!UICONTROL None]* (de standaardwaarde, die geen advertenties blokkeert op basis van verdachte activiteit), *[!UICONTROL Suspicious Activity - High Risk]*, of *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Ads.txt filtering]:**

Welk niveau van [Ads.txt](https://iabtechlab.com/ads-txt-about/) Filteren vóór bieden om te gebruiken door gebruik te maken van de lijst met geautoriseerde digitale verkopers van elke uitgever. De standaardinstelling op advertentieniveau is geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* *[!UICONTROL Opt out of ads.txt (default)]*: Winkel kopen van alle verkopers.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: Prioriteit geven aan inkoopvoorraad van geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers van een domein.

**[!UICONTROL DoubleVerify Authentic Brand Safety]:** (Adverteerders geconfigureerd met de [!UICONTROL DoubleVerify Authentic Brand Safety] optie) Inschakelen [!DNL DoubleVerify Authentic Brand Safety], die indrukkingen na het bieden blokkeert met de aangepaste merkveiligheidsregels die voor de opgegeven segment-id zijn geconfigureerd. DSP uw account aan voor gebruik van de segment-id die in de adverteerderinstellingen is opgegeven.

## [!UICONTROL Tracking] {#placement-tracking}

>[!NOTE]
>
>([!DNL Roku] plaatsingen) Verkopers van trackingservices van derden die zijn goedgekeurd door [!DNL Roku] include [!DNL Acxiom], [!DNL comScore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk], en [!DNL Research Now].

**[!UICONTROL Event Pixels]:** (Optioneel) Pixels voor het bijhouden van gebeurtenissen van derden die standaard worden gekoppeld aan alle nieuwe advertenties in de plaatsing. Gebeurtenispixels opgeven:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Als u een bestaande pixel wilt selecteren, schakelt u het selectievakje in de pixelrij in.
   * Een nieuwe pixel maken:
      1. Klik op **[!UICONTROL Create]**.
      1. Voer de volgende gegevens in:
         * **[!UICONTROL Pixel name]:** De pixelnaam; de maximumlengte is 500 tekens. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.
         * **[!UICONTROL Pixel event fires on]:** De gebeurtenis die de pixel activeert. De beschikbare gebeurtenissen variëren per advertentietype.
         * **[!UICONTROL Pixel type]:** Of de pixel een *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel), *[!UICONTROL HTML]*, of *[!UICONTROL JavaScript URL]*.
         * **[!UICONTROL Pixel URL]:** De URL van de pixelafbeelding.
      1. Klik op **[!UICONTROL Create and attach]**.
   1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Conversion Pixels]:** (Optioneel) Pixels voor het bijhouden van de conversie die standaard worden gekoppeld aan alle nieuwe advertenties in de plaatsing. Omzetpixels opgeven:

1. Klikken ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Als u een bestaande pixel wilt selecteren, schakelt u het selectievakje in de pixelrij in.
   * Een nieuwe pixel maken:
      1. Klik op **[!UICONTROL Create]**.
      1. Voer de volgende gegevens in:
         * **[!UICONTROL Conversion pixel name]:** De pixelnaam; de maximumlengte is 500 tekens. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.
         * **[!UICONTROL Conversion category]:** Het type conversie.
         * **[!UICONTROL Impression conversion window]:** Het aantal dagen na een advertentie waarin de indruk aan een conversie kan worden toegeschreven. De standaardwaarde is 30 dagen.
         * **[!UICONTROL Click conversion window]:** Het aantal dagen na een advertentie waarop de klik kan worden toegewezen aan een conversie. De standaardwaarde is 30 dagen.
         * **[!UICONTROL Notes]:** (Optioneel) Een beschrijving of andere informatie over de pixel.
      1. Klik op **[!UICONTROL Create and attach]**.
      1. Implementeer de conversiepixel op de relevante webpagina&#39;s:
         1. Ga in het hoofdmenu naar **[!UICONTROL Resources]>[!UICONTROL Conversion pixels]**.
         1. Klik in de pixelrij op **[!UICONTROL edit]**.
         1. Kopieer de waarde(n) in de [!UICONTROL HTML Tag] en [!UICONTROL Flash Tag] velden, indien nodig, om de adverteerder of de websitecontactpersoon te voorzien.

            De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.
   1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL 3rd-party Fees]:** (Optioneel) Een statisch tarief voor vergoedingen van derden dat moet worden bijgehouden als niet-factureerbare kosten per 1000 impressies. De standaardinstelling op pakketniveau wordt, indien van toepassing, automatisch toegepast op nieuwe plaatsingen, tenzij u een andere waarde opgeeft.

>[!NOTE]
>
>Facultatieve vergoedingen worden weerspiegeld in de [!UICONTROL Net CPM] metrisch.

>[!MORELIKETHIS]
>
>* [Info over Plaatsingsbeheer](placement-about.md)
>* [Een plaatsing maken](placement-create.md)
>* [Een plaatsing bewerken](placement-edit.md)
>* [Het Wijzigingslogboek voor een plaatsing weergeven](placement-change-log.md)
>* [Sneltoetsen](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [Veelgestelde vragen over Campaign Management](/help/dsp/campaign-management/campaign-management-faq.md)

