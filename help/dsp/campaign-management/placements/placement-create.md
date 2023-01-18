---
title: Een plaatsing maken
description: Leer hoe u een plaatsing maakt.
feature: DSP Placements
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Een plaatsing maken

>[!TIP]
>
>Plaatsen maken op basis van specifieke campagnedoelen of rapportagebehoeften.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.

1. Klik op de naam van de campagne waarin de plaatsing wordt opgenomen.

1. Klik boven de gegevenstabel op **[!UICONTROL Create]**. In de [!UICONTROL Placement Types] klikt u op het plaatsingstype.

   Het plaatsingstype bepaalt het advertentietype dat de plaatsing kan omvatten.

1. Voer de [plaatsingsinstellingen](placement-settings.md):

   1. Geef de [!UICONTROL Basics] instellingen.

   1. In de [!UICONTROL Goals] in, geeft u de [!UICONTROL Gross Budget] en, naar keuze, specificeer extra plaatsingsdoelstellingen.

      Sommige velden hebben standaardwaarden die u kunt overschrijven.

      Als het pakket waaraan de plaatsing wordt toegewezen pakketniveau het verpakken heeft, dan zullen uw doelstellingen en het verpakken montages de pakketmontages weerspiegelen.

   1. (Optioneel) In het dialoogvenster [!UICONTROL Geo-Targeting] , beperkt u de locaties die zijn opgenomen of uitgesloten.

      Als u geen specifieke plaatsen identificeert, worden alle plaatsen gericht.

      >[!NOTE]
      >
      >De plaatsen van de Stad en DMA zijn niet beschikbaar voor Plaatsen Roku.

   1. In de [!UICONTROL Inventory Targeting] de inventarisbronnen te beperken of uit te sluiten.

      Voor de meeste plaatsingstypen worden alle voorraadtypen en alle bronnen voor elk type standaard opgenomen. Voor [!DNL Roku] U moet het voorraadtype en de bronnen opgeven.

   1. (Optioneel) In het dialoogvenster [!UICONTROL Site Targeting] selecteert, beperkt u de sites waarop u wilt verwijzen en geeft u de sites op die u wilt uitsluiten.

   1. (Optioneel) In het dialoogvenster [!UICONTROL Audience Targeting] sectie:

      1. Versmal het publiek. Dit omvat het selecteren van publiekssegmenten om binnen de plaatsing te richten.

         Voor [!DNL] U kunt plaatsingen gebruiken [DSP unieke publiek dat overeenkomt met [!DNL Roku]](/help/dsp/inventory/roku-inventory.md) door een of meer publiekssegmenten op te nemen die kunnen worden vergeleken met de [!DNL Roku] (opted-in) deterministische gegevensset.
   1. (Voor campagnes met apparaatoverschrijdende doelgerichtheid op het niveau van de mens; (optioneel) Als de plaatsing gericht is op een of meer specifieke doelgroepen, schakelt u op personen gebaseerde cross-device-oriëntatie in voor de plaatsing.

      Op mensen gebaseerde cross-device gerichte toepassingen worden geleverd door [!DNL LiveRamp] alleen gegevens uit de VS gebruiken. De dienst is beschikbaar aan alle adverteerders bij $0.35 CPM voor beelden die door te gebruiken worden geleverd [!DNL LiveRamp] apparaatgrafiek (dat wil zeggen voor apparaten die niet worden gevonden binnen de doelpubliekssegmenten).

   1. (Optioneel) In het dialoogvenster [!DNL Brand Safety and Media Targeting] voor uw plaatsingen.

   1. (Optioneel) In het dialoogvenster [!DNL Tracking] in de plaatsing.

      >[!NOTE]
      >
      >([!DNL Roku] plaatsing) Pixelleveranciers van derden die zijn goedgekeurd door [!DNL Roku] include [!DNL Acxiom], [!DNL comScore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk], en [!DNL Research Now].


1. Klik op **[!UICONTROL Create Placement]**.

1. (Optioneel) Advertenties aan de plaatsing koppelen:

   1. Klik op **[!UICONTROL Attach an ad]**.

   1. Voer een van de volgende handelingen uit:
   * Een nieuwe advertentie maken:

      1. Klik op **[!UICONTROL Create a New Ad].**

      1. Geef de advertentie-instellingen op voor [audioadvertenties](/help/dsp/campaign-management/ads/ad-settings-audio.md), [aangesloten tv](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md), [advertenties weergeven](/help/dsp/campaign-management/ads/ad-settings-display.md), [mobiele advertenties](/help/dsp/campaign-management/ads/ad-settings-mobile.md), [native advertenties](/help/dsp/campaign-management/ads/ad-settings-native.md), [pre-rol advertenties](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md), of [universele videobanden](/help/dsp/campaign-management/ads/ad-settings-universal-video.md).

      1. Klik op **[!UICONTROL Save & Submit for Review]**.

      1. (Optioneel) Klik voor elke aanvullende advertentie die u voor de plaatsing wilt maken op **[!UICONTROL Attach Another Ad]** en herhaal vervolgens stap 1-3.

      1. Als u geen bestaande advertenties wilt bijvoegen, klikt u op **[!UICONTROL I'm done for now]**.
   * Bestaande advertenties toevoegen aan de campagne:

      1. Klik op **[!UICONTROL Select an Ad]**.

      1. Voer een van de volgende handelingen uit:

         * Eén advertentie tegelijk toevoegen:

            1. Klik naast de naam van de advertentie op **[!UICONTROL Select].**

            1. (Optioneel) Klik voor elke aanvullende advertentie die u wilt bijvoegen op **[!UICONTROL Attach Another Ad]** en herhaal vervolgens het proces.
         * U kunt maximaal 20 advertenties tegelijk toevoegen:

            1. Schakel het selectievakje boven de advertentielijst in.

            1. Schakel het selectievakje naast elke advertentie in die u wilt toevoegen.

            1. Klik op **[!UICONTROL Attach]**.

            1. Klik naast de naam van de advertentie op **[!UICONTROL Select]**.
      1. (Optioneel) De standaardvliegperiode en de ad-rotatie overschrijven voor specifieke advertenties in de plaatsing:

         1. Klik op **[!UICONTROL Custom Schedule Ads]**.

         1. Voer een van de volgende handelingen uit:

            * Als u een vlucht wilt toevoegen, klikt u op **[!UICONTROL Add Flight]** en geeft u vervolgens de begin- en einddatum op.

            * Als u een bestaande vlucht wilt toevoegen aan een advertentie, klikt u op **[!UICONTROL +]** in de rij ad voor de vluchtkolom.

            * Als u een bestaande vlucht uit een advertentie wilt verwijderen, klikt u op **[!UICONTROL x]** in de rij ad voor de vluchtkolom.

            * (Als meerdere advertenties dezelfde vlucht hebben) Als u de advertenties ongelijk wilt roteren, klikt u op **[!UICONTROL Even Rotation]** in de vluchtinformatie, en voert vervolgens het relatieve gewicht in waarmee elke advertentie moet worden geroteerd, als percentage.

               De totale gewichten moeten gelijk zijn aan 100.
         1. Klik in de rechterbovenhoek op **[!UICONTROL Continue]**.

         1. Bekijk de vlieggegevens en klik vervolgens op **[!UICONTROL Save & Finish]**.






>[!MORELIKETHIS]
>
>* [Info over Plaatsingsbeheer](placement-about.md)
>* [Een plaatsing bewerken](placement-edit.md)
>* [Het advertentieschema voor een plaatsing bewerken](placement-edit-ad-schedule.md)
>* [Een plaatsing pauzeren of activeren](placement-pause-activate.md)
>* [Het Wijzigingslogboek voor een plaatsing weergeven](placement-change-log.md)
>* [Plaatsingsinstellingen](placement-settings.md)
>* [Sneltoetsen](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)

   >*[Problemen oplossen](/help/dsp/optimization/troubleshooting-performance.md)
>* [Video: Hoe te om een StandaardPlaatsing van de Vertoning te creëren](https://video.tv.adobe.com/v/340454)

