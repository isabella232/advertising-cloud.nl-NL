---
title: Instellingen voor mobiele advertentie
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor mobiele advertenties.
feature: DSP Ads
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Instellingen voor mobiele advertentie

## [!UICONTROL Insert Ad Tag]

*Alleen nieuwe mobiele video-advertenties*

**[!UICONTROL URL]** of **[!UICONTROL Ad Tag]**: Een VAST-advertentietag of -advertentietag van derden die creatieve elementen en pixels bijhouden bevat

**[!UICONTROL Ad Title]** of **[!UICONTROL Title]**: Een naam voor de advertentie die wordt gebruikt in het dialoogvenster [!UICONTROL Ads] bekijken en rapporteren.

>[!TIP]
>
> Als u de geldigheid van een VAST-tag wilt controleren, plakt u deze in een browser en klikt u op de knop **[!UICONTROL Enter]** toets. Als de tag geldig is, wordt een XML-bestand weergegeven dat `<VAST>` aan de bovenkant.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]: Mobiele weergaveadvertenties

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de mening van Advertenties, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 300 x 250 gamer&quot;).

**\[Bron toevoegen\]**: (Alleen-lezen) *[!UICONTROL 3rd party]*.

**[!UICONTROL Display Code]:** De URL van het creatieve element van derden. Alle [tijdstempel] en [[tijdstempel]]-parameters worden vervangen door werkelijke waarden.

**[!UICONTROL Final Display Code]:** De URL voor het creatieve middel van derden, met de vereiste [Reclame DSP het volgen macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

### [!UICONTROL Basic]: Videoadvertenties

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de mening van Advertenties, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: Phone Preroll&quot;).

**[!UICONTROL Width]| [!UICONTROL Ad Unit Width]:** De breedte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

**[!UICONTROL Height]| [!UICONTROL Ad Unit Height]:** De hoogte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

**[!UICONTROL Player X]:** De X-coördinaat voor de advertentie-eenheid. De standaardinstelling behouden.

**[!UICONTROL Player Y]:** De Y-coördinaat voor de advertentie-eenheid. De standaardinstelling behouden.

**[!UICONTROL Player Width]:** De breedte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

Dit is hetzelfde als **[!UICONTROL Width]** veld.

**[!UICONTROL Player Height]:** De hoogte van de gehele advertentie-eenheid. Deze optie is mogelijk vergrendeld, afhankelijk van het type advertentie-eenheid dat u hebt geselecteerd.

Dit is hetzelfde als **[!UICONTROL Height]** veld.

**[!UICONTROL Show Controls]:** Waar moeten videobesturingselementen voor de advertentie worden opgenomen: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]*, of *[!UICONTROL None]* (de standaardinstelling).

**[!UICONTROL Preserve Aspect Ratio]:** Of de breedte- en hoogteverhouding van de video behouden moet blijven (*[!UICONTROL Yes]*) of om de video uit te rekken tot de beschikbare ruimte (*[!UICONTROL No]*).

**[!UICONTROL Close Button Delay]:** (Sommige advertenties) Het aantal seconden dat nodig is om de weergave van de sluitknop te vertragen.

**[!UICONTROL VAST Tag]:** (Toevoegen met alleen VAST-tags; (alleen-lezen) De VAST-tag van derden die u hebt ingevoerd als het creatieve middel.

**[!UICONTROL Final VAST Tag]:** (Toevoegen met alleen VAST-tags; (alleen-lezen) De VAST-tag van derden die u hebt ingevoerd als het creatieve middel met het vereiste [Reclame DSP het volgen macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL Wmode]:** (Sommige advertentietypen) De venstermodus: *[!UICONTROL window]*, *[!UICONTROL transparent]*, of *[!UICONTROL opaque]*.

### [!UICONTROL Pixel]

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels loskoppelen en nieuwe pixels maken wanneer dat nodig is, op basis van uw behoeften voor bijhouden voor de afzonderlijke advertentie.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op het *[!UICONTROL Impression]* of *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Of de pixel een *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel), *[!UICONTROL HTML]*, of *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor de opgegeven [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** De pixelnaam. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, of *[!UICONTROL Comscore]*.

### [!UICONTROL Sharing]

Vervangen

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Eén advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Advertentiespecificaties](ad-specs.md)
>* [DSP Macros](/help/dsp/campaign-management/macros.md)

