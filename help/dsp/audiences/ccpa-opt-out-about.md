---
title: Info [!UICONTROL CCPA Opt-out-of-Sale] Segmenten en rapporten
description: Leer over het creëren van segmenten om IDs van opt-out van CCPA te volgen verzoeken en hoe te om rapporten van identiteitskaarts terug te winnen.
feature: CCPA, DSP Segments
exl-id: 9256d34e-d0dd-4abf-bc96-2b599caf2a8e
source-git-commit: 17482b831c5db7ef6c211f87b2e408443180746e
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Info [!UICONTROL CCPA Opt-out-of-Sale] Segmenten en rapporten

U kunt gebruikers-id&#39;s bijhouden van een aanvraag voor een opt-out-of-sales (opt-out) voor de consument op uw website, op basis van de California Consumer Privacy Act (CCPA), door [tot oprichting en uitvoering van een CCPA-opt-out-of-sales-segment](ccpa-opt-out-segment-create.md). De gebruikers blijven in opt-out van CCPA-segmenten voor onbepaalde tijd.

Wanneer de segmentpixel-tag is geïmplementeerd, begint Adobe-advertentie namens de adverteerder een pool met id&#39;s te verzamelen.

## Rapporten over verkoopverbod voor consumenten

Adobe Advertising genereert maandelijkse rapporten van id&#39;s die klanten hebben ingediend voor een aanvraag om niet te verkopen voor de account. De gegevens consolideren aanvragen die zijn vastgelegd met CCPA-opt-out-of-sales-segmenten die zijn gemaakt in DSP en alle aanvragen die via de Privacy Service-API zijn ingediend.  Rapporten worden gegenereerd op de eerste van elke maand voor de vorige maand. De maandelijkse gebruikerslijst voor juni is bijvoorbeeld beschikbaar op 1 juli.

Elk rapport is beschikbaar als een tekstbestand met tabs als scheidingsteken en gecomprimeerd in de GZIP-indeling. In de CCPA-segmenten vastgelegde gebruikers-id&#39;s worden per segment en per adverteerder geïdentificeerd.

U kunt [koppelingen naar de maandelijkse rapporten ophalen](ccpa-opt-out-segment-report-retrieve.md) die in de voorafgaande drie maanden zijn gemaakt, hetzij vanuit DSP, hetzij met behulp van de DSP [!DNL Trafficking API]. Elke koppeling is zeven dagen geldig, maar wordt telkens vernieuwd wanneer een klant probeert een koppeling op te halen.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Support for the California Consumer Privacy Act: Support voor consumenten](/help/privacy/ccpa-opt-out-of-sale.md)
>* [Een [!UICONTROL CCPA Opt-Out-of-Sale] Segment](ccpa-opt-out-segment-create.md)
>* [Rapporten over verkoopopties voor consumenten ophalen](ccpa-opt-out-segment-report-retrieve.md)
>* [Over Audience Management](audience-about.md)

