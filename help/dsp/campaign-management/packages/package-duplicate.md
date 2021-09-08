---
title: Een pakket dupliceren
description: Leer hoe u een pakket dupliceert.
feature: Packages
exl-id: 4c37883f-5feb-4513-9573-ed4e32606132
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Een pakket dupliceren

Dupliceer een pakket om een pakket met gelijkaardige montages tot stand te brengen. U kunt:

* Het pakket dupliceren binnen de oorspronkelijke adverteerder en campagne of binnen verschillende
* U kunt desgewenst de plaatsen in het pakket dupliceren
* (Voor gedupliceerde pakketten in de oorspronkelijke campagnes) Dupliceer optioneel de oorspronkelijke advertenties en de gebeurtenispixels op plaatsingsniveau
* De vluchtdatums van het nieuwe pakket wijzigen

Zie &quot;[Wat is niet gedupliceerd](#package-not-duplicated)&quot;voor een lijst van plaatsingsmontages die niet worden gedupliceerd.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.
1. Klik op de naam van de campagne om de weergave [!UICONTROL Packages] te openen.
1. Klik naast de pakketnaam op **[!UICONTROL ...]>[!UICONTROL Duplicate]**.
1. Geef de nieuwe pakketinstellingen op:
   1. Voer de nieuwe pakketnaam in.
   1. (Optioneel) Wijzig de standaardinstellingen.

      Standaard:

      * Het nieuwe pakket wordt toegewezen aan de oorspronkelijke adverteerder en campagne.
      * Het nieuwe pakket wordt actief op de huidige dag.<!-- and the flight continues for NN  days. -->
      * Plaatsen in het originele pakket worden gekopieerd naar het nieuwe pakket.
      * De advertenties en de gebeurtenispixels op plaatsingsniveau worden niet naar het nieuwe pakket gekopieerd.
1. Klik op **[!UICONTROL Submit]**.

## Wat is niet gedupliceerd {#package-not-duplicated}

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
>* [Info over Pakketbeheer](package-about.md)
>* [Een pakket maken](package-create.md)
>* [Een pakket bewerken](package-edit.md)
>* [Pakketinstellingen](package-settings.md)

