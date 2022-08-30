---
title: Accountinstellingen voor adverteerders
description: Zie beschrijvingen van de beschikbare adverteerderinstellingen.
source-git-commit: d7afcc2200adc41e583d21712226cb25f35aab66
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 0%

---

# Accountinstellingen voor adverteerders

*Niet beschikbaar voor alleen-lezen gebruikers*

## [!UICONTROL General] Instellingen

**[!UICONTROL Advertiser Name]:** De naam van de adverteerder.

**[!UICONTROL Category]:** De categorie waarin het bedrijf van de adverteerder actief is. De rubriek wordt aan de uitgevers meegedeeld wanneer je op voorraad biedt. Kies een categorie die is uitgelijnd op uw advertenties of uitgevers kunnen uw advertenties afwijzen.

>[!NOTE]
>
>Als u *[!UICONTROL Other]*, dan zal de adverteerder geen toegang hebben tot DSP [!DNL On Demand Inventory].

**[!UICONTROL Advertiser URL]:** De homepage of URL van de hoofdwebsite van de adverteerder (begint met `http://` of `https://`).

**[!UICONTROL Share all private exchange feeds into this advertiser]:** (Alleen voor nieuwe adverteerderaccounts) Hiermee stelt u alle privéuitwisselingsfeeds die zijn geconfigureerd voor de DSP van de organisatie ter beschikking van de adverteerder.

### [!UICONTROL Adobe IMS IDs]

Adverteerders met extra Adobe Experience Cloud-producten kunnen gegevens over bepaalde producten delen met behulp van de unieke id van de organisatie voor Experience Cloud. U kunt specifieke productintegratie configureren in de [!UICONTROL Integrations] sectie.

**[!UICONTROL Account IMS org and ID]:** (Adverteerders met extra Experience Cloud-producten die een licentie hebben gekregen via een Experience Cloud-account met meerdere adverteerders; (optioneel) De Experience Cloud-organisatie-id van de adverteerder.

**[!UICONTROL Advertiser IMS org and ID]:** (Adverteerders met rechtstreekse licenties voor extra Experience Cloud-producten; (optioneel) De Experience Cloud-organisatie-id van de adverteerder.

### [!UICONTROL Integrations]

(Optioneel) Aanvullende Experience Cloud-producten gekoppeld aan de DSP account. De producten moeten worden gekoppeld aan dezelfde organisatie-id voor Experience Cloud die in het [!UICONTROL Adobe IMS IDs] sectie.

**[!UICONTROL Attribution services]> [!UICONTROL Adobe Media Optimizer]:** (Adverteerders met Advertising Cloud Search of die Advertising Cloud-conversiepixels gebruiken) A [!DNL Search] account waarmee DSP toewijzingsgegevens zal uitwisselen.

**[!UICONTROL Report suites]> [!UICONTROL Adobe Analytics]:** (Adverteerders bij Adobe Analytics; facultatief; alleen van toepassing op gegevens die zijn verzameld met trackingtags voor Advertising Cloud-conversie die een [!DNL EF Redirect] en alleen token) Een of meer [!DNL Analytics] rapporteereeksen waaraan DSP de gegevens die het bij uitgevers en leveranciers verzamelt, zal verzenden. Analytics zal ook de gegevens verzenden het van de plaats van de cliënt aan DSP verzamelt.

Om de gegevens in de rapportsuites te verschijnen, [!DNL Search] instelling op adverteerderniveau op &quot;[!UICONTROL Enable tracking for SAINT feeds]&quot; moet zijn ingeschakeld. Bovendien [!DNL Analytics] -account moet geconfigureerd zijn om gegevens van Advertising Cloud te ontvangen.

>[!WARNING]
>
>Als u een eerder gekoppelde rapportsuite verwijdert, worden DSP geen gegevens meer uitgewisseld met die suite. Verwacht gegevensschommelingen te zien.

Meer informatie over de integratie met [!DNL Analytics], zie &quot;[Overzicht van [!DNL Analytics for Advertising Cloud]](/help/integrations/analytics/overview.md).&quot;

**[!UICONTROL Audiences]> [!UICONTROL Adobe Analytics Cloud]:** (Adverteerders bij Adobe Audience Manager of Adobe Analytics; (optioneel) Een Audience Manager of [!DNL Analytics] -account waaruit DSP segmentmetagegevens, hiërarchiegegevens en unieke publieksgegevens voor alle Adobe-gebruikers van de adverteerder ophalen. Dit omvat gegevens voor:

* Audience Manager-segmenten
* [!DNL Analytics] segmenten die naar Adobe Experience Cloud worden gepubliceerd
* Segmenten die in Adobe Experience Cloud zijn gemaakt met de opdracht [!DNL People core service]
* Segmenten die in Adobe Experience Platform zijn gemaakt en via Audience Manager naar Advertising Cloud zijn verzonden

De eerste synchronisatie duurt ongeveer 24 uur. Daarna worden gegevens in real-time gesynchroniseerd met een vertraging van 1 tot 2 seconden.
<!-- I don't think this is true anymore:
Segment membership data is sent to Advertising Cloud only after one of the following:

* The segment is targeted in an Advertising Cloud placement or audience library
* The segment is added to the Advertising Cloud batch and real-time destinations within the Audience Manager user interface
-->

## [!UICONTROL Targeting] Instellingen

U kunt naar keuze standaarddoelstellingen voor de nieuwe plaatsen van de adverteerder vormen. Gebruikers kunnen de standaarddoelen voor elke nieuwe plaatsing overschrijven.

### [!UICONTROL Geo-targeting]

**[!UICONTROL Countries]:** Het standaardland voor de geotargeting van elke plaatsing. De gebruikers kunnen het land veranderen, en specifieker geo-gericht vormen, voor elke plaatsing.

### [!UICONTROL Audience Targeting]

**[!UICONTROL Audiences to exclude]:** Willekeurig publiek of segment dat standaard moet worden onderdrukt. Gebruikers kunnen de uitsluitingen voor elke plaatsing wijzigen.

### [!UICONTROL Media Quality]

#### [!UICONTROL Contextual Filtering]

Typen [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39] contextafhankelijke filters die moeten worden toegepast. U kunt de instellingen op adverteerderniveau overschrijven in het dialoogvenster [plaatsingsniveau](/help/dsp/campaign-management/placements/placement-settings.md).

##### [!UICONTROL DoubleVerify] {#doubleverify-context}

**[!UICONTROL Block sites that are]:** (Optioneel) Een of meer typen voorraadcontext die standaard worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

##### [!UICONTROL Peer 39] {#peer39-context}

**[!UICONTROL Target sites that are]:** (Optioneel) Een of meer typen voorraadkenmerken die standaard als doel moeten worden ingesteld. Er kunnen extra kosten van toepassing zijn.

##### [!UICONTROL ComScore]

**[!UICONTROL Block sites that are]:** (Optioneel) Een of meer typen voorraadkenmerken die standaard moeten worden geblokkeerd. Er kunnen extra kosten van toepassing zijn.

##### [!UICONTROL Integral Ad Science] {#ias-context}

**[!UICONTROL Adult Content]:** (Optioneel) De mate van inhoud voor volwassenen waarvoor advertenties standaard worden geblokkeerd: *[!UICONTROL Do Not Block]* (standaard), *[!UICONTROL Standard]*, of *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Alcohol Content]:** (Optioneel) Het alcoholgehalte waarvoor standaard advertenties worden geblokkeerd: *[!UICONTROL Do Not Block]* (standaard), *[!UICONTROL Standard]*, of *[!UICONTROL Strict]*. Er kunnen extra kosten van toepassing zijn.

#### [!UICONTROL Pre-Bid Fraud Blocking]

Soorten sites die moeten worden geblokkeerd op basis van frauduleus verkeer en verdachte activiteiten, gemeten via [!DNL DoubleVerify], [!DNL Integral Ad Science], en [!DNL Peer39]. U kunt de instellingen op adverteerderniveau overschrijven in het dialoogvenster [plaatsingsniveau](/help/dsp/campaign-management/placements/placement-settings.md).

##### [!UICONTROL DoubleVerify] {#doubleverify-fraud}

**[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** Door gebrek, blokkeert al 100% ongeldig verkeer, met inbegrip van verkeer op gekaapte apparaten, voor nieuwe plaatsen. Er kunnen extra kosten van toepassing zijn.

**[!UICONTROL Also block sites with]:** (Optioneel) Een extra niveau van fraude en ongeldig verkeer waardoor DSP standaard advertenties blokkeert:  *[!UICONTROL None]* (het gebrek, dat geen extra verkeer blokkeert), *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*, *[!UICONTROL >4% Average Fraud/IVT levels]*, *[!UICONTROL >6% Average Fraud/IVT levels]*, *[!UICONTROL >10% Average Fraud/IVT levels]*, of *[!UICONTROL >25% Average Fraud/IVT levels]*. Er kunnen extra kosten van toepassing zijn.

##### [!UICONTROL Peer 39] {#peer-39-fraud}

**[!UICONTROL Block sites that are]:** (Optioneel) Een of meer soorten fraude waardoor DSP standaard advertenties blokkeert: *[!UICONTROL Fraud]* (die alle sites blokkeert met fraude), *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]*, en/of *[!UICONTROL Fraud: Zero Ads]*. Er kunnen extra kosten van toepassing zijn.

##### [!UICONTROL Integral Ad Science] {#ias-fraud}

**[!UICONTROL Block sites that are]:** (Optioneel) Een type verdachte website- of app-activiteit waardoor DSP standaard advertenties blokkeert: *[!UICONTROL None]* (de standaardwaarde, die geen advertenties blokkeert op basis van verdachte activiteit), *[!UICONTROL Suspicious Activity - High Risk]*, of *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. Er kunnen extra kosten van toepassing zijn.

#### [!UICONTROL Ads.text]

**[!UICONTROL Ads.txt Filtering]:** Standaard, welk niveau van [[!DNL Ads.txt] filteren vóór bod](https://iabtechlab.com/ads-txt-about/) te gebruiken door gebruik te maken van de [!DNL Authorized Digital Sellers] lijst:
* *[!UICONTROL Opt out of ads.txt (default)]*: Winkel kopen van alle verkopers.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: Prioriteit geven aan inkoopvoorraad van geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers en wederverkopers in een domein.
* *[!UICONTROL Ads.txt sellers only]*: Alleen voorraad kopen bij geautoriseerde directe verkopers van een domein.

U kunt de instelling op adverteerderniveau overschrijven in het dialoogvenster [plaatsingsniveau](/help/dsp/campaign-management/placements/placement-settings.md).

#### [!UICONTROL Safe Site Block]

**[!UICONTROL Enable Site Safety Block]:** Door gebrek, laat een filter in real time, post-bieder toe om ervoor te zorgen dat de advertenties op de plaatsen dienen die de adverteerder richt. <!-- Can remove this: Users can enable or disable the feature for each placement. I don't see this option, but I should probably verify. If this can't be edited at placement level, then remove "By default." If it can, say that you can override at placement level. -->

#### [!UICONTROL DoubleVerify Authentic Brand Safety]

**[!UICONTROL DoubleVerify Account]:** ([!DNL DoubleVerify] alleen klanten; (facultatief) De merkveiligheidssegment-id verbonden aan de organisatie [!DNL DoubleVerify] account.

**[!UICONTROL Enable Authentic Brand Safety]:** (Optioneel) Schakelt standaard [!DNL DoubleVerify] Authentic Brand Safety, die indrukkingen na het bieden blokkeert met behulp van de aangepaste merkveiligheidsregels die voor de opgegeven segment-id zijn geconfigureerd. DSP uw account aan voor gebruik van de segment-id.

U kunt de instelling op advertentieniveau op plaatsingsniveau overschrijven.

>[!MORELIKETHIS]
>
>* [Account voor adverteerders maken](/help/dsp/admin/advertiser-create.md)


<!-- >* [View the Advertiser List for the Account](/help/dsp/admin/advertiser-view.md) -->
