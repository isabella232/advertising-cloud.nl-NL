---
title: Over Advertentiebeheer in Advertising Cloud DSP
description: Meer informatie over advertentiebeheer.
feature: Ads
exl-id: 72c8bbef-d09c-4cf4-994d-99578d043d39
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Over Advertentiebeheer in Advertising Cloud DSP

<!-- add "The Ads View (Dashboard?)" section -->

Advertising Cloud DSP biedt twee manieren om advertenties aan te bieden:

* Advertising Cloud DSP biedt uw advertenties gratis aan wanneer u uw eigen middelen rechtstreeks naar DSP uploadt (zoals weergavebanners, video-elementen, audiobestanden of URL&#39;s). Voor DSP middelen hebt u toegang tot extra functies, zoals overlays.

* Als u een externe advertentieserver gebruikt (zoals Google, Flashtalk of Sizmek), kunt u uw tags voor advertenties van derden uploaden om deze afzonderlijk of bulksgewijs te DSP. Voor de functie voor bulkupload moet u a) DoubleClick- en Flashtalk-tagbladen uploaden of b) een sjabloon downloaden, uw tags in de sjabloon invoeren en de sjabloon vervolgens opnieuw uploaden.<!-- need a list of all supported third-party ad servers; see file in future-tbd folder -->

Wanneer uw advertenties zijn ingesteld, moet u elke advertentie aan een plaatsing koppelen, die de doelparameters bevat (zoals geo, publiek, apparaat en inventarisgericht maken) die bepalen hoe uw campagne zal worden uitgevoerd. U kunt één advertentie aan een of meerdere plaatsen vastmaken.

## Beschikbare advertentietypen

* Audio
* Verbonden tv
* Weergave
* Mobiel
* Oorspronkelijk
* Pre-Roll

Zie [Beschikbare advertentietypen](ad-types.md) en de volledige [Specificaties toevoegen](/help/dsp/assets/ad-specs.pdf) voor meer informatie over deze advertentietypen.

## Speciale Advertentiefuncties

De volgende functies zijn alleen beschikbaar voor advertenties met DSP inhoud.

### Companion Banners

Companion banners worden geleverd naast [pre-roll advertenties](ad-settings-pre-roll.md) of (met sommige uitgevers) [audio advertenties](ad-settings-audio.md) en kunnen de merk- en berichtkoppeling helpen versterken.

>[!NOTE]
>
>* Niet alle uitgevers staan gezelschapsbanners toe. De uitgevers die gezelschapsbanners wel toestaan, garanderen geen beletsel voor gezelschapsbanners.
>* Companion banners van externe advertentietags zijn mogelijk niet altijd beschikbaar voor voorvertoning.


U kunt uw eigen bannerelement voor de partner uploaden of een iFrame- of scriptbannertag van derden uploaden van een gecertificeerde externe advertentiepartner.

### Bedekkingen

Overlays helpen u bij het doorlopen van branding in de video en kunnen extra klikken stimuleren. De overlayfunctie is beschikbaar voor [interactieve pre-roll advertenties](ad-settings-pre-roll.md) en voor [mobiele advertenties in interactieve en tap-naar-play formaten](ad-settings-mobile.md).

Zie [Aanbevolen werkwijzen voor het ontwerpen van overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)

### Teasers

Een gummetje is een opvallende afbeelding die de kijker ertoe aanzet een advertentie af te spelen. Teasers zijn alleen van toepassing op mobiele &#39;tap-to-play&#39;-advertentieformaten.

## Goedkeuringen Advertising Cloud DSP Ad

Wanneer u een advertentie maakt, controleert Advertising Cloud DSP deze op gevoelige categorieën, klikt u op URL-functionaliteit en geeft u een voorvertoning van de rendering weer.

Aanvankelijk, zult u een rode stip in de [!UICONTROL Status] kolom zien. Het herzieningsproces duurt gewoonlijk 24 tot 48 uur. Een verbroken advertentie kan echter langer dan 48 uur in behandeling zijn, dus u hebt tijd om fouten op te lossen voordat de advertentie wordt afgewezen. Geweigerde advertenties bevatten een reden voor de afwijzing.

Wanneer DSP een advertentie goedkeurt, ziet u een groene stip in de kolom Status.

![goedkeuringsindicator in  [!UICONTROL Status] kolom](/help/dsp/assets/ad-approval-status.png)

>[!NOTE]
>
>Uw advertentie zal slechts worden gediend als zowel DSP als het SSP creatief hebben goedgekeurd. Elk SSP heeft zijn eigen goedkeuringsvereisten en proces.

>[!MORELIKETHIS]
>
>* [Een advertentie maken](ad-create.md)
>* [Meerdere externe advertenties maken](ad-create-third-party.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)

