---
title: Een pakket dupliceren
description: Leer hoe u een pakket dupliceert.
feature: DSP Packages
exl-id: 4c37883f-5feb-4513-9573-ed4e32606132
source-git-commit: 5ed402a7c83072a7af6a06757050486c6d7d7080
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Een pakket dupliceren

Dupliceer een pakket om een pakket met gelijkaardige montages tot stand te brengen. U kunt:

* Het pakket dupliceren binnen de oorspronkelijke adverteerder en campagne of binnen verschillende
* U kunt desgewenst de plaatsen in het pakket dupliceren
* (Voor gedupliceerde pakketten in de oorspronkelijke campagnes) Dupliceer optioneel de oorspronkelijke advertenties en de gebeurtenispixels op plaatsingsniveau
* De vluchtdatums van het nieuwe pakket wijzigen

Zie &quot;[Wat is niet gedupliceerd](#package-not-duplicated)&quot; voor een lijst met plaatsingsinstellingen die niet worden gedupliceerd.

1. Klik in het hoofdmenu op **[!UICONTROL Campaigns]**.
1. Klik op de naam van de campagne om het dialoogvenster [!UICONTROL Packages] weergeven.
1. Klik naast de pakketnaam op  **[!UICONTROL ...]>[!UICONTROL Duplicate]**.
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
* Standaardplaatsingen voor door het programma gegarandeerde deals en plaatsingen voor [!UICONTROL Simple Ad Serving] deals
* (Als u plaatsingen naar een andere campagne kopieert):
   * Geo-doelen
   * Gebeurtenispixels
   * Adds
   * Plaatsingsniveau [!DNL DoubleVerify Authentic Brand Safety] segmenten (die de segmenten op adverteerderniveau overschrijven)

>[!MORELIKETHIS]
>
>* [Info over Pakketbeheer](package-about.md)
>* [Een pakket maken](package-create.md)
>* [Een pakket bewerken](package-edit.md)
>* [Het Wijzigingslogboek voor een pakket weergeven](package-change-log.md)
>* [Pakketinstellingen](package-settings.md)

