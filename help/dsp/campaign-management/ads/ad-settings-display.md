---
title: Ad-instellingen weergeven
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor weergaveadvertenties.
feature: DSP Ads
exl-id: ae88dfab-0b0c-42ab-9135-422b20a4b6cd
source-git-commit: bcece4bfec6f8a765cced3ee230fd8cbf3055b7b
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Ad-instellingen weergeven

De volgende instellingen gelden voor standaardschermadvertenties.

## [!UICONTROL Ad Options]

### Basis

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld. De standaardinstellingen *[!UICONTROL Display]*.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing koppelt, in [!UICONTROL Ads] en in rapporten. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 300 x 250 gamer&quot;).

**\[Bron toevoegen\]**: (Alleen-lezen) *[!UICONTROL 3rd party]*.

**[!UICONTROL This is an expandable Banner]:** (Alleen advertenties van derden) Geeft aan dat de advertentie een uitbreidbare banneradvertentie is. De gerelateerde uitbreidingsinstellingen bepalen welke voorraad moet worden aangeschaft, zodat deze het advertentiegedrag weerspiegelen.

**[!UICONTROL Expansion Method]:** (Alleen uitbreidingsbare banneradvertenties van derden) Of de banner wordt uitgevouwen *[!UICONTROL Click]* of *[!UICONTROL Rollover]*.

**[!UICONTROL Expansion Directions]:** (Uitgebreide banneradvertenties van derden alleen) De richting waarin de advertentie wordt uitgebreid: *[!UICONTROL Up]*, *[!UICONTROL Down]*, *[!UICONTROL Left]*, of *[!UICONTROL Right]*.

**[!UICONTROL Certified Vendors]:** (Alleen uitbreidingsbare banneradvertenties van derden) De gecertificeerde leverancier waarvoor de advertentie beschikbaar is: *[!UICONTROL DCM]* ([!DNL Google DoubleClick for Advertisers]), *[!UICONTROL Flashtalking]*, *[!UICONTROL Sizmek]*, of *[!UICONTROL Jivox]*.

**[!UICONTROL Display Code]:** (Alleen externe advertenties) De URL van het creatieve element van derden. Alle [tijdstempel] en [[tijdstempel]]-parameters worden vervangen door werkelijke waarden.

**[!UICONTROL Final Display Code]:** (Alleen externe advertenties) De URL voor het creatieve middel van derden, met de vereiste [Advertising Cloud DSP-tracking-macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL Ad Size]:** De breedte en hoogte van de advertentie. Het moet [ondersteunde standaardweergave en -grootte](ad-specs.md). U kunt de advertentiegrootte handmatig invoeren voordat u de advertentie uploadt of een [!UICONTROL Display Code]. Als u de advertentiegrootte niet invoert, worden de afmetingen van de geüploade advertentie of advertentietag automatisch ingevoerd als alleen-lezen. De advertentie wordt niet opgeslagen als de afmetingen zich niet in de standaardweergave bevinden als grootten, bijvoorbeeld 301x250 in plaats van 300x250 bij het formaat.

>[!IMPORTANT]
>
> De advertentiegrootte die in de velden width en height wordt gedeclareerd, komt overeen met binnenkomende biedaanvragen. U kunt leveringsproblemen ervaren als de afmetingen van de advertentie niet overeenkomen met de gedeclareerde advertentiegrootte.

### [!UICONTROL Pixel]

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels loskoppelen en nieuwe pixels maken wanneer dat nodig is, op basis van uw behoeften voor bijhouden voor de afzonderlijke advertentie.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op het *[!UICONTROL Impression]* of *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Of de pixel een *[!UICONTROL IMG URL]* (afbeeldingsbestand van 1 x 1 pixel), *[!UICONTROL HTML]*, of *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor de opgegeven [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** De pixelnaam. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, of *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Eén advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](ad-list-placements.md)
>* [Advertentiespecificaties](ad-specs.md)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)

