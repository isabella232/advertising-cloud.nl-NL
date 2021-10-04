---
title: Handmatig details van deal-id maken
description: Leer hoe te om details voor een identiteitskaart van de Overeenkomst manueel in te gaan.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: cd9763a7-99d4-4881-9df9-b4e24c55be0f
source-git-commit: 7e2a52e7b0d91f9206cd6e9a6ffb41a8399abf00
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Handmatig details van deal-id maken

1. Klik in het hoofdmenu op **[!UICONTROL Inventory]> [!UICONTROL Deals].**

1. Klik boven de gegevenstabel op **[!UICONTROL Create]** en selecteer **[!UICONTROL Deal ID]**.

1. Voer de [deal-instellingen](deal-id-settings.md) in:

   1. In de [!UICONTROL Deal ID basics] sectie, specificeer de overeenkomstendetails en adverteerders die tot de overeenkomst kunnen toegang hebben. Voor gegarandeerde deals moet u ook de geplande vluchtdata en de geschatte indrukken specificeren, alleen voor traceringsdoeleinden.

   1. (Alleen gebruikers van beheerders; (optioneel) Bewerk in de sectie [!UICONTROL Technical] de standaardinstellingen.

   1. Klik op **[!UICONTROL Save]**.

1. (Gegarandeerde overeenkomsten slechts) selecteer de advertenties die voor de overeenkomst zullen worden gebruikt en creeer een standaard programmatic gewaarborgde plaatsing (PG).

   Standaard PG-plaatsingen zorgen ervoor dat je deal altijd een bod retourneert voor elke biedaanvraag. Als u geen standaardplaatsing van PG creeert, dan zullen om het even welke plaatsen die de overeenkomst richten geen biedingen plaatsen tenzij zij opstelling correct zijn. U moet altijd een standaard-PG-plaatsing maken. In de [!UICONTROL Placements] mening, hebben de gebrek PG plaatsingen een [!UICONTROL Sub-type] kolomwaarde van &quot;[!UICONTROL PG Default].&quot;

   U kunt naar keuze de overeenkomst als inventarisdoel in extra plaatsingen gebruiken maar moet hen opstelling correct om biedingen te plaatsen.

   1. In de [!UICONTROL Ad & Campaign Selection] montages, selecteer de advertenties die voor de overeenkomst zullen worden gebruikt:

      1. Selecteer de adverteerder, de campagne en het type advertentie. Selecteer desgewenst een advertentiestatus waarmee de advertenties moeten worden gefilterd.

      1. Van de lijst van beschikbare advertenties, selecteer de controledoos naast elke advertentie die voor de overeenkomst zal worden gebruikt.

      1. Klik op **[!UICONTROL Apply]**.
   1. In het scherm met plaatsingsinstellingen:

      1. Voer de plaatsingsnaam in.

      1. (Facultatief) geef [plaatsingsmontages ](/help/dsp/campaign-management/placements/placement-settings.md) uit, met inbegrip van het beschrijven van het standaardbod, dat automatisch met de CPM waarde van de overeenkomst wordt bevolkt; het wijzigen van het datumbereik; of meer advertenties toevoegen.

      De overeenkomst wordt automatisch gericht in de sectie van de Streefcijfers van de Inventaris. Alle andere doelopties zijn niet van toepassing.

      1. Klik op **[!UICONTROL Create placement]**.



Nadat u de overeenkomst creeert, kunt u de overeenkomst als inventarisdoel voor veelvoudige plaatsen gebruiken.

>[!NOTE]
>
> U te hoeven niet om de overeenkomstenmarkering naar de uitgever voor controle te verzenden.

>[!TIP]
>
>* In [!UICONTROL Inventory] > [!UICONTROL Deals] mening, toont [!UICONTROL Pacing & Budget] kolom hoe de overeenkomst aan de gespecificeerde vluchtdatum en imperiatiedoel past.
>
>* Als de levering onderaan of overpakking is, contacteer uw uitgever om aan te passen hoeveel volume het door de overeenkomst verzendt.


>[!MORELIKETHIS]
>
>* [Instellingen voor handmatige deal-id](deal-id-settings.md)
>* [Opstelling een Programma Gegarandeerde Overeenkomst](programmatic-guaranteed-set-up.md)
>* [Verzend een Advertentie voor een Programma Gegarandeerde Overeenkomst met [!DNL FreeWheel]](freewheel-submit.md)
>* [Ongeveer Programma Gegarandeerde Overeenkomsten](programmatic-guaranteed-about.md)

<!-- >* [Specify Placements and Ads for a Private Deal](private-deal-attach-placements.md)-->