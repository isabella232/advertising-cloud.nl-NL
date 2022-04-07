---
title: '"Maak een [!UICONTROL Simple Ad Serving] Overeenkomst"'
description: '"Leer hoe u een tekstspatiëringspixel maakt voor een [!UICONTROL Simple Ad Serving] deal."'
feature: DSP Simple Ad Serving
exl-id: d8de85ec-616c-44ed-9a1a-cc25713ad4a4
source-git-commit: 3eb63e9d7161c354736ce53ee21518882c541884
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Een [!UICONTROL Simple Ad Serving] Deal

1. Klik in het hoofdmenu op **[!UICONTROL Inventory]> [!UICONTROL Deals].**

1. Klik boven de gegevenstabel op **[!UICONTROL Create]** en selecteer vervolgens **[!UICONTROL Simple Ad Serving]**.

1. Voer de [deal-instellingen](simple-deal-settings.md):

   1. In de [!UICONTROL Select Ad Source] , geeft u informatie op over de uitgever, adverteerder en de campagne en het type advertentie en klikt u vervolgens op **[!UICONTROL Next]**.

   1. In de [!UICONTROL Select Ad(s)] een advertentie opgeven die in DSP als proxy moet worden gebruikt:

      1. Voer een van de volgende handelingen uit:

         * Selecteer voor bestaande advertenties de advertenties die u wilt gebruiken.

         * Voor nieuwe advertenties maakt u een proxy [advertenties van derden](/help/dsp/campaign-management/ads/ad-create-multiple.md).
      >[!NOTE]
      > DSP zal de advertenties die u opgeeft, niet bedienen. De uitgever zal de advertentie bedienen.

      1. Klik op **[!UICONTROL Next]**.
   1. Bewerk in Details feed de gegevens van de feed en klik vervolgens op **[!UICONTROL Next]**.

      Advertising Cloud DSP genereert automatisch een plaatsing met de naam &quot;SAS Placement - &lt;*naam van deal*>,&quot; voor de advertentie. In de plaatsing, wordt de overeenkomst automatisch gericht in [!UICONTROL Inventory Targets] sectie. Alle andere doelopties zijn niet van toepassing.



1. Verzend de pixels voor het bijhouden van gebeurtenissen naar de uitgever voor implementatie op een van de volgende manieren:

   * (Optioneel) Van de [!UICONTROL Activate Tag with Publisher] scherm, verzend de overeenkomstenmarkering naar de uitgever.

      Wanneer u de vorige stappen hebt uitgevoerd, genereert DSP een e-mailbericht dat u naar de uitgever kunt verzenden. Het bericht omvat de overeenkomstendetails, een verbinding waarvan om de overeenkomstenmarkering terug te winnen, en een vergunningscode voor de verbinding.

      1. Herzie de overeenkomstendetails, en doe dan één van beiden van het volgende:

         * Als u de gegevens in een e-mailbericht in een e-mailtoepassing op uw apparaat wilt plakken, klikt u op **[!UICONTROL Email & Done]** en selecteer de e-mailtoepassing. De [!UICONTROL CC:] veld is vooraf gevuld met een [!DNL Adobe] ondersteuningsadres. U kunt het bericht dan naar het aangewezen contact voor de uitgever verzenden.

         * Als u de gegevens naar het klembord wilt kopiëren, klikt u op **[!UICONTROL Copy Email].** Vervolgens kunt u de inhoud handmatig in een e-mailbericht plakken en naar de juiste contactpersoon voor de uitgever verzenden. U moet een kopie (CC:) opnemen naar `publisher-support-global@adobe.com`. Wanneer u klaar bent met het kopiëren van het bericht, klikt u op **[!UICONTROL Email & Done]**.
      1. (Indien nodig) Neem contact op met de uitgever om te controleren of de tag de juiste macro&#39;s bevat, zodat de tag kan worden gebruikt voor de advertentieserver van de uitgever.
   * (Optioneel) Stuur de pixels voor het bijhouden van gebeurtenissen handmatig naar de uitgever:

      1. In de overeenkomstenrij binnen [!UICONTROL Deals] weergeven, klikken ![Menu Opties](/help/dsp/assets/options-menu.png) **>[!UICONTROL show pixel]**.

         De gebeurtenispixels bevatten een [!UICONTROL Clickthrough] en [!UICONTROL Impression] pixel. Video- en audioadvertenties bevatten ook gebeurtenispixels die met kwartiel zijn voltooid (van [!UICONTROL 25% Complete] tot [!UICONTROL 100% Complete]).

      1. Kopieer de pixels voor het bijhouden van gebeurtenissen en geef deze door aan uw uitgever.



>[!MORELIKETHIS]
>
>* [Info [!UICONTROL Simple Ad Serving]](simple-deal-about.md)
>* [[!UICONTROL Simple Ad Serving] Instellingen](simple-deal-settings.md)
>* [Pixels voor het bijhouden van gebeurtenissen weergeven voor een [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)

