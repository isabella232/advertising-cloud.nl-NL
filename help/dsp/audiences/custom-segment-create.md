---
title: Een aangepast segment maken en implementeren
description: Leer hoe u een aangepast segment kunt maken en implementeren om gebruikers te volgen die worden blootgesteld aan advertenties of gebruikers die uw webpagina's bezoeken.
feature: Segments
exl-id: 691903e2-773e-4205-837e-822f435f57a7
source-git-commit: e2ee41c7e3e195f062ad1cc67080ed913d6d3d06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Een aangepast segment maken en implementeren

U kunt uw eigen gegevens over het eerste publiek verzamelen door een aangepast Advertising Cloud-segment te maken en te implementeren. U kunt het segment gebruiken om a) gebruikers te volgen die aan advertenties van Desktop, mobiele apparaten, en apparaten CTV en b) gebruikers worden blootgesteld die specifieke webpagina&#39;s bezoeken. U kunt gebruikers in het segment later opnieuw richten met extra advertenties of gebruikers in het segment verhinderen extra advertenties te ontvangen.

>[!NOTE]
>
>Om gebruikers IDs van consument van opt-out-of-verkoop verzoeken op uw website, volgens de Wet van de Privacy van de Consumentenbescherming van Californië (CCPA) te volgen, creeer een [opt-out van-CCPA segment](ccpa-opt-out-segment-create.md).

1. Maak het segment:

   1. Klik in het hoofdmenu op **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

   1. Voer een unieke **[!UICONTROL Segment Name]** in.

   1. Selecteer **[!UICONTROL Custom]** voor [!UICONTROL Segment Type].

   1. Ga het Venster van het Segment in, dat het aantal dagen is het koekje van een gebruiker in het segment blijft.

      Het standaardvenster is 45 dagen. Voer een waarde tussen 1 en 365 in.

   1. Klik op **[!UICONTROL Save]**.

1. Kopieer en implementeer tags om het segment bij te houden, indien nodig:

   1. Ga terug naar **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   2. Plaats de cursor op de segmentrij en klik **[!UICONTROL Get pixel]**.

      * Ga als volgt te werk om bezoekers van het bureaublad en mobiele apparaten bij te houden op een webpagina:

         1. Kopieer de tag voor het bijhouden van de paginaweergave, die het label &quot;[!UICONTROL Desktop or mobile websites]&quot; heeft.

         1. Geef de tag door aan de adverteerder of websitecontactpersoon voor implementatie.

            De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.
      * Om gebruikers te volgen die aan een advertentie-eenheid op Desktop, mobiele, of apparaten CTV worden blootgesteld:

         1. Kopieer de code voor het bijhouden van de indruk met het label &quot;[!UICONTROL Desktop or mobile ads]&quot;.

         1. Voeg de tag voor elke advertentie toe aan het tabblad [!UICONTROL Pixel]. <!-- I'll add cross-reference to ad settings later. -->


Zodra een volgende markering wordt uitgevoerd, kunt u het segment in de publieksdoelstellingen of uitsluitingen voor om het even welke plaatsing gebruiken.

>[!TIP]
>
>Houd de segmentgrootte bij terwijl gebruikers worden bijgehouden.

>[!MORELIKETHIS]
>
>* [Over Audience Management](audience-about.md)
>* [Een  [!UICONTROL CCPA Opt-Out-of-Sale] segment maken en implementeren](ccpa-opt-out-segment-create.md)
>* [Een herbruikbaar publiek maken](reusable-audience-create.md)
>* [Instellingen publiek](audience-settings.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

<!-- I'll add x-ref to ad settings later.-->
