---
title: Handmatig details van deal-id maken
description: Leer hoe te om details voor een identiteitskaart van de Overeenkomst manueel in te gaan.
feature: DSP Private Inventory, DSP Deal IDs
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Handmatig details van deal-id maken

1. Klik in het hoofdmenu op **[!UICONTROL Inventory]> [!UICONTROL Deals].**

1. Klik boven de gegevenstabel op **[!UICONTROL Create]** en selecteer vervolgens **[!UICONTROL Deal ID]**.

1. Voer de [deal-instellingen](deal-id-settings.md):

   1. In de [!UICONTROL Deal ID basics] van de sectie, specificeer de overeenkomstendetails en adverteerders die tot de overeenkomst kunnen toegang hebben. Voor gegarandeerde deals moet u ook de geplande vluchtdata en het geschatte aantal indrukken specificeren, alleen voor traceringsdoeleinden.

   1. (Alleen gebruikers van beheerders; (optioneel) In de [!UICONTROL Technical] de standaardinstellingen naar wens bewerken.

   1. Klik op **[!UICONTROL Save]**.

1. (Gegarandeerde overeenkomsten slechts) selecteer de advertenties die voor de overeenkomst te gebruiken en een standaard programmatic gegarandeerde plaatsing (PG) tot stand te brengen.

   De standaardPG plaatsingen zorgen ervoor dat uw overeenkomst altijd een bod voor elke biedingsverzoek terugkeert. Als u geen standaardplaatsing van PG creeert, dan om het even welke plaatsen die de overeenkomst richten plaatsen geen biedingen tenzij zij opstelling correct zijn. U moet altijd een standaard-PG-plaatsing maken. In de [!UICONTROL Placements] weergave, standaard-PG-plaatsingen hebben een [!UICONTROL Sub-type] kolomwaarde van &quot;[!UICONTROL PG Default].&quot;

   U kunt naar keuze de overeenkomst als inventarisdoel in extra plaatsingen gebruiken maar moet hen opstelling correct om biedingen te plaatsen.

   1. In de [!UICONTROL Ad & Campaign Selection] montages, selecteer de advertenties die voor de overeenkomst zullen worden gebruikt:

      1. Selecteer de adverteerder, de campagne en het type advertentie. Selecteer desgewenst een advertentiestatus waarmee de advertenties moeten worden gefilterd.

      1. Van de lijst van beschikbare advertenties, selecteer de controledoos naast elke advertentie om voor de overeenkomst te gebruiken.

      1. Klik op **[!UICONTROL Apply]**.
   1. In het scherm met plaatsingsinstellingen:

      1. Voer de plaatsingsnaam in.

      1. (Optioneel) Bewerk de [plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md), met inbegrip van het overschrijven van het standaardbod, dat automatisch wordt gevuld met de CPM-waarde van de transactie; het wijzigen van het datumbereik; of meer advertenties toevoegen.

      De overeenkomst wordt automatisch gericht in de sectie van de Streefcijfers van de Inventaris. Alle andere doelopties zijn niet van toepassing.

      1. Klik op **[!UICONTROL Create placement]**.



Nadat u de overeenkomst creeert, kunt u de overeenkomst als inventarisdoel voor veelvoudige plaatsen gebruiken.

>[!NOTE]
>
> U te hoeven niet om de overeenkomstenmarkering naar de uitgever voor controle te verzenden.

>[!TIP]
>
>* In de [!UICONTROL Inventory] > [!UICONTROL Deals] de [!UICONTROL Pacing & Budget] de kolom toont hoe de overeenkomst aan het gespecificeerde vliegdatum en imperiatiedoel past.
>
>* Als de levering onderaan of overpakking is, contacteer uw uitgever om aan te passen hoeveel volume het door de overeenkomst verzendt.


>[!MORELIKETHIS]
>
>* [Instellingen voor handmatige deal-id](deal-id-settings.md)
>* [Opstelling een Programma Gegarandeerde Overeenkomst](programmatic-guaranteed-set-up.md)
>* [Verzend een Advertentie voor een Programma Gegarandeerde Overeenkomst met [!DNL FreeWheel]](freewheel-submit.md)
>* [Ongeveer Programma Gegarandeerde Overeenkomsten](programmatic-guaranteed-about.md)

<!-- >* [Specify Placements and Ads for a Private Deal](deal-id-attach-placements.md)-->