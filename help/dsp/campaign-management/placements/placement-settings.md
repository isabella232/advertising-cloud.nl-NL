---
title: Plaatsingsinstellingen
description: Zie beschrijvingen van de beschikbare plaatsingsmontages.
feature: DSP Placements
exl-id: 36097132-e589-4d49-bf86-54f61eae5b67
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '3281'
ht-degree: 0%

---

# Plaatsingsinstellingen

## [!UICONTROL Basics]

**[!UICONTROL Placement name]** De plaatsingsnaam.

>[!TIP]
>Gebruik een naamgevingsconventie die voor uw situatie zinnig is. Een gesuggereerde naamgevingsconventie is &quot;*\&lt;Naam campagne\>: \&lt;Advertentie-eenheid\>: \&lt;Duration\>: \&lt;Targeting\>*.&quot;

**[!UICONTROL Status]:** De plaatsingsstatus:  *[!UICONTROL Active]* (de standaardwaarde) of  *[!UICONTROL Paused]*.

>[!TIP]
>De beste manier is om de plaatsing te pauzeren tot u bereid bent om het te lanceren.

**[!UICONTROL Details]:** (Alleen-lezen) Het toepasselijke advertentietype, de account die de plaatsing maakt of heeft gemaakt, en de bovenliggende campagne. Klik op **[!UICONTROL Show more]** voor meer informatie.

**[!UICONTROL Templates]:** Hiermee opent u een lijst met bestaande plaatsingssjablonen. Als u doelinstellingen automatisch wilt invullen vanuit een sjabloon:

1. Voer een van de volgende handelingen uit:

   * Als u al het doel uit een sjabloon opnieuw wilt gebruiken, schakelt u het selectievakje naast de sjabloonnaam in.

   * Als u afzonderlijke doeltypen uit een sjabloon opnieuw wilt gebruiken, vouwt u de sjabloonnaam uit en schakelt u het selectievakje in naast de doeltypen die u opnieuw wilt gebruiken.

1. Klik op **[!UICONTROL Apply]**.

**[!UICONTROL Ad specs for forecast]:** (Alleen video en indelingen) De duur van de advertentie en/of de specificaties van de advertentie, die worden gebruikt om de voorspelde projectie aan de rechterkant te berekenen. De velden verschillen per advertentietype.

**[!UICONTROL Placement tags]:** (Optioneel) Trefwoorden of bijnamen om u te helpen deze plaatsing te vinden.

## Doelen

**[!UICONTROL Package]:** (Optioneel) Een pakket waaraan de plaatsing is toegewezen. Klik ![Bewerken](/help/dsp/assets/edit.png) om een bestaand pakket te selecteren en te maken of een nieuw pakket te maken. Wanneer u de plaatsing aan een pakket toewijst, wordt de [!UICONTROL Goals] sectie bijgewerkt met de vluchtdata, leveringsdoel, en begroting van het pakket.

**[!UICONTROL Flight Dates]:** De begindatum en einddatum voor de plaatsing. Goedgekeurde advertenties komen in aanmerking om tijdens de vlucht te worden uitgevoerd wanneer de plaatsing actief is en wordt toegewezen aan een actief pakket of een actieve campagne.

De datums voor het pakket (indien van toepassing) of de campagne worden standaard automatisch ingevuld.

>[!NOTE]
>
>* De vluchtdata moeten worden opgenomen in de campagnevluchtdata en de pakketvliegdata.


### Plaatsen die aan Pakketten met pakket-vlakke Tussenruimte worden toegewezen

**[!UICONTROL Placement Funding]:** Hoe begroot u de plaatsing?

* *[!UICONTROL Optimize based on performance]:* Hiermee bepaalt u de begroting op pakketniveau.
* *[!UICONTROL Set a fixed budget cap]:* Hiermee kunt u een budget voor dagelijkse, wekelijkse, maandelijkse of volledige plaatsing instellen. Voer een waarde en de duur in (*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Max Bid]:** Het maximum dat wordt betaald voor 1000 afbeeldingen.

**[!UICONTROL Placement Pre-bid Filters]:** Tot vijf KPI drempels (zoals een minimum viewability metrisch of klik-door tarief) die moeten worden ontmoet om te bieden voor te komen. U kunt voorbiedingsfilters gebruiken als optimalisatietactiek, maar u weet dat elke regel de mogelijkheden waarop deze plaatsing kan bieden, kan beperken. Filters toevoegen of bewerken:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een filter toevoegen:
      1. Klik op **[!UICONTROL Add Filter]**.
      1. Naast **[!UICONTROL Only bid if]**, selecteer metrisch, en ga dan een waarde in.
   * Als u een filter wilt verwijderen, klikt u op **[!UICONTROL X]** in de filterrij.
1. Klik op **[!UICONTROL Save]**.

Zie beschrijvingen van elk vooraf biedende filter op &quot;[Plaatsingsniveau pre-Bodfilters en hoe te om hen ](/help/dsp/optimization/optimization-pre-bid-filters.md) te gebruiken.&quot;

### Alle andere plaatsen

**[!UICONTROL Budget Goal]:** Het bruto-begrotingsmaximum en het begrotingsinterval (*[!UICONTROL All time]*,  *[!UICONTROL Daily]*,  *[!UICONTROL Weekly]*,  *[!UICONTROL Monthly]*).

**[!UICONTROL Gross Budget Goal]:** (Plaatsingen in campagnes met alleen margebeheer) Het bruto-begrotingsmaximum en het begrotingsinterval (*[!UICONTROL All time]*,  *[!UICONTROL Daily]*,  *[!UICONTROL Weekly]*,  *[!UICONTROL Monthly]*).

**[!UICONTROL Optimization Goal]:**  De optimalisatiedoelstelling voor het pakket. Zie beschrijvingen van elk optimalisatiedoel bij &quot;[Optimalisatiedoelstellingen en hoe te om hen ](/help/dsp/optimization/optimization-goals.md)&quot;te gebruiken.

**[!UICONTROL Target Goal]:** Het doeldoel, dat wordt gebruikt om prestaties te volgen.

>[!NOTE]
>
>Dit veld is alleen een benchmark en wordt niet gebruikt voor beslissingen.

**[!UICONTROL Pace on]:** Waarop wordt de spatiëring gebaseerd:

* **[!UICONTROL Budget goal]:** (Standaard) Deze optie levert zoveel mogelijk indrukken binnen de toegewezen begroting.

* **[!UICONTROL Impressions]:** Deze optie levert beelden tot een gespecificeerde hoeveelheid binnen een gespecificeerd interval wordt bereikt. Wanneer u deze optie selecteert, geeft u het aantal afbeeldingen en het interval op: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Max Bid]:** Het maximum dat wordt betaald voor 1000 afbeeldingen.

**[!UICONTROL Pacing Fill Strategy]:** (Pakketten met pakket-vlakke het verpakken slechts) hoe te plaats en levering:

* *[!UICONTROL Even]:* (De standaardwaarde) Plaatst gelijkmatig levering door elke vlucht, met een doel van 50% van de levering in de eerste helft van de vlucht.

* *[!UICONTROL Frontload]:* Versnelt levering zodat het 65-75% volledig halverwege de vlucht is.

* *[!UICONTROL Aggressive Frontload]:* Versnelt levering zodat het 75-85% volledig halverwege de vlucht is.

**[!UICONTROL Placement Pre-bid Filters]:** (Optioneel) Maximaal vijf filters waaraan moet zijn voldaan om te kunnen bieden. U kunt voorbiedingsfilters gebruiken als optimalisatietechniek, maar houd er rekening mee dat elke regel de mogelijkheden waarop deze plaatsing kan bieden, kan beperken. Filters toevoegen of bewerken:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een filter toevoegen:
      1. Klik op **[!UICONTROL Add Filter]**.
      1. Naast **[!UICONTROL Only bid if]**, selecteer metrisch, en ga dan een waarde in.
   * Als u een filter wilt verwijderen, klikt u op **[!UICONTROL X]** in de filterrij.
1. Klik op **[!UICONTROL Save]**.

## [!UICONTROL Geo-Targeting]

**[!UICONTROL Audience Location]:** (Optioneel) Specifieke locaties waar advertenties in de plaatsing moeten worden opgenomen of uitgesloten. Als u geen plaatsen specificeert, worden alle plaatsen gericht.

>[!NOTE]
>
>De plaatsen van de Stad en DMA zijn niet beschikbaar voor Plaatsen Roku.

Locaties opgeven:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Een land, een staat, een stad, een DMA, een federaal wetsdistrict of een wetsdistrict van een staat op te nemen of uit te sluiten:
      1. Selecteer het locatietype in de linkerkolom.
      1. (Indien nodig) Klik op een locatie om deze uit te vouwen.
      1. Klik naast de locatie op *[!UICONTROL Include]* om deze als doel op te nemen of op *[!UICONTROL Exclude]* om deze als doel uit te sluiten.
   * U kunt als volgt naar een postcode zoeken en alle geselecteerde resultaten opnemen of uitsluiten:
      1. Klik op **[!UICONTROL Search Postal Code]**.
      1. Selecteer het land.
      1. Voer de plaatsnaam in en klik op ![Bewerken](/help/dsp/assets/search.png).
      1. Klik op het juiste zoekresultaat.
      1. Klik *[!UICONTROL Include All]* om alle locaties als doelen op te nemen of *[!UICONTROL Exclude All]* om alle locaties als doelen uit te sluiten.
   * U kunt als volgt postcodes invoeren of plakken en deze allemaal opnemen of uitsluiten:
      1. Klik op **[!UICONTROL Paste Postal Code]**.
      1. Selecteer het land.
      1. Voer maximaal 1000 postcodes in of plak deze.
Neem één postcode per regel op of voer meerdere waarden in, gescheiden door komma&#39;s of tabs.
      1. Klik *[!UICONTROL Include All]* om alle locaties als doelen op te nemen of *[!UICONTROL Exclude All]* om alle locaties als doelen uit te sluiten.
   * Als u een locatie uit de lijst [!UICONTROL Included] of [!UICONTROL Excluded] wilt verwijderen, klikt u op **[!UICONTROL X]** naast de locatie in de rechterkolom.
1. Klik op **[!UICONTROL Done]**.

>[!NOTE]
>
>* Niet alle landen hebben de locatie Staat, de plaats of de postcode.
>* DMA (aangewezen marktgebied), Federal Legislative Districts, en de Wetgevende Districten van de Staat zijn beschikbaar voor de plaatsen van de V.S. slechts.


## [!UICONTROL Inventory Targeting]

**[!UICONTROL Inventory Sources]:** Inventarisbronnen die als doel moeten worden opgenomen of uitgesloten. Voor de meeste plaatsingstypen worden alle voorraadtypen en alle bronnen voor elk type standaard opgenomen. Voor [!DNL Roku] plaatsingen, moet u het inventaristype en de bronnen specificeren. U kunt uit de volgende soorten inventaris kiezen:

* [!UICONTROL Public]: (Alle plaatsingstypen, behalve voor Roku) Alle openwisselingsvoorraden waartoe Advertising Cloud toegang heeft. U kunt openbare voorraad opnemen en uitsluiten.

   U kunt de lijst bekijken door bron of door voer. Wanneer u de lijst weergeeft op basis van feed, kunt u zoeken op naam van de feed, op basis van de feed of op basis van een geselecteerde kenmerkende tag.

* [!UICONTROL Private] |  [!UICONTROL Roku Private]: Uw bestaande persoonlijke deals (of bestaande persoonlijke  [!DNL Roku] deals voor  [!DNL Roku] plaatsingen) met uitgevers die u in DSP hebt ingesteld. U kunt een openbare voorraad opnemen, maar niet uitsluiten.

   U kunt de lijst zoeken op trefwoord, sleutel, deal-id of aangepaste tag.

* [!UICONTROL On Demand] |  [!UICONTROL Roku On Demand]: Alle  [premies, niet-gegarandeerde  [!UICONTROL On Demand] voorraad](/help/dsp/inventory/on-demand-inventory-about.md)  (of  [!UICONTROL On Demand] [!DNL] Roku behandelt  [!DNL Roku] plaatsingen) waarop u zich hebt geabonneerd  [!DNL DSP]. U kunt [!UICONTROL On Demand]-voorraad opnemen en uitsluiten.

   U kunt de lijst bekijken door bron of door voer. Wanneer u de lijst op feed weergeeft, kunt u zoeken op naam van feed, feed-sleutel of een geselecteerd uitgeversgebied, een categorietag of een kenmerkende tag.

Opgeven welke inventarisdoelen worden gebruikt:

* Als u een voorraadtype wilt uitsluiten, schakelt u het selectievakje naast de naam uit.
* Een voorraadtype als doel instellen:
   1. Schakel het selectievakje naast de naam van het voorraadtype in.
   1. (Optioneel) Wijzig de bronnen in:
      1. Klik ![Bewerken](/help/dsp/assets/edit.png).
      1. ([!UICONTROL Public] en [!UICONTROL On Demand] voorraad) Klik *[!UICONTROL *View by Source]** of **[!UICONTROL View by Feed]** om te veranderen hoe de bronnen worden vermeld.
      1. (Indien van toepassing) Filter de voorraad naar wens.
      1. Geef de bronnen op die u wilt opnemen en uitsluiten:
         * Als u een [!UICONTROL Public]- of [!UICONTROL On Demand]-bron wilt opnemen, klikt u op **[!UICONTROL Include]** naast de bronnaam.
         * [!UICONTROL Private]-bronnen opnemen:
            * Om al inventaris in een overeenkomst te omvatten, klik **[!UICONTROL Include all]** naast de overeenkomstennaam.
            * Om een individuele inventarisbron te omvatten, breid de overeenkomstennaam uit, en klik dan het controlevakje naast de bronnaam.
         * Als u een [!UICONTROL Public]- of [!UICONTROL On ]-bron wilt uitsluiten, klikt u op **[!UICONTROL Exclude]** naast de bronnaam.
   1. (Optioneel) Als u een CSV-bestand met de doelgegevens naar de downloadlocatie van uw browser wilt downloaden, klikt u op **[!UICONTROL Save & Export]**.
   1. Klik op **[!UICONTROL Save]**.

>[!TIP]
>
>Als u zich hebt geabonneerd op [!UICONTROL On Demand]-voorraad maar de uitgevers of deals niet kunt vinden die u als doel wilt instellen, controleert u de status van de deals. Zie [Informatie [!DNL On Demand] Premiumvoorraad](/help/dsp/inventory/on-demand-inventory-about.md) voor meer informatie over statussen.

**[!UICONTROL Exclude out-stream]:** (Alleen videoplaatsingen) Sluit het stroomafwaartse verkeer uit.

Outstream-advertenties worden doorgaans als een pop-up of opgevuld in inhoud (in de eigen ervaring) weergegeven in plaats van als gewone videobanden in een videospeler.

## [!UICONTROL Site Targeting]

**[!UICONTROL Traffic type]:** De types van verkeer aan doel. U kunt onder andere **[!UICONTROL Websites]** en **[!UICONTROL Apps]** kiezen.

**[!UICONTROL Site tier]:** (Beschikbaar wanneer  **[!UICONTROL Paste list of targeted sites]** is  *[!UICONTROL Off]*) De kwaliteit van de sites waarop u zich wilt richten. Tiers 1-3 zijn allemaal merkveilig en zijn gecontroleerd en goedgekeurd door het DSP-kaartteam.

* *[!UICONTROL Tier 1]:* Premiumsites en -toepassingen die nationaal herkenbaar zijn.
* *[!UICONTROL Tier 2]:* Streefcijfers voor niveau 1 en kwaliteitsites en toepassingen die minder bekend zijn dan niveau 1.
* *[!UICONTROL Tier 3]:* Doeltips 1-2 en legitieme en brandveilige sites en toepassingen die geschikt zijn voor een nichepubliek. Gebruik Niveau 3 voor bereik of gegevens die op aankopen gericht zijn.
* *[!UICONTROL All Sites]:* Doeltips 1-3 en nieuwe voorraad die niet is gescreend of gecategoriseerd en die u kunt gebruiken voor reach.

>[!NOTE]
>
>Inventaris is specifiek voor de advertentie-eenheden in de plaatsing.

>[!TIP]
>
>Voor prestatiecampagnes, is de beste praktijken *[!UICONTROL All Sites]* te selecteren.

**[!UICONTROL Site Categories]:** (Optioneel; Beschikbaar wanneer  **[!UICONTROL Paste list of targeted sites]** is  *[!UICONTROL Off]*) Sitecategorieën binnen de geselecteerde siteniveaus om (maar niet allebei) als doelen op te nemen of uit te sluiten. Maak een keuze uit verticale sitelijsten die door Advertising Cloud zijn toegewezen op basis van het onderwerp van de site:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sitecategorieën op die u wilt opnemen of uitsluiten:
   * Sitecategorieën opnemen:
      1. Klik op **[!UICONTROL Include categories]**.
      1. Schakel het selectievakje naast elke categorie in die u wilt activeren.
   * Sitecategorieën uitsluiten:
      1. Klik op **[!UICONTROL Exclude categories]**.
      1. Schakel het selectievakje naast elke categorie in die u wilt uitsluiten.
1. (Optioneel) Als u een CSV-bestand met de doelgegevens naar de downloadlocatie van uw browser wilt downloaden, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Exclude Sites]:** (Optioneel; beschikbaar wanneer  **[!UICONTROL Paste list of targeted sites]** is  *[!UICONTROL Off]*) De plaatsen om uit te sluiten. U kunt zoeken naar sites en deze selecteren, of u kunt domeinnamen invoeren of plakken:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sites op:
   * Ga als volgt te werk om een site te zoeken:
      1. Klik op **[!UICONTROL Search]**.
      1. Voer een trefwoord in, selecteer een sitelaag en/of selecteer een sitecategorie.
      1. Selecteer in de zoekresultaten de sites die u wilt uitsluiten:
         * Als u een afzonderlijke site wilt uitsluiten, schakelt u het selectievakje naast de site in.
         * (Als er meer dan 50 resultaten beschikbaar zijn) Als u de eerste 50 resultaten wilt uitsluiten, klikt u op **[!UICONTROL Exclude these 50]**. Om alle onderzoeksresultaten uit te sluiten, klik **[!UICONTROL Exclude these \<*NN *\>]**.
   * Domeinnamen invoeren:
      1. Klik op **[!UICONTROL Paste]**.
      1. Voer een of meer domeinnamen op afzonderlijke regels in.
      1. Klik op **[!UICONTROL Exclude All]**.
1. Klik **[!UICONTROL Done]** wanneer u wordt gebeëindigd.

>[!NOTE]
>
>* Naast de Advertising Cloud DSP [algemeen geblokkeerde sitelijst](/help/dsp/introduction/features/brand-safety-media-quality.md), die sites bevat die onveilig worden geacht voor advertenties, worden ook sitelijsten op accountniveau en op adverteerderniveau toegepast.
>* Lijsten met geblokkeerde sites hebben altijd voorrang op lijsten met doelsites. Als een plaatsing zowel het zelfde doel voor een advertentie uitsluit als omvat, dan wordt het doel uitgesloten.


**[!UICONTROL Language]:** (Optioneel) Eén taal waarop u zich wilt richten.

**[!UICONTROL Site List Preview]:** (Alleen-lezen) Alle beoogde en geblokkeerde sites voor de plaatsing.

U kunt desgewenst de lijst met doelsites en geblokkeerde sites exporteren als een CSV-bestand (comma-separated values, door komma&#39;s gescheiden waarden). Als u de lijst wilt exporteren, klikt u op **[!UICONTROL Export full site list]** en opent of slaat u het bestand op volgens de normale procedure van uw browser.

<!-- **[!UICONTROL Allow unscreened sites]:** (XXX placements only) Allows you to XXXX.   Optional available for https://advertising.adobe.com/configurator/placement/edit/2432022 -->

**[!UICONTROL Paste list of targeted sites]:** Hiermee kunt u alleen specifieke sites als doel instellen. Wanneer u deze optie inschakelt, worden de andere opties voor het instellen van doelen voor de site uitgeschakeld.

**[!UICONTROL Sites]:** (Beschikbaar als  **[!UICONTROL Paste list of targeted sites]** dit  *[!UICONTROL On]* het geval is) De sites waarop u wilt verwijzen. U kunt zoeken naar sites en deze selecteren, of u kunt domeinnamen invoeren of plakken:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de sites op:
   * Ga als volgt te werk om een site te zoeken:
      1. Klik op **[!UICONTROL Search]**.
      1. Voer een trefwoord in, selecteer een sitelaag en/of selecteer een sitecategorie.
      1. Selecteer in de zoekresultaten de sites die u wilt opnemen:
         * Als u een afzonderlijke site wilt uitsluiten, schakelt u het selectievakje naast de site in.
         * (Als er meer dan 50 resultaten beschikbaar zijn) Als u de eerste 50 resultaten wilt opnemen, klikt u op **[!UICONTROL Include these 50]**. Als u alle zoekresultaten wilt opnemen, klikt u op **[!UICONTROL Include these \<*NN *\>]**.
   * Domeinnamen invoeren:
      1. Klik **[!UICONTROL Paste]**.
      1. Voer een of meer domeinnamen op afzonderlijke regels in.
      1. Klik op **[!UICONTROL Include All]**.
1. Klik op **[!UICONTROL Done]**.

## [!UICONTROL Audience Targeting]

**[!UICONTROL Included Audiences]:** Om het even welke publieksdoelstellingen voor de plaatsing, met inbegrip van  [derdesegmenten, eerste-partijsegmenten, de segmenten van de Adobe, douanesegmenten, en bewaarde publiek](/help/dsp/audiences/audience-settings.md). De totale en actieve gededupliceerde publieksgrootte voor alle geselecteerde segmenten en opgeslagen doelgroepen wordt ook weergegeven. U kunt een bestaand publiek selecteren, een nieuw publiek maken dat u later opnieuw kunt gebruiken of specifieke publiekssegmenten selecteren:

* Als u een bestaand publiek wilt selecteren, klikt u op ![Select](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Included Audiences] en selecteert u vervolgens het publiek.
* Als u een nieuw publiek wilt maken, klikt u op ![Select](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Included Audiences] en selecteert u **[!UICONTROL + Create Audience]**. Zie [Een herbruikbaar publiek maken](/help/dsp/audiences/reusable-audience-create.md), te beginnen met stap 3.
* Als u bepaalde publiekssegmenten wilt selecteren, klikt u op **[!UICONTROL Select segments for this placement only]**. Selecteer de segmentlogica. voor instructies, zie Stap 6 in &quot;[Creeer een Herbruikbaar Publiek](/help/dsp/audiences/reusable-audience-create.md).&quot; Wanneer u wordt gedaan, klik **sparen**.

**[!UICONTROL Excluded Audiences]:** Om het even welk publiek om voor de plaatsing uit te sluiten, met inbegrip van publiek met  [derdesegmenten, eerste-partijsegmenten, de segmenten van de Adobe, douanesegmenten, en bewaard publiek](/help/dsp/audiences/audience-settings.md). De totale en actieve gededupliceerde publieksgrootte voor alle uitgesloten doelgroepen wordt ook weergegeven. U kunt een bestaand publiek selecteren of een nieuw publiek maken dat u later opnieuw kunt gebruiken:

* Als u een bestaand publiek wilt selecteren, klikt u op ![Select](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Excluded Audiences] en selecteert u vervolgens het publiek.
* Als u een nieuw publiek wilt maken, klikt u op ![Select](/help/dsp/assets/chevron-down.png) naast [!UICONTROL Excluded Audiences] en selecteert u **+ Audience** maken. Zie [Een herbruikbaar publiek maken](/help/dsp/audiences/reusable-audience-create.md), te beginnen met stap 3.

**[!UICONTROL Cross Device Targeting]:** (Beschikbaar wanneer u minstens één segment of publiek selecteert en de  [campagne wordt gevormd voor op mensen-gebaseerde het dwars-apparaat richten](/help/dsp/campaign-management/campaigns/campaign-settings.md). Staat u toe om uw het richten over alle bekende apparaten van een persoon (per de apparatengrafiek uit te breiden die in de campagnemontages wordt gespecificeerd), zelfs apparaten die niet in de gespecificeerde segmenten zijn. De kosten kunnen van toepassing zijn afhankelijk van de grafiek die voor de campagne wordt gespecificeerd. Apparaatgrafiekgegevens zijn momenteel alleen beschikbaar in Noord-Amerika.

**[!UICONTROL Placement Cap]:** (Optioneel) Het aantal keren dat een uniek apparaat of een unieke persoon (afhankelijk van het opgegeven apparaat of de opgegeven persoon  [!UICONTROL Cross Device Level]) advertenties ontvangt van de plaatsing. U kunt onder andere *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand opgeven.

>[!NOTE]
>
> U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

**[!UICONTROL Secondary Cap]:** (Optioneel; Deze optie is beschikbaar als u een numerieke waarde toevoegt  [!UICONTROL Placement Cap]) Een extra beperking binnen de grenzen van de primaire plaatsingslimiet. Selecteer het aantal afbeeldingen en de tijdsperiode (bijvoorbeeld 3 per 12 uur).

**[!UICONTROL Day Parting]:** (Optioneel) Specifieke dagen van de week en het tijdstip van de dag waarop advertenties kunnen worden uitgevoerd. De zomerintervallen opgeven:
1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Selecteer de toepasselijke tijdzone.
1. Geef de intervallen op:
   * Klik op een van de intervalknoppen om een vooraf ingesteld interval te selecteren. Opties zijn onder andere *[!UICONTROL Weekends]**, *[!UICONTROL Weekdays]*, *[!UICONTROL Morning]*, *[!UICONTROL Lunch]*, *[!UICONTROL Dinner]* of *[!UICONTROL Prime]* (primetime).
   * Als u handmatig een interval wilt selecteren, klikt u in een cel en sleept u optioneel om het interval te selecteren.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Topic Targeting]:** (Optioneel; beschikbaar aan adverteerders die met  [!DNL Comscore] en  [!DNL Grapeshot] segmenten) worden gevormd - specifieke segmentnamen of IDs van  [!DNL Comscore] en  [!DNL Grapeshot] om als doelstellingen te omvatten. Voor deze functie kunnen extra kosten in rekening worden gebracht. Neem contact op met uw accountmanager van Adobe om deze functie te activeren en onderwerpsegmenten in te stellen.

Onderwerpgerichte onderwerpen opgeven:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
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

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Geef de apparaatdetails op die u wilt opnemen en uitsluiten:
   1. Selecteer de categorie in de linkerkolom.
   1. Doelstelling opgeven:
      * Als u een waarde wilt opnemen, klikt u op **[!UICONTROL Include]** naast de naam van de waarde.
      * Als u een waarde wilt uitsluiten, klikt u op **[!UICONTROL Exclude]** naast de naam van de waarde.
1. (Optioneel) Als u een CSV-bestand met de doelgegevens van het apparaat naar de downloadlocatie van uw browser wilt downloaden, klikt u op **[!UICONTROL Export]**.
1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL ISP Targeting]:** (Optioneel) Specifieke internetserviceproviders (ISP&#39;s) moeten deze als doel opnemen of uitsluiten (maar niet beide). Om ISP het richten te specificeren:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
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

**[!UICONTROL Contextual filtering]:** Typen  [!DNL Comscore],  [!DNL DoubleVerify],  [!DNL Integral Ad Science], en toe te passen  [!DNL Peer39] contextuele filters. De standaardinstellingen op adverteerderniveau worden geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een of meer typen voorraadcontext die standaard worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Peer 39]:

   * **Doelsites die:** (Optioneel) Een of meer typen voorraadkenmerken die standaard als doel moeten dienen. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL ComScore]:

   * **Bloksites die:** (Optioneel) Een of meer typen voorraadkenmerken die standaard moeten worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Integral Ad Science]

   * **[!UICONTROL Adult Content]:** (Optioneel) De mate van inhoud voor volwassenen waarvoor advertenties standaard worden geblokkeerd:  *[!UICONTROL Do Not Block]* (de standaardwaarde),  *[!UICONTROL Standard]* of  *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

   * **[!UICONTROL Alcohol Content]:** (Optioneel) De mate van alcoholgehalte waarvoor advertenties standaard worden geblokkeerd:  *[!UICONTROL Do Not Block]* (de standaardwaarde),  *[!UICONTROL Standard]* of  *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Pre-bid fraud blocking]:** Soorten sites die worden geblokkeerd op basis van frauduleus verkeer en verdachte activiteiten gemeten via  [!DNL DoubleVerify],  [!DNL Integral Ad Science]en  [!DNL Peer39]. De standaardinstellingen op adverteerderniveau worden geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** Door gebrek, blokkeert al 100% ongeldig verkeer, met inbegrip van verkeer op benadrukte apparaten, voor nieuwe plaatsen. Er kunnen extra kosten van toepassing zijn.

   * **[!UICONTROL Also block sites with]:** (Optioneel) Een extra mate van fraude en ongeldig verkeer waardoor DSP standaard advertenties blokkeert:   *[!UICONTROL None]* (het gebrek, dat geen extra verkeer blokkeert),  *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*,  *[!UICONTROL >4% Average Fraud/IVT levels]*,  *[!UICONTROL >6% Average Fraud/IVT levels]*,  *[!UICONTROL >10% Average Fraud/IVT levels]*, of  *[!UICONTROL >25% Average Fraud/IVT levels]*. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Peer 39]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een of meer soorten fraude waardoor DSP standaard advertenties blokkeert:  *[!UICONTROL Fraud]* (die alle sites blokkeert met fraude),  *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]* en/of  *[!UICONTROL Fraud: Zero Ads]*. Er kunnen extra kosten van toepassing zijn.

* [!UICONTROL Integral Ad Science]:

   * **[!UICONTROL Block sites that are]:** (Optioneel) Een type verdachte website- of app-activiteit waardoor DSP standaard advertenties blokkeert:  *[!UICONTROL None]* (de standaardwaarde, die geen advertenties blokkeert op basis van verdachte activiteit),  *[!UICONTROL Suspicious Activity - High Risk]*, of  *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Ads.txt filtering]:**

Welk niveau van [Ads.txt](https://iabtechlab.com/ads-txt-about/) pre-bied het filtreren aan gebruik door de lijst van geautoriseerde Digitale Verkopers van elke uitgever te gebruiken. De standaardinstelling op advertentieniveau is geselecteerd voor nieuwe plaatsingen, maar u kunt de instellingen wijzigen:

* *[!UICONTROL Opt out of ads.txt (default)]*: Winkel kopen van alle verkopers.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: Prioriteit geven aan inkoopvoorraad van geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers van een domein.

**[!UICONTROL DoubleVerify Authentic Brand Safety]:** (Advertisers die met de  [!UICONTROL DoubleVerify Authentic Brand Safety] optie worden gevormd) laat toe  [!DNL DoubleVerify Authentic Brand Safety], die impressies na-bod gebruikend de de veiligheidsregels van het douanemerk blokkeert die voor gespecificeerde segmentidentiteitskaart worden gevormd. DSP uw account aan voor gebruik van de segment-id die in de adverteerderinstellingen is opgegeven.

## [!UICONTROL Tracking]

>[!NOTE]
>
>([!DNL Roku] plaatsing) Door [!DNL Roku] goedgekeurde leveranciers voor het volgen van derden omvatten [!DNL Acxiom], [!DNL comScore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], 13/>, [!DNL Placed], [!DNL Polk] en [!DNL Research Now].[!DNL Oracle]

**[!UICONTROL Event Pixels]:** (Optioneel) Pixels voor het bijhouden van gebeurtenissen van derden die standaard worden gekoppeld aan alle nieuwe advertenties in de plaatsing. Gebeurtenispixels opgeven:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Als u een bestaande pixel wilt selecteren, schakelt u het selectievakje in de pixelrij in.
   * Een nieuwe pixel maken:
      1. Klik op **[!UICONTROL Create]**.
      1. Voer de volgende gegevens in:
         * **[!UICONTROL Pixel name]:** De naam van de pixel; de maximumlengte is 500 tekens. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.
         * **[!UICONTROL Pixel event fires on]:** De gebeurtenis die de pixel activeert. De beschikbare gebeurtenissen variëren per advertentietype.
         * **[!UICONTROL Pixel type]:** Geeft aan of de pixel een  *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel),  *[!UICONTROL HTML]* of  *[!UICONTROL JavaScript URL]*.
         * **[!UICONTROL Pixel URL]:** De URL van de pixelafbeelding.
      1. Klik op **[!UICONTROL Create and attach]**.
   1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL Conversion Pixels]:** (Optioneel) Pixels voor het bijhouden van de conversie die standaard worden gekoppeld aan alle nieuwe advertenties in de plaatsing. Omzetpixels opgeven:

1. Klik ![Bewerken](/help/dsp/assets/edit.png).
1. Voer een van de volgende handelingen uit:
   * Als u een bestaande pixel wilt selecteren, schakelt u het selectievakje in de pixelrij in.
   * Een nieuwe pixel maken:
      1. Klik op **[!UICONTROL Create]**.
      1. Voer de volgende gegevens in:
         * **[!UICONTROL Conversion pixel name]:** De naam van de pixel; de maximumlengte is 500 tekens. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.
         * **[!UICONTROL Conversion category]:** Het type conversie.
         * **[!UICONTROL Impression conversion window]:** Het aantal dagen nadat een advertentie voorkomt waarin de indruk aan een omzetting kan worden toegeschreven. De standaardwaarde is 30 dagen.
         * **[!UICONTROL Click conversion window]:** Het aantal dagen nadat een advertentie voorkomt waarin de klik aan een omzetting kan worden toegeschreven. De standaardwaarde is 30 dagen.
         * **[!UICONTROL Notes]:** (Optioneel) Een beschrijving of andere informatie over de pixel.
      1. Klik op **[!UICONTROL Create and attach]**.
      1. Implementeer de conversiepixel op de relevante webpagina&#39;s:
         1. Ga in het hoofdmenu naar **[!UICONTROL Resources]>[!UICONTROL Conversion pixels]**.
         1. Klik in de pixelrij op **[!UICONTROL edit]**.
         1. Kopieer de waarde(n) in de velden [!UICONTROL HTML Tag] en [!UICONTROL Flash Tag], indien nodig, om de adverteerder of de websitecontactpersoon te voorzien.

            De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.
   1. Klik op **[!UICONTROL Save]**.

**[!UICONTROL 3rd-party Fees]:** (Optioneel) Een statisch tarief van een externe vergoeding dat moet worden bijgehouden als een niet-factureerbare kostprijs per duizend impressies. De standaardinstelling op pakketniveau wordt, indien van toepassing, automatisch toegepast op nieuwe plaatsingen, tenzij u een andere waarde opgeeft.

>[!NOTE]
>
>Facultatieve vergoedingen worden weerspiegeld in de [!UICONTROL Net CPM]-norm.

>[!MORELIKETHIS]
>
>* [Info over Plaatsingsbeheer](placement-about.md)
>* [Een plaatsing maken](placement-create.md)
>* [Een plaatsing bewerken](placement-edit.md)
>* [Sneltoetsen](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [Veelgestelde vragen over Campagnebeheer](/help/dsp/campaign-management/campaign-management-faq.md)

