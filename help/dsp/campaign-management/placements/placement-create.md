---
title: Een plaatsing maken
description: Leer hoe u een plaatsing maakt.
feature: DSP Placements
exl-id: 4e37b571-9af4-4897-bff2-035a5f2600a5
source-git-commit: 608774723f865c22bfdd5c911ac818600a495114
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Een plaatsing maken

>[!TIP]
>
>Plaatsen maken op basis van specifieke campagnedoelen of rapportagebehoeften.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.

1. Klik op de naam van de campagne waarin de plaatsing wordt opgenomen.

1. Klik boven de gegevenstabel op **[!UICONTROL Create]**. Klik in de sectie [!UICONTROL Placement Types] van het menu op het plaatsingstype.

   Het plaatsingstype bepaalt het advertentietype dat de plaatsing kan omvatten.

1. Voer de [plaatsingsinstellingen](placement-settings.md) in:

   1. Geef de [!UICONTROL Basics]-instellingen op.

   1. Geef in de sectie [!UICONTROL Goals] [!UICONTROL Gross Budget] op en geef desgewenst aanvullende plaatsingsdoelen op.

      Sommige velden hebben standaardwaarden die u kunt overschrijven.

      Als het pakket waaraan de plaatsing wordt toegewezen pakketniveau het verpakken heeft, dan zullen uw doelstellingen en het verpakken montages de pakketmontages weerspiegelen.

   1. (Optioneel) Verklein in de sectie [!UICONTROL Geo-Targeting] de locaties die zijn opgenomen of uitgesloten.

      Als u geen specifieke plaatsen identificeert, worden alle plaatsen gericht.

      >[!NOTE]
      >
      >De plaatsen van de Stad en DMA zijn niet beschikbaar voor Plaatsen Roku.

   1. Verklein in de sectie [!UICONTROL Inventory Targeting] de inventarisbronnen die u wilt opnemen of uitsluiten.

      Voor de meeste plaatsingstypen worden alle voorraadtypen en alle bronnen voor elk type standaard opgenomen. Voor [!DNL Roku] plaatsingen, moet u het inventaristype en de bronnen specificeren.

   1. (Optioneel) Verklein in de sectie [!UICONTROL Site Targeting] de sites waarop u wilt verwijzen en geef de sites op die u wilt uitsluiten.

   1. (Optioneel) In de sectie [!UICONTROL Audience Targeting]:

      1. Versmal het publiek. Dit omvat het selecteren van publiekssegmenten om binnen de plaatsing te richten.

         Voor [!DNL] plaatsing van de Roku, kunt u hefboomwerking [DSP uniek publiek dat met  [!DNL Roku]](/help/dsp/inventory/roku-inventory.md) door één of meerdere publiekssegmenten te omvatten die tegen [!DNL Roku] (opted-in) deterministische dataset kunnen worden aangepast.
   1. (Voor campagnes met apparaatoverschrijdende doelgerichtheid op het niveau van de mens; (optioneel) Als de plaatsing gericht is op een of meer specifieke doelgroepen, schakelt u op personen gebaseerde cross-device-oriëntatie in voor de plaatsing.

      Op mensen gebaseerde cross-device targeting wordt alleen door [!DNL LiveRamp] geleverd met Amerikaanse gegevens. De dienst is beschikbaar aan alle adverteerders bij $0.35 CPM voor beelden die door de [!DNL LiveRamp] apparatengrafiek worden geleverd te gebruiken (namelijk voor apparaten die niet binnen de gerichte publiekssegmenten worden gevonden).

   1. (Optioneel) Pas in de sectie [!DNL Brand Safety and Media Targeting] merkveiligheidsbeperkingen toe op uw plaatsen.

   1. (Optioneel) Voer in de sectie [!DNL Tracking] gebeurtenispixels van derden of conversiepixels voor advertenties in de plaatsing in.

      >[!NOTE]
      >
      >([!DNL Roku] plaatsing) Pixelleveranciers van derden die zijn goedgekeurd door [!DNL Roku] omvatten [!DNL Acxiom], [!DNL comScore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], 13/>, [!DNL Placed], [!DNL Polk] en [!DNL Research Now].[!DNL Oracle]


1. Klik op **[!UICONTROL Create Placement]**.

1. (Optioneel) Advertenties aan de plaatsing koppelen:

   1. Klik op **[!UICONTROL Attach an ad]**.

   1. Voer een van de volgende handelingen uit:
   * Een nieuwe advertentie maken:

      1. Klik op **[!UICONTROL Create a New Ad].**

      1. Geef de advertentie-instellingen op voor [audioadvertenties](/help/dsp/campaign-management/ads/ad-settings-audio.md), [aangesloten tv](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md), [weergaveadvertenties](/help/dsp/campaign-management/ads/ad-settings-display.md), [mobiele advertenties](/help/dsp/campaign-management/ads/ad-settings-mobile.md), [native advertenties](/help/dsp/campaign-management/ads/ad-settings-native.md) of [pre-roll advertenties](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md).

      1. Klik op **[!UICONTROL Save & Submit for Review]**.

      1. (Optioneel) Voor elke aanvullende advertentie die u voor de plaatsing wilt maken, klikt u op **[!UICONTROL Attach Another Ad]** en herhaalt u vervolgens stap 1-3.

      1. Als u geen bestaande advertenties wilt koppelen, klikt u op **[!UICONTROL I'm done for now]**.
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

            * Als u een bestaande vlucht aan een advertentie wilt toevoegen, klikt u op **[!UICONTROL +]** in de rij voor het toevoegen van een advertentie voor de vluchtkolom.

            * Als u een bestaande vlucht uit een advertentie wilt verwijderen, klikt u op **[!UICONTROL x]** in de rij voor het toevoegen van de vluchtkolom.

            * (Als meerdere advertenties dezelfde vlucht hebben) Als u de advertenties ongelijk wilt roteren, klikt u op **[!UICONTROL Even Rotation]** in de vluchtinformatie en voert u vervolgens het relatieve gewicht in waarmee u elke advertentie wilt roteren, als een percentage.

               De totale gewichten moeten gelijk zijn aan 100.
         1. Klik in de rechterbovenhoek op **[!UICONTROL Continue]**.

         1. Controleer de vlieggegevens en klik op **[!UICONTROL Save & Finish]**.




>[!MORELIKETHIS]
>
>* [Info over Plaatsingsbeheer](placement-about.md)
>* [Een plaatsing bewerken](placement-edit.md)
>* [Het advertentieschema voor een plaatsing bewerken](placement-edit-ad-schedule.md)
>* [Een plaatsing pauzeren of activeren](placement-pause-activate.md)
>* [Plaatsingsinstellingen](placement-settings.md)
>* [Sneltoetsen](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)

   >*[Problemen oplossen](/help/dsp/optimization/troubleshooting-performance.md)

