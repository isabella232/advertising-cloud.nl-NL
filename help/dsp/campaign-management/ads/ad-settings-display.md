---
title: Ad-instellingen weergeven
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor weergaveadvertenties.
feature: Ads
exl-id: ae88dfab-0b0c-42ab-9135-422b20a4b6cd
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ad-instellingen weergeven

De volgende instellingen gelden voor standaardschermadvertenties. U kunt ook klikvideo-advertenties voor weergaveadvertenties gebruiken, maar dat wordt afgeraden omdat niet veel uitgevers ze ondersteunen.

## [!UICONTROL Ad Options]

### Basis

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld. De standaardwaarde is *[!UICONTROL Display]*.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de [!UICONTROL Ads] mening, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 300 x 250 gamer&quot;).

**\[Bron toevoegen\]**: Of Advertising Cloud DSP de advertentie (*[!UICONTROL Adobe served]*) levert of u een externe advertentieserver (*[!UICONTROL 3rd party]*) gebruikt.

**[!UICONTROL This is an expandable Banner]:** (Alleen advertenties van derden) Geeft aan dat de advertentie een uitbreidbare banneradvertentie is. De gerelateerde uitbreidingsinstellingen bepalen welke voorraad moet worden aangeschaft, zodat deze het advertentiegedrag weerspiegelen.

**[!UICONTROL Expansion Method]:** (Alleen externe banneradvertenties) Of de banner wordt uitgebreid  *[!UICONTROL Click]* of  *[!UICONTROL Rollover]*.

**[!UICONTROL Expansion Directions]:** (Uitgebreide banneradvertenties van derden alleen) De richting waarin de advertentie wordt uitgebreid:  *[!UICONTROL Up]*,  *[!UICONTROL Down]*,  *[!UICONTROL Left]*, of  *[!UICONTROL Right]*.

**[!UICONTROL Certified Vendors]:** (Alleen uitbreidingsbare banneradvertenties van derden) De gecertificeerde leverancier waarvoor de advertentie beschikbaar is:  *[!UICONTROL DCM]* ([!DNL Google DoubleClick for Advertisers]),  *[!UICONTROL Flashtalking]*,  *[!UICONTROL Sizmek]*, of  *[!UICONTROL Jivox]*.

**[!UICONTROL Display Code]:** (Alleen externe advertenties) De URL van het creatieve middel van derden. Alle [timestamp] en [[timestamp]] parameters worden vervangen door werkelijke waarden.

**[!UICONTROL Final Display Code]:** (Alleen externe advertenties) De URL voor het creatieve middel van derden, met de benodigde  [Advertising Cloud DSP-](/help/dsp/campaign-management/macros.md) trackingmacro&#39;s, indien van toepassing.

**[!UICONTROL Creative type]:** (alleen advertenties met Adobe-bediening) Of het element een  *[!UICONTROL Image]* of een  *[!UICONTROL HTML5]* element is.

**[!UICONTROL Asset]|  [!UICONTROL HTML5 Asset]:** (alleen voor advertenties met Adobe-bediening) Een afbeeldingsbestand of gecomprimeerd HTML5-element dat moet worden geüpload, afhankelijk van het creatieve type. Klik **[!UICONTROL Browse]** en bepaal de plaats van het dossier op uw apparaat of netwerk, en klik dan **[!UICONTROL Upload]** of **[!UICONTROL Upload Image]**.

**[!UICONTROL Ad Size]:** De breedte en hoogte van de advertentie. Het moet een [ondersteunde standaardvertoning en grootte](/help/dsp/assets/ad-specs.pdf) zijn. U kunt de advertentiegrootte handmatig invoeren voordat u de advertentie uploadt of een [!UICONTROL Display Code] invoeren. Als u de advertentiegrootte niet invoert, worden de afmetingen van de geüploade advertentie of advertentietag automatisch ingevoerd als alleen-lezen. De advertentie wordt niet opgeslagen als de afmetingen zich niet in de standaardweergave bevinden als grootten, bijvoorbeeld 301x250 in plaats van 300x250 bij het formaat.

>[!IMPORTANT]
>
> De advertentiegrootte die in de velden width en height wordt gedeclareerd, komt overeen met binnenkomende biedaanvragen. U kunt leveringsproblemen ervaren als de afmetingen van de advertentie niet overeenkomen met de gedeclareerde advertentiegrootte.

**[!UICONTROL Click URL]:** (alleen voor advertenties met Adobe-bediening) De URL waarop de viewer landt wanneer deze op de advertentie klikt.

**[!UICONTROL Final Click URL]:** (alleen door Adobe bediende advertenties; alleen-lezen) De  [!UICONTROL Click URL] met de benodigde  [Advertising Cloud DSP tracking-](/help/dsp/campaign-management/macros.md) macrosinserted, indien van toepassing.

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
>* [De aan een advertentie gekoppelde plaatsen weergeven](ad-list-placements.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)

