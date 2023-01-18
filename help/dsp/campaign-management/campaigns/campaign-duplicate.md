---
title: Een campagne dupliceren
description: Leer hoe u een campagne dupliceert.
feature: DSP Campaigns
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Een campagne dupliceren

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG placements, or all placements using private inventory? And anything else? -->

Dupliceer een campagne om een nieuwe campagne met gelijkaardige montages tot stand te brengen. U kunt:

* De campagne dupliceren voor de oorspronkelijke adverteerder of voor een andere
* De originele pakketten en plaatsen eventueel dupliceren
* De vluchtdata van de nieuwe campagne wijzigen

Zie &quot;[Wat is niet gedupliceerd](#campaign-not-duplicated)&quot; voor een lijst met plaatsingsinstellingen die niet worden gedupliceerd.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.

1. Klik naast de naam van de campagne op **... >[!UICONTROL Duplicate]**.

1. Geef de nieuwe instellingen voor de campagne op:

   1. Voer de nieuwe naam van de campagne en de einddatum van de vlucht in.

   1. (Optioneel) Wijzig de standaardinstellingen.

      De nieuwe campagne wordt standaard toegewezen aan de oorspronkelijke adverteerder, heeft een vliegschema dat op de huidige dag begint en de originele pakketten en plaatsen bevat.

1. Klik op **[!UICONTROL Submit]**.

## Wat is niet gedupliceerd {#campaign-not-duplicated}

Alle instellingen van de originele plaatsingen worden gedupliceerd, behalve:

* Instellingen Experimenteren
* (Als u de vluchtdatums wijzigt) Aangepaste en geplande planning
* (Als u geen advertenties koppelt) Aangepaste weging en planning
* Standaardplaatsingen voor door het programma gegarandeerde deals en plaatsingen voor [!UICONTROL Simple Ad Serving] deals
* (Als u plaatsingen naar een andere campagne kopieert):
   * Geo-doelen
   * Gebeurtenispixels
   * Adds
   * Plaatsingsniveau [!DNL DoubleVerify Authentic Brand Safety] segmenten (die de segmenten op adverteerderniveau overschrijven)

>[!MORELIKETHIS]
>
>* [Informatie over Campaign Management](campaign-about.md)
>* [Een campagne maken](campaign-create.md)
>* [Een campagne bewerken](campaign-edit.md)
>* [Campagne-instellingen](campaign-settings.md)

