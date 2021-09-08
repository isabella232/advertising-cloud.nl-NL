---
title: Merk, veiligheid en mediakwaliteit
description: Meer informatie over de functies voor merkveiligheid en mediakwaliteit.
feature: Introduction
exl-id: df5be5d4-490e-479f-b76d-4fda4acd4201
source-git-commit: e2ee41c7e3e195f062ad1cc67080ed913d6d3d06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Merk, veiligheid en mediakwaliteit

<!-- Check on logo sizes in staging environment -- I made them all 100 pixels high except for DoubleVerify, which is 150 (harder to see at 100), but some instances look larger in VS Code. -->

Advertising Cloud DSP biedt een reeks functies voor merkbescherming om ervoor te zorgen dat elk van uw campagnes echte gebruikers bereikt in een merkveilige omgeving.

Ons team voor fraudebewaking werkt nauw samen met toonaangevende partners in de branche, zoals [!DNL Interactive Advertising Bureau], [!DNL Trust and Accountability Group] [!DNL (TAG)] en [!DNL WhiteOps], om de inventaris op ons platform zorgvuldig te beheren. Door ons aanbod proactief te beheren, zorgt DSP ervoor dat alle adverteerders op het platform beschermd zijn tegen niet-menselijk verkeer (bots, crawlers, datacenterverkeer en fraude) en alleen in merkveilige contexten leveren.

Naast centraal kwaliteitsbeheer geloven wij in het vermogen van adverteerders om de controles te ontwerpen die op hun merk zijn afgestemd. Adobe Advertising Cloud biedt integratie met [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], [!DNL Oracle Data Cloud], en [!DNL Peer39], die ervoor zorgen dat elke adverteerder zijn gewenste niveau van fraudebescherming, contextafhankelijke filtratie, en sleutelwoordrichten kan kiezen.

## Advertising Cloud DSP-kwaliteitsinitiatieven

### Inventarisverificatie met ondersteuning [!DNL Ads.txt]

[[!DNL Ads.txt], which stands for [!DNL Authorized Digital Sellers]](https://iabtechlab.com/ads-txt) is een initiatief dat in juni 2017 door de  [!DNL Interactive Advertising Bureau] ([!DNL IAB]) is gelanceerd om de correcte weergave van voorraden op de open markt te vergemakkelijken en aldus onrechtmatige bronnen van verkeers- en domeinspoofing te bestrijden. Deelnemende uitgevers en distributeurs geven publiekelijk aan welke bedrijven toestemming hebben om hun digitale inventaris en de aard van die relaties te verkopen, door een `ads.txt`-pagina op het hoogste niveau van het domein te houden (bijvoorbeeld `example.com/ads.txt`).

DSP ondersteunt [!DNL ads.txt] door het `ads.txt`-bestand van elke uitgever te lezen en u de optie te geven om alleen van geverifieerde [!DNL ads.txt]-verkopers aan te schaffen. Door bijvoorbeeld de verkopers te vergelijken die we zien benaderen `nytimes.com` tot het bestand `ads.txt` van de New York Times, kunnen we vaststellen welke wettig zijn en welke niet, en we zullen de overtreders blokkeren als de plaatsing is geconfigureerd om alleen van geverifieerde verkopers te kopen. <!-- can we actually mention NY Times? -->

U kunt standaard [!DNL ads.txt] controles voor elke adverteerder <!-- [default ads.txt controls for each advertiser](/help/dsp/admin/advertiser-settings.md) --> plaatsen, en dan optioneel [aanpassen de montages voor elke plaatsing](/help/dsp/campaign-management/placements/placement-settings.md) aan:

* Alleen door directe verkopers binnen een domein geautoriseerde voorraad kopen

* Alleen bij geautoriseerde directe verkopers en wederverkopers van een domein voorraad kopen

* Prioriteit geven aan inkoopvoorraad van geautoriseerde directe verkopers en wederverkopers van een domein

* Winkelvoorraad kopen van alle verkopers

### Platform Fraude Surveillance

DSP heeft sterke interne hulpmiddelen en systemen gebouwd om fraude over ons platform te beheren, in samenwerking met toonaangevende industrieleveranciers zoals [!DNL Whiteops] en [!DNL Integral Ad Science].

Bovendien werkt Adobe nauw samen met [!DNL IAB] en [!DNL TAG] om robuuste, industriestandaard fraudeblokkering te verzekeren om onze adverteerders te beschermen, die hulpmiddelen zoals [!DNL ads.txt] (zie de vorige sectie) gebruiken, [!DNL IAB] Bots and Spiders lijst, en [!DNL TAG] Datacenter IP lijst.

Door onze multidimensionale benadering van kwaliteit, controleert ons team anomalieën en ongeldige verkeerspatronen, die minder dan 3% ongeldig verkeer op beschermde inventaris verzekeren. Elke verdachte voorraad — inclusief inventarisatie op specifieke domeinen of van specifieke uitgevers of verkopers — wordt onmiddellijk geblokkeerd op het hele platform.

### Inventaristoewijzing, lagen en categorisering

Het in kaart brengen van de inventaris is het gedetailleerde overzicht en het aan boord nemen proces dat voor alle nieuwe inventaris wordt vereist alvorens het aan ons platform wordt toegevoegd. Dit proces is bedoeld om de veiligheid en de kwaliteit van alle inventarislijsten bij DSP te waarborgen.

* **Toewijzing:** Ons inventarisatieteam evalueert elk domein zorgvuldig, waarbij aspecten zoals:

   * Brand-veiligheid

   * Typecontrole toevoegen

   * Algemene inhoud, dubbele domeinen en nagemaakte advertentie

* **Tiering:** We onderzoeken holistisch de aanwezigheid van merken in het ecosysteem als geheel om inventarisatie over verschillende niveaus te classificeren. U kunt [uw plaatsen ](/help/dsp/campaign-management/placements/placement-settings.md) aan deze lagen voor het gewenste niveau van bereik richten:

   * **[!UICONTROL T1]** - Merknaam, internationaal herkenbare sites

   * **[!UICONTROL T2]** - Uitstekende sites die actueel, up-to-date zijn, geen door gebruikers gegenereerde inhoud bevatten en die gewoonlijk geen wereldwijde herkenning hebben

   * **[!UICONTROL T3]** - Door de gebruiker gegenereerde inhoud en niche-inhoud

* **Sitecategorisering:** Om ervoor te zorgen dat inhoud eenvoudig wordt toegewezen en geblokkeerd, labelen we elke eigenschap met een door Advertising Cloud gedefinieerde sitecategorie op basis van de inhoud van de eigenschap. U kunt [deze sitecategorieën voor elke plaatsing ](/help/dsp/campaign-management/placements/placement-settings.md) richten of uitsluiten die op de plaatsingsdoelstellingen wordt gebaseerd.

### Uitgebreide ondersteuning voor blokkeren van sites

Advertising Cloud DSP biedt zowel een lijst met wereldwijd geblokkeerde sites als de optie om aangepaste lijsten met geblokkeerde sites voor adverteerders en accounts te maken.

#### Advertising Cloud DSP Global Blocked Sites List

Advertising Cloud DSP houdt een wereldwijd geblokkeerde lijst met sites bij die onveilig worden geacht om advertenties uit te voeren. Deze lijst bevat sites met aanstootgevende inhoud (zoals haat of terreur) en sites die besmet zijn met bots, valse pre-roll, niet-afgedekte domeinen en andere frauduleuze activiteiten.

In het kader van ons Brand Safety-initiatief om activiteiten die adverteerders bedriegen uit te roeien, worden alle sites gescreend met behulp van de maatregelen in de lijst met geblokkeerde sites. Alle sites die niet voldoen aan de veiligheidscontroles worden toegevoegd aan de lijst met wereldwijd geblokkeerde sites. Omdat Advertising Cloud DSP deze lijst dynamisch beheert, kunnen sites op elk gewenst moment van de lijst worden verwijderd of in- en uitgeschakeld, op basis van de meest recente analyse van de merkveiligheid.

Wanneer u een site in de lijst met wereldwijd geblokkeerde sites opneemt als plaatsingsdoel, wordt de site gemarkeerd met een rood uitroepteken (!). Dit geeft aan dat advertenties niet worden uitgevoerd op de gemarkeerde site.

#### Geblokkeerde sitelijsten op accountniveau en op advertentieniveau

Gebruikers kunnen ook op accountniveau geblokkeerde sites en lijsten met websites op adverteerderniveau bijhouden<!-- [account-level and advertiser-level blocked sites lists](/help/dsp/admin/blocked-sites-list-edit.md) -->, die automatisch voor alle plaatsingen worden gebruikt. De lijst met geblokkeerde sites op een lager niveau wordt naast de lijst met wereldwijd geblokkeerde sites toegepast.

## Integraties van derden

### Contextueel filteren

Met contextafhankelijke filters kunt u advertentiemogelijkheden activeren of blokkeren op basis van de context van de pagina waarop de advertentie zou worden geplaatst. Adobe biedt contextafhankelijke filtering via integratie met toonaangevende leveranciers in de branche: [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science] en [!DNL Peer39]. Voorbeelden van huidige filters zijn [!UICONTROL Adult Content], [!UICONTROL Natural Disasters], [!UICONTROL Legal Drinking Age], [!UICONTROL MANGA], [!UICONTROL Epidemics] en [!UICONTROL G-rated Sites].

U kunt standaardcontextafhankelijke filterbesturingselementen instellen voor elke adverteerder<!-- [default contextual filter controls for each advertiser](/help/dsp/admin/advertiser-settings.md) --> en desgewenst [de instellingen voor elke plaatsing aanpassen](/help/dsp/campaign-management/placements/placement-settings.md). Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

![Comscore-](/help/dsp/assets/comscore-logo.png) ![logoDoubleVerify-](/help/dsp/assets/doubleverify-logo.png) ![logoIntegral Ad Science-](/help/dsp/assets/ias-logo.png) ![logoPeer39-logo](/help/dsp/assets/peer39-logo.png)

### Blokkeren van voorbiedingsfraude

Gebruik onze integratie van derden met [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39] om niet-menselijk verkeer van uw campagnes te blokkeren. Deze integratie biedt toonaangevende functies voor het blokkeren van voorbiedingen om zowel het algemene als het geavanceerde ongeldige verkeer (GIVT en SIVT) in uw campagnes te minimaliseren.

U kunt standaardbesturingselementen instellen voor het blokkeren van fraude met voorbiedingen voor elke adverteerder. <!-- [default pre-bid fraud blocking controls for each advertiser](/help/dsp/admin/advertiser-settings.md) --> Vervolgens kunt u desgewenst [de instellingen voor elke plaatsing aanpassen. ](/help/dsp/campaign-management/placements/placement-settings.md) Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

Neem voor meer informatie over functionaliteit rechtstreeks contact op met de voorkeursleverancier of neem contact op met de Adobe-accountmanager.

![Comscore-](/help/dsp/assets/comscore-logo.png) ![logoDoubleVerify-](/help/dsp/assets/doubleverify-logo.png) ![logoIntegral Ad Science-](/help/dsp/assets/ias-logo.png) ![logoPeer39-logo](/help/dsp/assets/peer39-logo.png)

### Viewability vóór het bod {#pre-bid-viewability}

Met weergavefilters voor vooraf biedende weergave, aangedreven door onze toonaangevende partners [!DNL DoubleVerify], [!DNL Oracle Advertising] ([!DNL Moat]) en [!DNL Integral Ad Science], kunnen adverteerders ervoor zorgen dat hun campagnes in de video- en weergaveinventarisatie aan hun gewenste prestatiedoelen voldoen.

U kunt standaardviewability filters voor elke adverteerder <!-- [default pre-viewability filters for each advertiser](/help/dsp/admin/advertiser-settings.md) --> plaatsen, en dan optioneel [aanpassen de montages voor elke plaatsing](/help/dsp/campaign-management/placements/placement-settings.md). Er kunnen extra kosten van toepassing zijn wanneer u deze functie gebruikt.

![DoubleVerify-](/help/dsp/assets/doubleverify-logo.png) ![logoOracle Advertising-](/help/dsp/assets/oracle-advertising-logo.png) ![logoIntegral Ad Science-logo](/help/dsp/assets/ias-logo.png)

### Doel van onderwerp

DSP onderwerp het richten staat u toe om sleutelwoordlijsten te richten of te blokkeren door onze industrie-leidende contextuele partners [!DNL Comscore] en [!DNL Oracle Data Cloud] ([!DNL Grapeshot]) te gebruiken.

Met onderwerpgerichte toepassingen kunt u ervoor zorgen dat uw advertenties altijd worden aangeboden in een omgeving die op uw merk is afgestemd. Dit geldt zowel voor het blokkeren van schadelijke inhoud als voor het veiligstellen van uitgaven in een context die een groter resultaat biedt.

Voor het toewijzen van onderwerpen moet u onderwerpsegmenten rechtstreeks maken met [!DNL Comscore] of [!DNL Grapeshot] (met [!DNL Oracle Data Cloud]). Zodra deze in het partnerplatform worden gecreeerd, kunt u [een segmentidentiteitskaart in [!UICONTROL  Audience Targeting] sectie voor elke plaatsing ](/help/dsp/campaign-management/placements/placement-settings.md) richten of uitsluiten. Voor deze functie kunnen extra kosten in rekening worden gebracht.

Neem contact op met de leverancier van uw voorkeur of met uw Adobe-accountmanager om aan de slag te gaan.

![Comscore-](/help/dsp/assets/comscore-logo.png) ![logoGrapeshot-logo](/help/dsp/assets/oracle-grapeshot-logo.png)

### [!DNL DoubleVerify Authentic Brand Safety]

DSP heeft met [!DNL DoubleVerify] samengewerkt om zijn [!DNL Authentic Brand Safety] richtende oplossing aan te bieden, die u toestaat om een gecentraliseerde reeks van merkveiligheidseisen tot stand te brengen om zich op al uw koopplatforms voor consistentie te richten.

Als u eenmaal een [!DNL DoubleVerify]-merkveiligheidssegment hebt gemaakt met de vereiste focus, kunt u dit binnen DSP gebruiken om de regels voor blokregels na het bieden te repliceren met pre-bid voor webomgevingen.

U kunt een [!DNL DoubleVerify] segment ID voor elke adverteerder <!-- [specify a DoubleVerify segment ID for each advertiser](/help/dsp/admin/advertiser-settings.md) --> specificeren, en dan optioneel [laat of onbruikbaar maakt [!UICONTROL Authentic Brand Safety] voor elke plaatsing ](/help/dsp/campaign-management/placements/placement-settings.md) toe. DSP uw account aan voor gebruik van de segment-id.

Neem voor meer informatie over functionaliteit rechtstreeks contact op met [!DNL DoubleVerify] of neem contact op met uw Adobe-accountmanager.

![DoubleVerify-logo](/help/dsp/assets/doubleverify-logo.png)

>[!MORELIKETHIS]
>
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

<!-- >* [Advertiser Account Settings](/help/dsp/admin/advertiser-settings.md) -->
