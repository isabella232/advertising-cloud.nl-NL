---
title: Informatie over [!UICONTROL CCPA Opt-out-of-Sale] Segmenten en rapporten
description: Leer over het creëren van segmenten om IDs van opt-out van CCPA te volgen verzoeken en hoe te om rapporten van identiteitskaarts terug te winnen.
feature: CCPA, DSP Segments
exl-id: 9256d34e-d0dd-4abf-bc96-2b599caf2a8e
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Informatie over [!UICONTROL CCPA Opt-out-of-Sale] Segmenten en rapporten

U kunt gebruikers IDs van consument van opt-out-of-verkoop verzoeken op uw website, volgens de Wet van de Privacy van de consument van Californië (CCPA) volgen, door [het creëren en het uitvoeren van een opting-uit-van-verkoop segment CCPA](ccpa-opt-out-segment-create.md). De gebruikers blijven in opt-out van CCPA-segmenten voor onbepaalde tijd.

Zodra de segmentpixel-tag is geïmplementeerd, begint Advertising Cloud namens de adverteerder een pool met id&#39;s te verzamelen.

## Rapporten over verkoopverbod voor consumenten

Advertising Cloud genereert maandelijkse rapporten met id&#39;s die klanten hebben ingediend voor een aanvraag om te weigeren te verkopen voor de account. De gegevens consolideren aanvragen die zijn vastgelegd met CCPA-opt-out-of-sales-segmenten die in Advertising Cloud DSP zijn gemaakt en alle aanvragen die via de Privacy Service-API zijn ingediend.  Rapporten worden gegenereerd op de eerste van elke maand voor de vorige maand. De maandelijkse gebruikerslijst voor juni is bijvoorbeeld beschikbaar op 1 juli.

Elk rapport is beschikbaar als een tekstbestand met tabs als scheidingsteken en gecomprimeerd in de GZIP-indeling. In de CCPA-segmenten vastgelegde gebruikers-id&#39;s worden per segment en per adverteerder geïdentificeerd.

U kunt [koppelingen ophalen naar de maandelijkse rapporten](ccpa-opt-out-segment-report-retrieve.md) die in de voorafgaande drie maanden zijn gemaakt, vanuit Advertising Cloud DSP of met de Advertising Cloud [!DNL Trafficking API]. Elke koppeling is zeven dagen geldig, maar wordt telkens vernieuwd wanneer een klant probeert een koppeling op te halen.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Support voor consumenten](https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html)
>* [Een  [!UICONTROL CCPA Opt-Out-of-Sale] segment maken en implementeren](ccpa-opt-out-segment-create.md)
>* [Rapporten over verkoopopties voor consumenten ophalen](ccpa-opt-out-segment-report-retrieve.md)
>* [Over Audience Management](audience-about.md)

