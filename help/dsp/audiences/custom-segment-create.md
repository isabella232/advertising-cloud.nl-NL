---
title: Een aangepast segment maken en implementeren
description: Leer hoe u een aangepast segment kunt maken en implementeren om gebruikers te volgen die worden blootgesteld aan advertenties of gebruikers die uw webpagina's bezoeken.
feature: DSP Segments
exl-id: 691903e2-773e-4205-837e-822f435f57a7
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Een aangepast segment maken en implementeren

U kunt uw eigen gegevens van het eerste publiek verzamelen door een douane DSP segment te creëren en uit te voeren. U kunt het segment gebruiken om a) gebruikers te volgen die aan advertenties van Desktop, mobiele apparaten, en apparaten CTV en b) gebruikers worden blootgesteld die specifieke webpagina&#39;s bezoeken. U kunt gebruikers in het segment later opnieuw richten met extra advertenties of gebruikers in het segment verhinderen extra advertenties te ontvangen.

>[!NOTE]
>
>Als u gebruikers-id&#39;s wilt bijhouden van een aanvraag voor een opt-out-of-verkoop voor een consument op uw website, maakt u een [CCPA opt-out of-of-sales segment](ccpa-opt-out-segment-create.md).

1. Maak het segment:

   1. Klik in het hoofdmenu op **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

   1. Voer een unieke waarde in **[!UICONTROL Segment Name]**.

   1. Voor de **[!UICONTROL Segment Type]**, selecteert u *[!UICONTROL Custom]*.

   1. Voer de **[!UICONTROL Segment Window]** Dit is het aantal dagen dat een cookie van een gebruiker in het segment blijft staan.

      Het standaardvenster is 45 dagen. Voer een waarde tussen 1 en 365 in.

   1. Klik op **[!UICONTROL Save]**.

1. Kopieer en implementeer tags om het segment bij te houden, indien nodig:

   1. Terug naar **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   2. Plaats de cursor op de segmentrij en klik op **[!UICONTROL Get Pixel]**.

      * Ga als volgt te werk om bezoekers van het bureaublad en mobiele apparaten bij te houden op een webpagina:

         1. Kopieer de tag voor het bijhouden van de paginaweergave, die is gelabeld als &quot;[!UICONTROL Desktop or mobile websites].&quot;

         1. Geef de tag door aan de adverteerder of websitecontactpersoon voor implementatie.

            De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.
      * Om gebruikers te volgen die aan een advertentie-eenheid op Desktop, mobiele, of apparaten CTV worden blootgesteld:

         1. Kopieer de code voor het bijhouden van de indruk met het label &quot;[!UICONTROL Desktop or mobile ads].&quot;


1. Voeg de tag toe aan de [!UICONTROL Pixel] tabblad voor elke relevante advertentie of voor de [!UICONTROL Event Pixels] van de [[!UICONTROL Tracking] instellingen voor elke relevante plaatsing](/help/dsp/campaign-management/placements/placement-settings.md#placement-tracking).

Zodra een volgende markering wordt uitgevoerd, kunt u het segment in de publieksdoelstellingen of uitsluitingen voor om het even welke plaatsing gebruiken.

>[!TIP]
>
>Houd de segmentgrootte bij terwijl gebruikers worden bijgehouden.

>[!MORELIKETHIS]
>
>* [Over Audience Management](audience-about.md)
>* [Segmentinformatie bewerken](segment-edit.md)
>* [Een segment verwijderen](segment-delete.md)
>* [Trackingpixels voor een segment weergeven](segment-view-pixels.md)
>* [Delen of Stoppen met delen van een segment](segment-share.md)
>* [Een [!UICONTROL CCPA Opt-Out-of-Sale] Segment](ccpa-opt-out-segment-create.md)
>* [Een herbruikbaar publiek maken](reusable-audience-create.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

