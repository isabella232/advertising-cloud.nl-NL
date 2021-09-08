---
title: Creeer en voer een CCPA uit Opt-uit-van-Verkoop segment
description: Leer hoe u een segment maakt en implementeert om gebruikers-id's bij te houden die afkomstig zijn uit een aanvraag voor een opt-out bij de consument.
feature: CCPA, Segments
exl-id: aebe0c5b-382f-4e4a-b145-c32f32d216ca
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creeer en voer een CCPA uit Opt-uit-van-Verkoop segment

U kunt een segment tot stand brengen om gebruikers IDs van consument van uit-verkoopverzoeken op uw website te volgen, volgens de Wet van de Privacy van de consument van Californië (CCPA). De gebruikers blijven in opt-out van CCPA-segmenten voor onbepaalde tijd.

Zodra de segmentpixel-tag is geïmplementeerd, begint Advertising Cloud namens de adverteerder een pool met id&#39;s te verzamelen.

>[!NOTE]
>
>* Zie [https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html](https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html) voor informatie over het doorgeven van optioneel-uit-verkoop CCPA-verzoeken aan Advertising Cloud met de Adobe Experience Platform Privacy Service API.
>* Als u gebruikers wilt volgen die webpagina&#39;s bezoeken voor doeleinden die geen verband houden met het volgen van CCPA-opt-out-of-sale gebeurtenissen, en gebruikers die worden blootgesteld aan advertenties van desktop-, mobiele en CTV-apparaten, maakt u een [aangepast segment](/help/dsp/audiences/custom-segment-create.md).


1. Maak het segment:

   1. Klik in het hoofdmenu op **Soorten publiek > Segmenten**.

   1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

   1. Voer een unieke **[!UICONTROL Segment Name]** in.

      Aanbevolen segmentnaam: &quot;&lt;*De naam van uw adverteerder* - CCPA niet meer in de handel brengen&quot; (zoals &quot;Acme - CCPA niet in de handel&quot;)

   1. Selecteer **[!UICONTROL CCPA Opt-out of sale]** voor [!UICONTROL Segment Type].

   1. Klik op **[!UICONTROL Save]**.

1. Kopieer en implementeer een pixeltag om het segment bij te houden:

   1. Ga terug naar **[!UICONTROL Audiences]>[!UICONTROL Segments]**.

   1. Houd in de segmentrij de cursor boven het nieuwe segment en klik op **[!UICONTROL Get pixel]**.

   1. Kopieer de afbeeldingspixel (te beginnen met `<img src="https://rtd-tm.everesttech.net"`) om gebruikers-id&#39;s van gebruikers van het bureaublad en mobiele bezoekers te verzamelen naar een webpagina.

   1. Geef de tag door aan de adverteerder of de websitecontactpersoon voor implementatie met behulp van het mechanisme dat het bedrijf gebruikt om CCPA-verzoeken om niet te verkopen (zoals het gebruik van een Platform voor beheer van toestemming) bij te houden.

      De IT-afdeling of andere groep van de adverteerder moet mogelijk de implementatie van de tag plannen of hierover worden geïnformeerd.

      Nadat de pixel is geïmplementeerd, begint Advertising Cloud namens de adverteerder een pool met id&#39;s te verzamelen.

      Hoewel de keuze en logica van de implementatie bij de adverteerder liggen, ziet u hier een voorbeeld van hoe een adverteerder de pixel kan afvuren:

      1. Een consument landt op de homepage van de adverteerder.
      1. De consument zoekt en klikt op de knop CCPA-optie om de adverteerder te weigeren.
      1. De consument krijgt een lijst van dienstverleners te zien waarmee de adverteerder werkt.
      1. De consument schakelt het selectievakje uit om gegevens niet aan Adobe Advertising Cloud te verkopen.

         Deze actie activeert de pixel om in brand te steken en de koekjesidentiteitskaart van de consument binnen het gespecificeerde &quot;[!UICONTROL CCPA Opt-out of sale]&quot;segment te verzamelen.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Support voor consumenten](https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html)
>* [Informatie over  [!UICONTROL CCPA Opt-out-of-Sale] segmenten en rapporten](ccpa-opt-out-about.md)
>* [Rapporten over verkoopopties voor consumenten ophalen](ccpa-opt-out-segment-report-retrieve.md)
>* [Een aangepast segment maken en implementeren](custom-segment-create.md)
>* [Over Audience Management](audience-about.md)

