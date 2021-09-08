---
title: Instellingen voor pre-roll-advertentie
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor pre-roladvertenties.
feature: Ads
exl-id: 638d5a3d-3dff-40b6-a3ba-7ab3f08282b9
source-git-commit: e2ee41c7e3e195f062ad1cc67080ed913d6d3d06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Instellingen voor pre-roll-advertentie

## [!UICONTROL Upload or Select Creative]

*Alleen nieuwe advertenties*

**[!UICONTROL Transcode to]:** (Sommige gebruikers, afhankelijk van toestemmingen; (optioneel) De indelingen die u in de VAST-tag wilt opnemen wanneer de uitgever specifieke vereisten voor creatieve bestanden heeft. De indelingen die door de meeste uitgevers worden geaccepteerd, zijn standaard geselecteerd.

**[!UICONTROL Custom Transcode]:** (Alleen bètagebruikers; niet beschikbaar wanneer Verticale video is geselecteerd) Hiermee wordt aangegeven dat de video aangepaste transcode gebruikt. Als u deze optie selecteert, geeft u de bestandsindeling, videobitsnelheid, zoom en afmetingen op voor maximaal drie aangepaste transcodeversies.

**[!UICONTROL XTrader]:** (Sommige gebruikers, afhankelijk van toestemmingen) wijzen erop dat de video één of meerdere  [!DNL X_TRADER] voer gebruikt.

**[!UICONTROL Upload Video]:** Een Raw-element uploaden naar DSP. Voer de volgende handelingen uit wanneer u dit selecteert:

1. Klik op **[!UICONTROL Choose File]** en zoek het bestand op uw apparaat of netwerk.
1. Voer een titel in voor het bestand. Deze titel wordt gebruikt in de weergave [!UICONTROL Ads] en rapporten.
1. Klik op **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Video]:** Om eerder geüploade creatieve bestanden in de juiste indeling in de account te selecteren.

**[!UICONTROL Advanced: VAST Tag URL]:** (Sommige soorten advertenties) Als u een VAST-tag van derden wilt invoeren die creatieve elementen en pixels voor het bijhouden van objecten bevat:

1. Klik ![pijl](/help/dsp/assets/compressed.png) naast **[!UICONTROL Advanced: VAST Tag URL]**.
1. Voer in het veld **[!UICONTROL URL]** de URL van de VAST-tag in.
1. Voer een **[!UICONTROL Title]** voor het bestand in, dat wordt gebruikt in de weergave [!UICONTROL Ads] en rapporten.

>[!TIP]
>
> Als u de geldigheid van een VAST-tag wilt controleren, plakt u deze in een browser en drukt u op **[!UICONTROL Enter]**. Als de tag geldig is, ziet u bovenaan een XML-bestand met `<VAST>`.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de [!UICONTROL Ads] mening, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 30 sec Preroll&quot;).

**[!UICONTROL Width]|  [!UICONTROL Ad Unit Width]:** (Standaard en Alleen voorroladvertenties die kunnen worden overgeslagen) De breedte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

**[!UICONTROL Height]|  [!UICONTROL Ad Unit Height]:** (Standaard en Alleen voorroladvertenties die kunnen worden overgeslagen) De hoogte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

**[!UICONTROL Player X]:** De X-coördinaat voor de advertentie-eenheid. De standaardinstelling behouden.

**[!UICONTROL Player Y]:** De Y-coördinaat voor de advertentie-eenheid. De standaardinstelling behouden.

**[!UICONTROL Player Width]:** De breedte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

Dit is hetzelfde als het veld **[!UICONTROL Width]**.

**[!UICONTROL Player Height]:** De hoogte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

Dit is hetzelfde als het veld **[!UICONTROL Height]**.

**[!UICONTROL Show Controls]:** Waar moeten de videoknoppen voor de advertentie worden opgenomen?  *[!UICONTROL Under]*,  *[!UICONTROL Over]*,  *[!UICONTROL Bottom]* of  *[!UICONTROL None]* (de standaardwaarde).

**[!UICONTROL Preserve Aspect Ratio]:** Of u de breedte- en hoogteverhouding van de video wilt behouden (*[!UICONTROL Yes]*) of dat u de video wilt uitrekken om de beschikbare ruimte (*[!UICONTROL No]*) te vullen.

**[!UICONTROL Click URL]:** (alleen voor advertenties met Adobe-bediening) De URL waarop de viewer landt wanneer deze op de advertentie klikt.

**[!UICONTROL Final Click URL]:** (alleen door Adobe bediende advertenties; alleen-lezen) De  [!UICONTROL Click URL] met de benodigde  [Advertising Cloud DSP tracking-](/help/dsp/campaign-management/macros.md) macrosinserted, indien van toepassing.

**[!UICONTROL VAST Tag]:** (alleen met VAST-tags toevoegen; alleen-lezen) De VAST-tag van derden die u hebt ingevoerd als advertentiebron.

**[!UICONTROL Final VAST Tag]:** (alleen met VAST-tags toevoegen; (alleen-lezen) De VAST-tag van derden die u hebt ingevoerd als advertentiebron met de benodigde  [Advertising Cloud DSP-](/help/dsp/campaign-management/macros.md) trackingmacro&#39;s, indien van toepassing.

**[!UICONTROL Wmode]:** (Alleen interactief vooraf bladeren) De venstermodus:  *[!UICONTROL window]*,  *[!UICONTROL transparent]* of  *[!UICONTROL opaque]*.

**[!UICONTROL Video Format]:** (Alleen interactief pre-roll) De indeling van de advertentiespeler voor mogelijke inventarisatie:  *[!UICONTROL VPAID]* of  *[!UICONTROL VPAID & VAST]*. De weergavebaarheid wordt altijd gemeten voor VPAID, maar VPAID en VAST bevatten een voorraad die geen meting van de weergavemogelijkheid toestaat. Houd dit in mening als de viewability metriek voor uw campagne belangrijk zijn.

**[!UICONTROL Clock Number]**: (alleen interactief vóór de rol; uitsluitend in het Verenigd Koninkrijk worden gebruikt; (alleen beschikbaar voor gebruikers met toestemming) Een unieke id die wordt gebruikt om ervoor te zorgen dat de juiste advertentie wordt uitgezonden. Laat deze instelling leeg als deze niet van toepassing is.

### [!UICONTROL Companion]

*Alleen DSP advertenties*

U kunt desgewenst maximaal drie bijbehorende banners aan een advertentie koppelen. De beste manier is om daar waar mogelijk gezelschapsbanners aan te sluiten.

>[!NOTE]
>
> Niet alle uitgevers staan gezelschapsbanners toe. De uitgevers die gezelschapsbanners wel toestaan, garanderen geen beletsel voor gezelschapsbanners.
> Companion banners van externe advertentietags zijn mogelijk niet altijd beschikbaar voor voorvertoning.

**\[Selectievakje\]:** Bevat de opgegeven bijbehorende banner bij de advertentie. Als het selectievakje is uitgeschakeld, wordt de bijbehorende banner niet opgenomen.

**\[Bannergrootte\]:** de grootte van de bijbehorende banner:  *[!UICONTROL 300x600 (Skyscraper)]*;  *[!UICONTROL 300x250 (Medium Rectangle)]*, de meest gebruikelijke advertentiegrootte en aanbevolen voor alle advertenties;  *[!UICONTROL 300x60 (Small Banner)]*; of  *[!UICONTROL 728x90 (Leaderboard)]*, wat een minder gebruikelijke advertentiegrootte is.

**\[Bron\]:** Of u uw eigen metgezelbannerelement uploadt of een tag van derden gebruikt.

**Element:** (alleen Raw-elementen) Het bijbehorende bannerelement. Klik **[!UICONTROL Browse]** en bepaal de plaats van het dossier op uw apparaat of netwerk, en klik dan **[!UICONTROL Upload]**.

**Add-tag]:[!UICONTROL ** (alleen bij het gebruik van VAST-tags) Een URL naar een bannerbron van een externe partner.

**[!UICONTROL Final Ad Tag]:** (Alleen VAST-tags gebruiken) Een URL naar een bannerbronbron van een externe partner met de benodigde  [Advertising Cloud DSP-](/help/dsp/campaign-management/macros.md) trackingmacro&#39;s, indien van toepassing.

### [!UICONTROL Overlays]

*Interactieve pre-roll en mobiele interactieve en kraan-aan-speel formaten voor DSP-gediende advertenties*

De volgende instellingen zijn van toepassing op elke overlay die u maakt of bewerkt.

**[!UICONTROL Asset]:** (Alleen Raw-elementen) Het bedekkende afbeeldingselement. Het bestand moet de GIF-, JPG- of PNG-indeling voor één frame hebben en de maximale afbeeldingsgrootte moet kleiner zijn dan 2 MB. Als u het element wilt uploaden, klikt u op **[!UICONTROL Browse]** en zoekt u het bestand op uw apparaat of netwerk. Klik vervolgens op **[!UICONTROL Upload]**.

>[!TIP]
>
>Zie [Aanbevolen werkwijzen voor het ontwerpen van overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)

**[!UICONTROL Click URL]:**  De URL waarop de viewer landt wanneer deze op een overlay voor uw advertentie klikt.

**[!UICONTROL X]:** De X-coördinaat voor de bedekking. Selecteer de beginpositie van de bedekking en voer het aantal pixels in vanaf de beginpositie (bijvoorbeeld 10 px van midden). De beste manier is om *Van Midden* te gebruiken, die de bekleding verhindert zich rond met verschillende spelergrootte op uitgeversplaatsen te bewegen.

**[!UICONTROL Y]:** De Y-coördinaat voor de overlay. Selecteer de beginpositie van de bedekking en voer het aantal pixels in vanaf de beginpositie (bijvoorbeeld 10 px van boven). De beste manier is om een coördinaat *[!UICONTROL From Bottom]* of *[!UICONTROL From Top],* op te geven, afhankelijk van de positie waarin u de overlay op de advertentie wilt weergeven.

**[!UICONTROL Layer]:** De laag waarin de bedekking wordt weergegeven. De video en elke overlay bevinden zich in afzonderlijke lagen.

* *[!UICONTROL 2 through 5]:* Voor de video maar achter andere overlays.

* *[!UICONTROL 1]:* Voor de video.

* *[!UICONTROL 0]:* In dezelfde laag als de video. De video wordt kleiner om de resterende ruimte te vullen. Niet aanbevolen voor Interactive Preroll.

* *[!UICONTROL -1]:* Achter de video.

* *[!UICONTROL -2 through -5]:* Achter de video, maar vóór andere overlays.

* *[!UICONTROL Background]:* Achter de video en andere overlays. De bedekking wordt geschaald naar de volledige breedte en hoogte van de video en de hoogte-breedteverhouding blijft niet behouden.

### [!UICONTROL Pixel]

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels desgewenst loskoppelen en nieuwe pixels maken op basis van uw behoeften voor bijhouden.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op *[!UICONTROL Impression]* of *[!UICONTROL Click-through]* worden geactiveerd.

**[!UICONTROL Pixel Type]:** Geeft aan of de pixel een  *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel),  *[!UICONTROL HTML]* of  *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor de opgegeven afbeelding  [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** De naam van de pixel. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider:  *[!UICONTROL None]*,  *[!UICONTROL Nielsen]* of  *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Een advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)
>* [Aanbevolen procedures voor het ontwerpen van overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)

