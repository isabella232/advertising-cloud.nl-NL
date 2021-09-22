---
title: Meerdere externe advertenties maken
description: Leer hoe u meerdere advertenties van derden tegelijk kunt maken.
feature: DSP Ads
exl-id: 83d35d27-1ab6-4fcf-877f-650a2dc6975a
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Meerdere externe advertenties maken

U kunt maximaal 500 advertenties van derden tegelijk maken door tags te uploaden die verwijzen naar creatieve elementen die worden gehost op externe advertentieservers. U kunt het volgen pixel voor de advertenties omvatten.<!-- The bulksheet template for other ad servers says you can include 200. Which is it: 200 or 500? -->

Met de meegeleverde sjabloon kunt u [!DNL DoubleClick]- en [!DNL Flashtalking]-tagbladen of een handmatig ingevuld bestand uploaden.

Zie [Een advertentie maken](ad-create.md) om één advertentie van derden te maken.

>[!TIP]
>
> U kunt het beste advertenties van derden gebruiken die veilig via HTTPS worden aangeboden. URL&#39;s die via HTTPS worden aangeboden, beginnen met &quot;https.&quot;

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.

1. Klik op de naam van de campagne waarin de advertentie wordt opgenomen.

1. Klik boven de gegevenstabel op **[!UICONTROL Create]**. Klik in de sectie Typen toevoegen van het menu op **[!UICONTROL Bulk upload ads]**.

1. Selecteer de advertentieserver waarop de advertentie wordt gehost: *[!UICONTROL DoubleClick]*, *[!UICONTROL Flashtalking]* of *[!UICONTROL Other]*.

1. ([!DNL DoubleClick]- en [!DNL Flashtalking]-advertenties) Selecteer het type code dat u wilt gebruiken voor elk video-element en elk weergaveelement. De beschikbare opties variëren per advertentieserver.

1. (Toevoegen op alle advertentieservers behalve [!DNL DoubleClick] en [!DNL Flashtalking]) Klik **[!UICONTROL Download this template]** om een sjabloon te downloaden in [!DNL Microsoft Excel] spreadsheet (XLSX) formaat, dat u kunt vullen met advertentiegegevens en lokaal opslaan. De vereiste kolommen omvatten [!UICONTROL Ad Name], [!UICONTROL VAST/VPAID URL or Ad Tag], en [!UICONTROL Ad Types].

1. Klik **[!UICONTROL Upload]** en selecteer een dossier in .xlsx of .xls formaten van uw apparaat of netwerk.

   Voor [!DNL DoubleClick]- en [!DNL Flashtalking]-advertenties uploadt u onbewerkte tagbladen van de advertentieserver. Voor andere advertentieservers, gebruik het malplaatje u in Stap 3 downloadde.

1. Klik op **[!UICONTROL Start Building Ads]** nadat het uploaden is voltooid.

1. Bekijk de details en status van elke advertentie:

   1. Controleer de status van elke advertentie, die is gebaseerd op validatiecontroles van de geüploade tag.
   1. (Optioneel) Voer een van de volgende handelingen uit voor elke advertentie:
      * Als u een voorvertoning van een advertentie wilt weergeven, klikt u op ![play](/help/dsp/assets/play.png) in de advertentierij.
      * Als u de advertentiedetails wilt bewerken, klikt u op ![bewerken](/help/dsp/assets/edit.png), bewerkt u de details en klikt u op **Opslaan**.
      * Als u een advertentie wilt verwijderen, klikt u op **[!UICONTROL X]** in de rij met toevoegingen.

1. Klik **[!UICONTROL Create *N *Advertentie(s)]**.

1. Voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL Done]**.

   * (Indien een advertentie wordt afgewezen; (optioneel) U kunt als volgt de advertentierecord bewerken en de advertentie opnieuw ter controle verzenden:
      1. Klik op de naam van de advertentie.
      1. Bewerk de advertentie-instellingen.
      1. Klik op **[!UICONTROL Save & submit for review]**.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Een advertentie maken](ad-create.md)
>* [Beschikbare advertentietypen](ad-types.md)
>* [Advertentiespecificaties](/help/dsp/assets/ad-specs.pdf)

