---
title: Instellingen voor aangesloten tv-advertentie
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor aangesloten tv-advertenties.
feature: Ads
exl-id: 4daae9e4-27eb-4496-9186-f33aebd8daae
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Instellingen voor aangesloten tv-advertentie

## [!UICONTROL Upload or Select Creative]

*Alleen nieuwe advertenties*

**[!UICONTROL Upload Audio]:** Een Raw-element uploaden naar DSP. Voer de volgende handelingen uit wanneer u dit selecteert:

1. Klik op **[!UICONTROL Choose File]** en zoek het bestand op uw apparaat of netwerk.
1. Voer een titel in voor het bestand. Deze titel wordt gebruikt in de weergave [!UICONTROL Ads] en rapporten.
1. Klik op **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Audio]:** Om eerder geüploade creatieve bestanden in de juiste indeling in de account te selecteren.

**[!UICONTROL Advanced: VAST Tag URL]:** (Sommige soorten advertenties) Als u een VAST-tag van derden wilt invoeren die creatieve elementen en pixels voor het bijhouden van objecten bevat:

1. Klik ![pijl](/help/dsp/assets/compressed.png) naast **[!UICONTROL Advanced: VAST Tag URL]**.
1. Voer in het veld **[!UICONTROL URL]** de URL van de VAST-tag in.
1. Voer een **[!UICONTROL Title]** in voor het bestand. Dit wordt gebruikt in de weergave Advertenties en in rapporten.

>[!TIP]
>
> Als u de geldigheid van een VAST-tag wilt controleren, plakt u deze in een browser en drukt u op **[!UICONTROL Enter]**. Als de tag geldig is, ziet u bovenaan een XML-bestand met `<VAST>`.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de [!UICONTROL Ads] mening, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 30 sec CTV&quot;).

**[!UICONTROL Width | Ad Unit Width]:** De breedte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

**[!UICONTROL Height | Ad Unit Height]:** De hoogte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

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

**[!UICONTROL Clock Number]**: (Alleen gebruikt in het Verenigd Koninkrijk; (alleen beschikbaar voor gebruikers met toestemming) Een unieke id die wordt gebruikt om ervoor te zorgen dat de juiste advertentie wordt uitgezonden. Laat deze instelling leeg als deze niet van toepassing is.

### [!UICONTROL Pixel]

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels desgewenst loskoppelen en nieuwe pixels maken op basis van uw behoeften voor bijhouden.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op *[!UICONTROL Impression]* of *[!UICONTROL Click-through]* worden geactiveerd.

**[!UICONTROL Pixel Type]:** Geeft aan of de pixel een  *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel),  *[!UICONTROL HTML]* of  *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor het opgegeven pixeltype.

**[!UICONTROL Pixel Name]:** De naam van de pixel. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider:  *[!UICONTROL None]*,  *[!UICONTROL Nielsen]* of  *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Een advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)

