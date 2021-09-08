---
title: Instellingen voor audio toevoegen
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor audioadvertenties.
feature: Ads
exl-id: 746b6f40-ff59-4bbe-bfc0-3579d4461e4a
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Instellingen voor audio toevoegen

## [!UICONTROL Upload or Select Creative]

*Alleen nieuwe advertenties*

**[!UICONTROL Upload Audio]:** Een Raw-element uploaden naar DSP. Voer de volgende handelingen uit wanneer u dit selecteert:

1. Klik op **[!UICONTROL Choose File]** en zoek het bestand op uw apparaat of netwerk.
1. Voer een titel in voor het bestand. Deze titel wordt gebruikt in de weergave [!UICONTROL Ads] en rapporten.
1. Klik op **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Audio]:** Om eerder geüploade creatieve bestanden in de juiste indeling in de account te selecteren.

**[!UICONTROL Advanced: VAST Tag URL]:** U kunt als volgt een VAST-tag van derden invoeren die creatieve elementen en pixels bijhoudt:

1. Klik ![pijl](/help/dsp/assets/compressed.png) naast **[!UICONTROL Advanced: VAST Tag URL]**.
1. Voer in het veld **[!UICONTROL URL]** de URL van de VAST-tag in.
1. Voer een **[!UICONTROL Title]** voor het bestand in, dat wordt gebruikt in de weergave [!UICONTROL Ads] en rapporten.

>[!TIP]
>
> Als u de geldigheid van een VAST-tag wilt controleren, plakt u deze in een browser en drukt u op **[!UICONTROL Enter]**. Als de tag geldig is, ziet u bovenaan een XML-bestand met `<VAST>`.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Alleen-lezen) Het advertentietype dat u maakt, komt overeen met het plaatsingstype waaraan de advertentie kan worden gekoppeld. De standaardwaarde is *[!UICONTROL Audio]*.

**[!UICONTROL Ad Name]:** De naam van de advertentie. De titel van het element wordt standaard gebruikt, maar u kunt de naam wijzigen.

>[!TIP]
>
> Gebruik een naam die u gemakkelijk kunt vinden wanneer u de advertentie aan een plaatsing, in de [!UICONTROL Ads] mening, en in rapporten vastmaakt. Beschrijf bijvoorbeeld het eenheidstype en enkele belangrijke kenmerken (zoals Voorvertoning van vakantieproduct: 30sec Audio&quot;).

**[!UICONTROL Ad Duration]:** De lengte van het audiobestand. Het wordt automatisch ingesteld als of [!UICONTROL 15] of [!UICONTROL 30], afhankelijk van de geselecteerde advertentie-eenheid.

Dit veld kan al dan niet worden weergegeven, afhankelijk van de accountmachtigingen.

**[!UICONTROL Click URL]:** (Toevoegen met onbewerkte elementen en alleen met weergavebanners; (optioneel) De URL waarop de viewer landt wanneer deze op een weergavebanner klikt die bij uw advertentie hoort.

**[!UICONTROL Final Click URL]:** (Toevoegen met onbewerkte elementen en alleen met weergavebanners; alleen-lezen) De  [!UICONTROL Click URL] met de benodigde  [Advertising Cloud DSP tracking-](/help/dsp/campaign-management/macros.md) macrosinserted, indien van toepassing.

**[!UICONTROL VAST Tag]:** (Alleen VAST-tags gebruiken) Een URL voor een advertentiebron van derden. Zorg ervoor dat de VAST-tag alleen audiomediabestanden bevat.

**[!UICONTROL Final VAST Tag]:** (Alleen bij het gebruik van VAST-tags) De URL voor de externe advertentie-bron met de benodigde  [Advertising Cloud DSP-](/help/dsp/campaign-management/macros.md) trackingmacro&#39;s, indien van toepassing.

**[!UICONTROL Select Rate]:** (Gebruikers met slechts toestemming) Een vooraf onderhandelde tarief dat door Adobe wordt gefactureerd, of één van de tarieven die u hebt onderhandeld en zal voor door de verkoper in rekening worden gebracht. Neem contact op met uw accountmanager van Adobe om een tarief toe te voegen.

### [!UICONTROL Companion]

*Alleen DSP advertenties*

U kunt desgewenst maximaal drie bijbehorende banners aan een advertentie koppelen. De beste manier is om daar waar mogelijk gezelschapsbanners aan te sluiten.

>[!NOTE]
>
>* Niet alle uitgevers staan gezelschapsbanners toe. De uitgevers die gezelschapsbanners wel toestaan, garanderen geen beletsel voor gezelschapsbanners.
>* Companion banners van externe advertentietags zijn mogelijk niet altijd beschikbaar voor voorvertoning.


**\[Selectievakje\]:** Bevat de opgegeven bijbehorende banner bij de advertentie. Als het selectievakje is uitgeschakeld, wordt de bijbehorende banner niet opgenomen.

**\[Bannergrootte\]:** de grootte van de bijbehorende banner:  *[!UICONTROL 300x250]* (gebruikt voor  [!DNL iHeartRadio],  [!DNL Spotify],  [!DNL SoundCloud], en  [!DNL TuneIn]),  *[!UICONTROL 640x640]* (gebruikt voor  [!DNL Spotify), or *1024x1024]* (gebruikt voor  [!DNL SoundCloud]).

**\[Bron\]:** De bron van het bijbehorende bannerelement:

* *[!UICONTROL Upload My Own Asset]:* Uw eigen middel uploaden.
* *[!UICONTROL Use a Third Party Tag]:* Een iFrame- of scripttag invoeren van een gecertificeerde externe advertentiepartner.

Gebruik een tag van derden wanneer u bannerafdrukken van derden wilt bijhouden.

**[!UICONTROL Asset]:** (Alleen Raw-elementen) Het bijbehorende bannerelement in de GIF-, JPG- of PNG-indeling. Klik **[!UICONTROL Browse]** en bepaal de plaats van het dossier op uw apparaat of netwerk, en klik dan **[!UICONTROL Upload]**.

**[!UICONTROL Click URL]:** (Alleen Raw-elementen) De URL waarop de viewer landt wanneer deze op de bijbehorende banner voor de advertentie klikt. U kunt ook klikken op omleiding gebruiken door een klik van een andere fabrikant op te volgen pixel.

**[!UICONTROL Final Click URL]:** (Alleen Raw-activa; (alleen-lezen) Klik op URL met de benodigde  [Advertising Cloud DSP-trackingmacro&#39;](/help/dsp/campaign-management/macros.md) s, indien van toepassing.

**[!UICONTROL Ad Tag]:** (Alleen advertenties van derden) Een iFrame- of scriptbannertag voor een bannerbron van een derde partij. Het moet afkomstig zijn van een gecertificeerde derde partij en dienstverrichtende partner.

**[!UICONTROL Final Ad Tag]:** (Alleen advertenties van derden) De advertentietags met de benodigde  [Advertising Cloud DSP-](/help/dsp/campaign-management/macros.md) trackingmacro&#39;s worden, indien van toepassing, toegevoegd.

### Pixel

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels desgewenst loskoppelen en nieuwe pixels maken op basis van uw behoeften voor bijhouden.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op *[!UICONTROL Impression]* of *[!UICONTROL Click-through]* worden geactiveerd.

**[!UICONTROL Pixel Type]:** Geeft aan of de pixel een  *[!UICONTROL IMG UR]L*  (afbeeldingsbestand van 1 x 1 pixel)  *[!UICONTROL HTML]* of  *[!UICONTROL JavaScript URL]* is.

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

