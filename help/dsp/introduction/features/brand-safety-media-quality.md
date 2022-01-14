---
title: Merk, veiligheid en mediakwaliteit
description: Meer informatie over de functies voor merkveiligheid en mediakwaliteit.
feature: DSP Introduction
exl-id: df5be5d4-490e-479f-b76d-4fda4acd4201
source-git-commit: 3bca3d5b4a1ec0bf9bb23946248de350b8bbf2a6
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# Merk, veiligheid en mediakwaliteit

<!-- Check on logo sizes in staging environment -- I made them all 100 pixels high except for DoubleVerify, which is 150 (harder to see at 100), but some instances look larger in VS Code. -->

Advertising Cloud DSP biedt een reeks functies voor merkbescherming om ervoor te zorgen dat elk van uw campagnes echte gebruikers bereikt in een merkveilige omgeving.

Ons team voor toezicht op fraude werkt nauw samen met toonaangevende partners uit de industrie, zoals de [!DNL Interactive Advertising Bureau], [!DNL Trust and Accountability Group] [!DNL (TAG)], en [!DNL WhiteOps]om de inventarisatie op ons platform zorgvuldig te beheren. Door ons aanbod proactief te beheren, zorgt DSP ervoor dat alle adverteerders op het platform beschermd zijn tegen niet-menselijk verkeer (bots, crawlers, datacenterverkeer en fraude) en alleen in merkveilige contexten leveren.

Naast centraal kwaliteitsbeheer geloven we in het vermogen van adverteerders om de controles te ontwerpen die op hun merk zijn afgestemd. Adobe Advertising Cloud biedt integratie met [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], [!DNL Oracle Data Cloud], en [!DNL Peer39], waarbij elke adverteerder zijn gewenste niveau van fraudebescherming, contextafhankelijke filtering en trefwoordgerichtheid kan kiezen.

## Advertising Cloud DSP-kwaliteitsinitiatieven

### Inventariscontrole met [!DNL Ads.txt] Ondersteuning

[[!DNL Ads.txt], die [!DNL Authorized Digital Sellers]](https://iabtechlab.com/ads-txt) is een initiatief van de [!DNL Interactive Advertising Bureau] ([!DNL IAB]) in juni 2017 om de correcte weergave van voorraden op de open markt te vergemakkelijken en aldus illegale bronnen van verkeer en domeinspoofing te bestrijden. Deelnemende uitgevers en distributeurs geven publiekelijk aan welke ondernemingen gemachtigd zijn hun digitale inventaris te verkopen en wat de aard van deze relaties is, door een `ads.txt` pagina op het hoogste niveau van het domein (zoals `example.com/ads.txt`).

DSP [!DNL ads.txt] door elke uitgever te lezen `ads.txt` bestand te kopen en u de optie te geven alleen van geverifieerde [!DNL ads.txt] verkopers. Als je bijvoorbeeld de verkopers afstemt die we zien openen `nytimes.com` aan de New York Times&quot; `ads.txt` -bestand, kunnen we identificeren welke legitiem zijn en welke niet, en we zullen de overtreders blokkeren als de plaatsing is geconfigureerd om alleen van geverifieerde verkopers te kopen. <!-- can we actually mention NY Times? -->

U kunt de standaardinstelling instellen [!DNL ads.txt] besturingselementen voor elke adverteerder<!-- [default ads.txt controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->en vervolgens optioneel [de instellingen voor elke plaatsing aanpassen](/help/dsp/campaign-management/placements/placement-settings.md) tot:

* Alleen door directe verkopers binnen een domein geautoriseerde voorraad kopen

* Alleen bij geautoriseerde directe verkopers en wederverkopers van een domein voorraad kopen

* Prioriteit geven aan inkoopvoorraad van geautoriseerde directe verkopers en wederverkopers van een domein

* Winkelvoorraad kopen van alle verkopers

### Platform Fraude Surveillance

DSP heeft sterke interne hulpmiddelen en systemen gebouwd om fraude over ons platform te beheren, in samenwerking met toonaangevende industrieleveranciers zoals [!DNL Whiteops] en [!DNL Integral Ad Science].

Daarnaast werkt Adobe nauw samen met [!DNL IAB] en [!DNL TAG] om robuuste, industriestandaard fraudeblokkering te garanderen om onze adverteerders te beschermen, met behulp van hulpmiddelen zoals [!DNL ads.txt] (zie de vorige paragraaf), de [!DNL IAB] Bots and Spiders list, en de [!DNL TAG] IP-lijst van datacenter.

Door onze multidimensionale benadering van kwaliteit, controleert ons team anomalieën en ongeldige verkeerspatronen, die minder dan 3% ongeldig verkeer op beschermde inventaris verzekeren. Elke verdachte voorraad — inclusief inventarisatie op specifieke domeinen of van specifieke uitgevers of verkopers — wordt onmiddellijk geblokkeerd op het hele platform.

### Inventaristoewijzing, lagen en categorisering

Het in kaart brengen van de inventaris is het gedetailleerde overzicht en het aan boord nemen proces dat voor alle nieuwe inventaris wordt vereist alvorens het aan ons platform wordt toegevoegd. Dit proces is bedoeld om de veiligheid en de kwaliteit van alle inventarislijsten bij DSP te waarborgen.

* **Toewijzing:** Ons inventarisatieteam evalueert elk domein zorgvuldig en evalueert aspecten zoals:

   * Brand-veiligheid

   * Typecontrole toevoegen

   * Algemene inhoud, dubbele domeinen en nagemaakte advertentie

* **Lagen:** We onderzoeken holistisch de aanwezigheid van merken in het totale ecosysteem om inventarisatie over verschillende niveaus te classificeren. U kunt [uw plaatsing als doel instellen](/help/dsp/campaign-management/placements/placement-settings.md) op deze niveaus voor het gewenste bereik:

   * **[!UICONTROL T1]** - Merknaam, internationaal herkenbare sites

   * **[!UICONTROL T2]** - Uitstekende sites die actueel, up-to-date zijn, geen door gebruikers gegenereerde inhoud bevatten en die gewoonlijk geen wereldwijde herkenning hebben

   * **[!UICONTROL T3]** - Door de gebruiker gegenereerde inhoud en niche-inhoud

* **Indeling van de site:** Om ervoor te zorgen dat inhoud eenvoudig kan worden toegewezen en geblokkeerd, labelen we elke eigenschap met een door Advertising Cloud gedefinieerde sitecategorie op basis van de inhoud van de eigenschap. U kunt [Deze sitecategorieën voor elke plaatsing opgeven of uitsluiten](/help/dsp/campaign-management/placements/placement-settings.md) op basis van de plaatsingsdoelstellingen.

### Uitgebreide ondersteuning voor blokkeren van sites

Advertising Cloud DSP biedt zowel een lijst met wereldwijd geblokkeerde sites als de optie om aangepaste lijsten met geblokkeerde sites voor adverteerders en accounts te maken.

#### Advertising Cloud DSP Global Blocked Sites List {#global-blocked-sites}

Advertising Cloud DSP houdt een wereldwijd geblokkeerde lijst met sites bij die onveilig worden geacht om advertenties uit te voeren. Deze lijst bevat sites met aanstootgevende inhoud (zoals haat of terreur) en sites die besmet zijn met bots, valse pre-roll, niet-afgedekte domeinen en andere frauduleuze activiteiten.

In het kader van ons Brand Safety-initiatief om activiteiten die adverteerders bedriegen uit te roeien, worden alle sites gescreend met behulp van de maatregelen in de lijst met geblokkeerde sites. Alle sites die niet voldoen aan de veiligheidscontroles worden toegevoegd aan de lijst met wereldwijd geblokkeerde sites. Omdat Advertising Cloud DSP deze lijst dynamisch beheert, kunnen sites op elk gewenst moment van de lijst worden verwijderd of in- en uitgeschakeld, op basis van de meest recente analyse van de merkveiligheid.

Wanneer u een site in de lijst met wereldwijd geblokkeerde sites opneemt als plaatsingsdoel, wordt de site gemarkeerd met een rood uitroepteken (!). Dit geeft aan dat advertenties niet worden uitgevoerd op de gemarkeerde site.

#### Geblokkeerde sitelijsten op accountniveau en op advertentieniveau

Gebruikers kunnen ook geblokkeerde sites op accountniveau en op adverteerderniveau bijhouden<!-- [account-level and advertiser-level blocked sites lists](/help/dsp/admin/blocked-sites-list-edit.md) -->, die automatisch voor alle stages worden gebruikt. De lijst met geblokkeerde sites op een lager niveau wordt naast de lijst met wereldwijd geblokkeerde sites toegepast.

## Integraties van derden

### Contextueel filteren

Met contextafhankelijke filters kunt u advertentiemogelijkheden activeren of blokkeren op basis van de context van de pagina waarop de advertentie zou worden geplaatst. Adobe biedt contextafhankelijke filtering via integratie met toonaangevende leveranciers in de branche: [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39]. Voorbeelden van huidige filters zijn [!UICONTROL Adult Content], [!UICONTROL Natural Disasters], [!UICONTROL Legal Drinking Age], [!UICONTROL MANGA], [!UICONTROL Epidemics], en [!UICONTROL G-rated Sites].

U kunt standaardbesturingselementen voor contextafhankelijke filters instellen voor elke adverteerder<!-- [default contextual filter controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->en vervolgens optioneel [de instellingen voor elke plaatsing aanpassen](/help/dsp/campaign-management/placements/placement-settings.md). Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

![Comscore-logo](/help/dsp/assets/comscore-logo.png) ![DoubleVerify-logo](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science-logo](/help/dsp/assets/ias-logo.png) ![Peer39-logo](/help/dsp/assets/peer39-logo.png)

### Blokkeren van voorbiedingsfraude

Profiteer van onze integratie met derden [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39] om niet-menselijk verkeer van uw campagnes te blokkeren. Deze integratie biedt toonaangevende functies voor het blokkeren van voorbiedingen om zowel het algemene als het geavanceerde ongeldige verkeer (GIVT en SIVT) in uw campagnes te minimaliseren.

Je kunt standaard blokkeringscontroles voor vooraf biedingen instellen voor elke adverteerder<!-- [default pre-bid fraud blocking controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->en vervolgens optioneel [de instellingen voor elke plaatsing aanpassen](/help/dsp/campaign-management/placements/placement-settings.md). Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

Neem voor meer informatie over functionaliteit rechtstreeks contact op met de voorkeursleverancier of neem contact op met uw [!DNL Adobe] accountmanager.

![Comscore-logo](/help/dsp/assets/comscore-logo.png) ![DoubleVerify-logo](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science-logo](/help/dsp/assets/ias-logo.png) ![Peer39-logo](/help/dsp/assets/peer39-logo.png)

### Viewability vóór het bod {#pre-bid-viewability}

Weergavefilters voor voorbiedingen van onze toonaangevende partners [!DNL DoubleVerify], [!DNL Oracle Advertising] ([!DNL Moat]), en [!DNL Integral Ad Science] adverteerders in staat stellen ervoor te zorgen dat hun campagnes hun gewenste prestatiedoelen voor de weergave van video en display bereiken.

U kunt standaardweergavefilters instellen voor elke adverteerder<!-- [default pre-viewability filters for each advertiser](/help/dsp/admin/advertiser-settings.md) -->en vervolgens optioneel [de instellingen voor elke plaatsing aanpassen](/help/dsp/campaign-management/placements/placement-settings.md). Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

![DoubleVerify-logo](/help/dsp/assets/doubleverify-logo.png) ![Reclamelogo oracle](/help/dsp/assets/oracle-advertising-logo.png) ![Integral Ad Science-logo](/help/dsp/assets/ias-logo.png)

### Doel van onderwerp

DSP onderwerp het richten staat u toe om sleutelwoordlijsten te richten of te blokkeren door onze industrie-leidende contextafhankelijke partners te leveranteren [!DNL Comscore] en [!DNL Oracle Data Cloud] ([!DNL Grapeshot]). Met onderwerpgerichte toepassingen kunt u ervoor zorgen dat uw advertenties altijd worden aangeboden in een omgeving die op uw merk is afgestemd. Dit geldt zowel voor het blokkeren van schadelijke inhoud als voor het veiligstellen van uitgaven in een context die een groter resultaat biedt.

Het richten van het onderwerp vereist u om de segmenten van het douaneonderwerp direct tot stand te brengen met [!DNL Comscore] of [!DNL Grapeshot] (gebruiken [!DNL Oracle Data Cloud]). Zodra deze in het partnerplatform worden gecreeerd, kunt u [doel of sluit een segmentID in uit [!UICONTROL Audience Targeting] sectie voor elke plaatsing](/help/dsp/campaign-management/placements/placement-settings.md). Voor deze functie kunnen extra kosten in rekening worden gebracht.

Aangepaste onderwerpsegmenten maken:

* Als u een [!DNL Comscore] account en maak aangepaste segmenten, kunt u een aanmeldingsnaam aanvragen voor [!DNL Activation Segment Manager] om [https://agents.comscore.com](https://agents.comscore.com). Zie de [[!DNL Comscore] helpcentrum](https://comscoreactivation.zendesk.com/hc/) voor volledige instructies voor het instellen van aangepaste segmenten. De kosten voor aangepaste segmenten zijn zichtbaar in [!DNL Segment Manager] als u ze maakt.

* Aan de slag met [!DNL Oracle Data Cloud], contact [!DNL Oracle Data Cloud] of uw [!DNL Adobe] accountmanager.

![Comscore-logo](/help/dsp/assets/comscore-logo.png) ![Grapeshot-logo](/help/dsp/assets/oracle-grapeshot-logo.png)

### [!DNL DoubleVerify Authentic Brand Safety]

DSP heeft samengewerkt met [!DNL DoubleVerify] haar [!DNL Authentic Brand Safety] gericht oplossing, die u toestaat om een gecentraliseerde reeks vereisten van de merkveiligheid tot stand te brengen om zich op al uw aankoopplatforms voor consistentie te richten.

Als u eenmaal een [!DNL DoubleVerify] met de vereiste focus, kunt u het segment binnen DSP gebruiken om de regels voor blokken na het bieden te repliceren met een voorbod in een webomgeving.

U kunt een [!DNL DoubleVerify] segment-id voor elke adverteerder<!-- [specify a DoubleVerify segment ID for each advertiser](/help/dsp/admin/advertiser-settings.md) -->en vervolgens optioneel [in- of uitschakelen [!UICONTROL Authentic Brand Safety] voor elke plaatsing](/help/dsp/campaign-management/placements/placement-settings.md). DSP uw account aan voor gebruik van de segment-id.

Voor meer informatie over functionaliteit, contacteer [!DNL DoubleVerify] rechtstreeks, of neem contact op met uw [!DNL Adobe] accountmanager.

![DoubleVerify-logo](/help/dsp/assets/doubleverify-logo.png)

>[!MORELIKETHIS]
>
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

<!-- >* [Advertiser Account Settings](/help/dsp/admin/advertiser-settings.md) -->
