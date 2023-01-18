---
title: Instellingen voor audio toevoegen
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor audioadvertenties.
feature: DSP Ads
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Instellingen voor audio toevoegen

## [!UICONTROL Insert Ad Tag]

*Alleen nieuwe advertenties*

**[!UICONTROL URL]**: De URL van de VAST-tag.

**[!UICONTROL Title]**: Een naam voor het bestand, die wordt gebruikt in het dialoogvenster [!UICONTROL Ads] bekijken en rapporteren.

>[!TIP]
>
> Als u de geldigheid van een VAST-tag wilt controleren, plakt u deze in een browser en klikt u op de knop **[!UICONTROL Enter]** toets. Als de tag geldig is, wordt een XML-bestand weergegeven dat `<VAST>` aan de bovenkant.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld. De standaardinstellingen *[!UICONTROL Audio]*.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing koppelt, in [!UICONTROL Ads] en in rapporten. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 30sec Audio&quot;).

**[!UICONTROL Ad Duration]:** De lengte van het audiobestand. Deze wordt automatisch ingesteld als [!UICONTROL 15] of [!UICONTROL 30], afhankelijk van de geselecteerde advertentie-eenheid.

Dit veld kan al dan niet worden weergegeven, afhankelijk van de accountmachtigingen.

**[!UICONTROL VAST Tag]:** (Alleen bij gebruik van VAST-tags) Een URL voor een advertentiebron van derden. Zorg ervoor dat de VAST-tag alleen audiomediabestanden bevat.

**[!UICONTROL Final VAST Tag]:** (Alleen bij gebruik van VAST-tags) De URL voor de advertentiebron van derden met de vereiste [Reclame DSP het volgen macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL Select Rate]:** (Alleen gebruikers met toestemming) Een vooraf overeengekomen tarief dat in rekening wordt gebracht via Adobe, of een van de tarieven die u hebt onderhandeld en waarvoor de kosten via de leverancier in rekening worden gebracht. Neem contact op met uw [!DNL Adobe] accountteam.

### Pixel

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels loskoppelen en nieuwe pixels maken wanneer dat nodig is, op basis van uw behoeften voor bijhouden voor de afzonderlijke advertentie.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op het *[!UICONTROL Impression]* of *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Of de pixel een *[!UICONTROL IMG UR]L* (afbeeldingsbestand van 1 x 1 pixel), *[!UICONTROL HTML]*, of *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor het opgegeven pixeltype.

**[!UICONTROL Pixel Name]:** De pixelnaam. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, of *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Eén advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Advertentiespecificaties](ad-specs.md)
>* [DSP Macros](/help/dsp/campaign-management/macros.md)

