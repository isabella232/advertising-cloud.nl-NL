---
title: Plaatsen dupliceren
description: Leer hoe u een of meer stages dupliceert.
feature: DSP Placements
exl-id: d22a61a8-4f1b-41ee-b4fb-3124bec81a2f
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Plaatsen dupliceren

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG placements, or all placements using private inventory? And anything else? -->

Dupliceer een of meer plaatsen om plaatsingen met gelijkaardige montages tot stand te brengen. U kunt:

* Meerdere duplicaten van plaatsingen maken
* Dubbele plaatsingen binnen de oorspronkelijke adverteerders en campagnes of binnen verschillende
* (Voor dubbele plaatsen binnen de originele campagnes) Naar keuze dupliceer de originele advertenties
* De status en vluchtdata van de nieuwe plaatsingen wijzigen

Zie &quot;[Wat is niet gedupliceerd](#placement-not-duplicated)&quot;voor een lijst van plaatsingsmontages die niet worden gedupliceerd.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.
1. Klik op de naam van de campagne.
1. Klik in het submenu op **[!UICONTROL Placements]**.
1. Voer een van de volgende handelingen uit:
   * Als u één plaatsing wilt dupliceren, klikt u op **[!UICONTROL ...]>[!UICONTROL Duplicate]** naast de pakketnaam.
   * Meerdere plaatsen dupliceren:
      1. Schakel het selectievakje naast elke plaatsing die u wilt dupliceren in.
      1. Klik op **[!UICONTROL Duplicate]** op de werkbalk voor bulkacties.
1. Geef de nieuwe plaatsingsinstellingen op:
   1. (Enkele plaatsen) Voer de nieuwe plaatsingsnaam in.
   1. Selecteer in het menu **[!UICONTROL Choose Package (Required)]** het bovenliggende pakket of **[!UICONTROL No package]*.
   1. (Optioneel) Wijzig de standaardinstellingen.

   De instellingen gelden voor alle geselecteerde plaatsingen.

   De nieuwe plaatsingen zijn standaard bedoeld voor het oorspronkelijke advertentietype, worden toegewezen aan de oorspronkelijke adverteerders en campagnes, hebben vluchtschema&#39;s die op de huidige dag beginnen, worden gepauzeerd en bevatten niet de originele advertenties.

   Wanneer u veelvoudige plaatsen creeert, worden de nieuwe plaatsingsnamen toegevoegd met een aantal, in opeenvolging, gebruikend de overeenkomst &lt;*original_placement_name #N*>, zoals &quot;Mijn Plaatsing #2.&quot;

1. Klik op **[!UICONTROL Submit]**.

## Wat is niet gedupliceerd {#placement-not-duplicated}

Alle instellingen van de originele plaatsingen worden gedupliceerd, behalve:

* Instellingen Experimenteren
* (Als u de vluchtdatums wijzigt) Aangepaste en geplande planning
* (Als u geen advertenties koppelt) Aangepaste weging en planning
* Standaard plaatsingen voor programmatic gewaarborgde (PG) overeenkomsten en plaatsingen voor [!UICONTROL Simple Ad Serving] overeenkomsten
* (Als u plaatsingen naar een andere campagne kopieert):
   * Geo-doelen
   * Gebeurtenispixels
   * Adds
   * [!DNL DoubleVerify Authentic Brand Safety]-segmenten op plaatsingsniveau (die de segmenten op adverteerderniveau overschrijven)

>[!MORELIKETHIS]
>
>* [Info over Plaatsingsbeheer](placement-about.md)
>* [Een plaatsing maken](placement-create.md)
>* [Een plaatsing bewerken](placement-edit.md)
>* [Plaatsingsinstellingen](placement-settings.md)

