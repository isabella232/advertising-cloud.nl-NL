---
title: Instellingen voor audio toevoegen
description: Zie beschrijvingen van de beschikbare advertentie-instellingen voor audioadvertenties.
feature: DSP Ads
exl-id: 746b6f40-ff59-4bbe-bfc0-3579d4461e4a
source-git-commit: b40c6f08b94e546e5fc068c46b279292a4d8a14f
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Instellingen voor audio toevoegen

## [!UICONTROL Upload or Select Creative]

*Alleen nieuwe advertenties*

**[!UICONTROL Upload Audio]:** Een Raw-element uploaden naar DSP. Voer de volgende handelingen uit wanneer u dit selecteert:

1. Klikken **[!UICONTROL Choose File]** en zoek het bestand op uw apparaat of netwerk.
1. Voer een titel in voor het bestand. Deze titel wordt gebruikt in het dialoogvenster [!UICONTROL Ads] bekijken en rapporteren.
1. Klik op **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Audio]:** Eerder geüploade creatieve bestanden in de juiste indeling in de account selecteren.

**[!UICONTROL Advanced: VAST Tag URL]:** U voert als volgt een VAST-tag van derden in die creatieve elementen en pixels bijhoudt:

1. Klikken ![pijl](/help/dsp/assets/compressed.png) naast **[!UICONTROL Advanced: VAST Tag URL]**.
1. In de **[!UICONTROL URL]** voert u de URL van de VAST-tag in.
1. Voer een **[!UICONTROL Title]** voor het bestand, dat wordt gebruikt in het dialoogvenster [!UICONTROL Ads] bekijken en rapporteren.

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

**[!UICONTROL Click URL]:** (Toevoegingen die ruw materiaal gebruiken en alleen met weergavebanners; (optioneel) De URL waarop de viewer landt wanneer deze op een weergavebanner klikt die bij uw advertentie hoort.

**[!UICONTROL Final Click URL]:** (Toevoegingen die ruw materiaal gebruiken en alleen met weergavebanners; alleen-lezen) De [!UICONTROL Click URL] de nodige [Advertising Cloud DSP-tracking-macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL VAST Tag]:** (Alleen bij gebruik van VAST-tags) Een URL voor een advertentiebron van derden. Zorg ervoor dat de VAST-tag alleen audiomediabestanden bevat.

**[!UICONTROL Final VAST Tag]:** (Alleen bij gebruik van VAST-tags) De URL voor de advertentiebron van derden met de vereiste [Advertising Cloud DSP-tracking-macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL Select Rate]:** (Alleen gebruikers met toestemming) Een vooraf overeengekomen tarief dat in rekening wordt gebracht via Adobe, of een van de tarieven die u hebt onderhandeld en waarvoor de kosten via de leverancier in rekening worden gebracht. Neem contact op met uw [!DNL Adobe] accountteam.

### [!UICONTROL Companion]

*Alleen DSP advertenties*

U kunt desgewenst maximaal drie bijbehorende banners aan een advertentie koppelen. De beste manier is om daar waar mogelijk gezelschapsbanners aan te sluiten.

>[!NOTE]
>
>* Niet alle uitgevers staan gezelschapsbanners toe. De uitgevers die gezelschapsbanners wel toestaan, garanderen geen beletsel voor gezelschapsbanners.
>* Companion banners van externe advertentietags zijn mogelijk niet altijd beschikbaar voor voorvertoning.


**\[Selectievakje\]:** Neemt de opgegeven begeleidende banner op bij de advertentie. Als het selectievakje is uitgeschakeld, wordt de bijbehorende banner niet opgenomen.

**\[Bannergrootte\]:** De grootte van de bijbehorende banner: *[!UICONTROL 300x250]* (wordt gebruikt voor [!DNL iHeartRadio], [!DNL Spotify], [!DNL SoundCloud], en [!DNL TuneIn]), *[!UICONTROL 640x640]* (wordt gebruikt voor [!DNL Spotify), or *1024x1024]* (gebruikt voor [!DNL SoundCloud]).

**\[Bron\]:** De bron van het bijbehorende bannerelement:

* *[!UICONTROL Upload My Own Asset]:* Uw eigen middel uploaden.
* *[!UICONTROL Use a Third Party Tag]:* Een iFrame- of scripttag invoeren van een gecertificeerde externe advertentiepartner.

Gebruik een tag van derden wanneer u bannerafdrukken van derden wilt bijhouden.

**[!UICONTROL Asset]:** (Alleen Raw-elementen) Het bijbehorende bannerelement in GIF-, JPG- of PNG-indeling. Klikken **[!UICONTROL Browse]** en zoek het bestand op uw apparaat of netwerk en klik vervolgens op **[!UICONTROL Upload]**.

**[!UICONTROL Click URL]:** (Alleen Raw-elementen) De URL waarop de viewer wordt aangeland wanneer deze op de bijbehorende banner voor de advertentie klikt. U kunt ook klikken op omleiding gebruiken door een klik van een andere fabrikant op te volgen pixel.

**[!UICONTROL Final Click URL]:** (Alleen ruwe activa; (alleen-lezen) Klik op de URL met de vereiste [Advertising Cloud DSP-tracking-macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

**[!UICONTROL Ad Tag]:** (Alleen advertenties van derden) Een iFrame- of scriptbannertag voor een bannerbron van een derde partij. Het moet afkomstig zijn van een gecertificeerde derde partij en dienstverrichtende partner.

**[!UICONTROL Final Ad Tag]:** (Alleen advertenties van derden) De advertentietag wordt voorzien van de vereiste [Advertising Cloud DSP-tracking-macro&#39;s](/help/dsp/campaign-management/macros.md) ingevoegd, indien van toepassing.

### Pixel

Alle bestaande pixels voor het bijhouden van gebeurtenissen voor de plaatsing worden automatisch gekoppeld. U kunt bestaande pixels desgewenst loskoppelen en nieuwe pixels maken op basis van uw behoeften voor bijhouden.

De volgende instellingen zijn van toepassing op elke pixel die u maakt of bewerkt.

**[!UICONTROL Integration Event]:** De gebeurtenis die de pixel activeert. Gebruik voor dit advertentietype pixels die op het *[!UICONTROL Impression]* of *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Of de pixel een *[!UICONTROL IMG UR]L* (afbeeldingsbestand van 1 x 1 pixel), *[!UICONTROL HTML]*, of *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** De URL van de pixelafbeelding, in de juiste indeling voor het opgegeven pixeltype.

**[!UICONTROL Pixel Name]:** De pixelnaam. Gebruik een naam waarmee u de pixel gemakkelijk kunt herkennen.

**[!UICONTROL Pixel Provider]:** De pixelprovider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, of *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Een advertentie maken](ad-create.md)
>* [De aan een advertentie gekoppelde plaatsen weergeven](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)

