---
title: Creeer en voer een CCPA uit Opt-uit-van-Verkoop segment
description: Leer hoe u een segment maakt en implementeert om gebruikers-id's te traceren op basis van verzoeken van consumenten om te weigeren een product te verkopen.
feature: CCPA, DSP Segments
exl-id: 0623c52e-02ea-4e06-bc54-8abb7a87765a
source-git-commit: e9d9d51302d32b06af805917db2f46e5f6daee62
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Creeer en voer een CCPA uit Opt-uit-van-Verkoop segment

U kunt een segment tot stand brengen om gebruikers IDs van consument van uit-verkoopverzoeken op uw website te volgen, volgens de Wet van de Privacy van de consument van Californië (CCPA). De gebruikers blijven in opt-out van CCPA-segmenten voor onbepaalde tijd.

Wanneer de segmentpixel-tag is geïmplementeerd, begint Adobe-advertentie namens de adverteerder een pool met id&#39;s te verzamelen.

>[!NOTE]
>
>* Voor informatie over het communiceren van CCPA-aanvragen voor niet-verkoop aan Adobe Advertising met de Adobe Experience Platform Privacy Service API, raadpleegt u [https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ccpa/ccpa-opt-out-of-sale.html](/help/privacy/ccpa/ccpa-opt-out-of-sale.md).
>* Als u gebruikers wilt volgen die webpagina&#39;s bezoeken voor doeleinden die geen verband houden met het volgen van CCPA-opt-out-of-sale gebeurtenissen, en gebruikers die worden blootgesteld aan advertenties van desktop-, mobiele en CTV-apparaten, maakt u een [aangepast segment](/help/dsp/audiences/custom-segment-create.md).


1. Maak het segment:

   1. Klik in het hoofdmenu op **Soorten publiek > Segmenten**.

   1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

   1. Voer een unieke waarde in **[!UICONTROL Segment Name]**.

      Aanbevolen segmentnaam: &quot;&lt;*De naam van uw adverteerder*> - CCPA niet meer in de handel&quot; (zoals &quot;Acme - CCPA niet meer in de handel&quot;)

   1. Voor de [!UICONTROL Segment Type], selecteert u **[!UICONTROL CCPA Opt-out of sale]**.

   1. Klik op **[!UICONTROL Save]**.

1. Kopieer en implementeer een pixeltag om het segment bij te houden:

   1. Terug naar **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   1. Houd de cursor in de segmentrij boven het nieuwe segment en klik op **[!UICONTROL Get pixel]**.

   1. De afbeeldingspixel kopiëren (beginnen met `<img src="https://rtd-tm.everesttech.net"`) om gebruikers-id&#39;s van bezoekers van het bureaublad en mobiele apparaten te verzamelen op een webpagina.

   1. Geef de tag door aan de adverteerder of de websitecontactpersoon voor implementatie met behulp van het mechanisme dat het bedrijf gebruikt om CCPA-verzoeken om niet te verkopen (zoals het gebruik van een Platform voor beheer van toestemming) bij te houden.

      De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.

      Wanneer de pixel is geïmplementeerd, begint Adobe Advertising namens de adverteerder een pool met id&#39;s te verzamelen.

      Hoewel de keuze en logica van de implementatie bij de adverteerder liggen, ziet u hier een voorbeeld van hoe een adverteerder de pixel kan afvuren:

      1. Een consument landt op de homepage van de adverteerder.
      1. De consument zoekt en klikt op de knop CCPA-optie om de adverteerder te weigeren.
      1. De consument krijgt een lijst van dienstverleners te zien waarmee de adverteerder werkt.
      1. De consument schakelt het selectievakje uit om gegevens niet te verkopen aan Adobe-advertenties.

         Deze actie activeert de pixel om in brand te steken en de koekjesidentiteitskaart van de consument binnen gespecificeerde te verzamelen &quot;[!UICONTROL CCPA Opt-out of sale]&quot; segment.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Support for the California Consumer Privacy Act: Support voor consumenten](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)
>* [Info [!UICONTROL CCPA Opt-out-of-Sale] Segmenten en rapporten](ccpa-opt-out-about.md)
>* [Rapporten over verkoopopties voor consumenten ophalen](ccpa-opt-out-segment-report-retrieve.md)
>* [Een aangepast segment maken en implementeren](custom-segment-create.md)
>* [Over Audience Management](audience-about.md)

