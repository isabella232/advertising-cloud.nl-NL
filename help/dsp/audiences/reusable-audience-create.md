---
title: Een herbruikbaar publiek maken
description: Leer hoe u een herbruikbaar publiek kunt maken dat bestaat uit doelsegmenten en andere opgeslagen soorten publiek.
feature: DSP Audiences
exl-id: 48e3dc4c-6e2d-452c-8d69-7e6211d808e0
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Een herbruikbaar publiek maken

<!-- "Saved audience" is used in UI (where?), but "saved" is a state, not a type. "Reusable audience" sounds better in a description. "Audience template" isn't right, either, since it implies you can edit it on the fly to create a new, different audience. Some other term? -->

U kunt herbruikbare soorten publiek opslaan en beheren. Dit zijn groepen publiekssegmenten en zelfs andere opgeslagen soorten publiek, die u kunt gebruiken als doelen of uitsluitingen voor meerdere plaatsen.

1. Klik in het hoofdmenu op **[!UICONTROL Audiences]>[!UICONTROL All Audiences]**.

1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

1. Voer een unieke [!UICONTROL Audience Name] in.

1. (Optioneel) Schakel de optie **[!UICONTROL Share with all advertisers in my account]** uit.

   Wanneer u een publiek deelt, wordt het publiek beschikbaar als doel of uitsluiting voor alle adverteerders binnen de account. De afzonderlijke segmenten in het publiek zijn echter alleen beschikbaar voor gebruikers waarop de segmenten worden gedeeld. Als u bijvoorbeeld een publiek met Adobe Analytics-segmenten deelt met een adverteerder die niet is toegewezen aan dezelfde [!DNL Analytics]-account, wordt er geen voorvertoning van het segment weergegeven voor die adverteerder in dat publiek. Alleen de segmenten die voor die adverteerder beschikbaar zijn, worden in het publiek voorvertoond.

1. Klik op **[!UICONTROL Save]**.

1. Maak het publiek:

   >[!NOTE]
   >
   >Tijdens het samenstellen van het publiek worden gedetailleerde [gegevens voor de doelgrootte](audience-about.md) bijgewerkt in het rechterdeelvenster.

   * Ga als volgt te werk om de segmentlogica handmatig te maken met behulp van segmenten op de tabbladen [[!UICONTROL Third Party Segments], [!UICONTROL First Party Segments], [!UICONTROL Adobe Segments], [!UICONTROL Custom Segments] en [!UICONTROL Saved Audiences]](audience-settings.md).

      * Als u het eerste segment wilt toevoegen, zoekt u het segment in het linkerdeelvenster en schakelt u het selectievakje naast de segmentnaam in.

      * Een segment toevoegen aan een bestaande segmentgroep:

         1. Klik op de segmentgroep in het rechterdeelvenster.

         1. (Optioneel) Wijzig desgewenst de groeplogica in *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* of *[!UICONTROL Exclude All]*.

            *[!UICONTROL Exclude All]* is niet beschikbaar aan de eerste segmentgroep. Voor een publiek dat slechts uitsluitingen omvat, bouw dit publiek als *[!UICONTROL Include Any]* en dan, binnen een plaatsing, selecteer dat publiek van het Uitgesloten menu van het Publiek.

         1. Zoek het nieuwe segment in het linkerdeelvenster en schakel het selectievakje naast de segmentnaam in.

            De segmentgroep wordt automatisch bijgewerkt met het nieuwe segment.
      * Een nieuwe segmentgroep toevoegen:

         1. Klik **[!UICONTROL + New Group]** in het juiste paneel.

         1. (Optioneel) Wijzig desgewenst de logica tussen de vorige groep en de nieuwe groep in *[!UICONTROL And]* of *[!UICONTROL Or]*.

         1. Zoek de segmenten voor de nieuwe groep in het linkerdeelvenster en selecteer de selectievakjes naast de segmentnamen.

         1. (Optioneel) Wijzig desgewenst de groeplogica in *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* of *[!UICONTROL Exclude All]*.
   * Segmentlogica van een bestaand publiek gebruiken:

      1. Kopieer de segmentlogica van het bestaande publiek op een van de volgende manieren:

         * Houd in de weergave Alle soorten publiek de cursor boven de publiekstrij en klik vervolgens op **[!UICONTROL More]>[!UICONTROL Copy to Clipboard]**.

         * In de montages voor het bestaande publiek, bij de bovenkant van het paneel van de segmentlogica, klik **[!UICONTROL More]>[!UICONTROL Copy to Clipboard]**.

         * In een tekstredacteur, creeer manueel de segmentlogica gebruikend alfanumerieke segment IDs en [Booleaanse syntaxis](audience-segment-logic-syntax.md), en kopieer het aan uw klembord.
      1. Klik **[!UICONTROL paste in an audience rule to begin building]**, kleef de bestaande segmentlogica in het inputgebied, en klik dan **[!UICONTROL Apply]**.

         >[!NOTE]
         >
         >Als het publiek reeds om het even welke segmentlogica omvat, beschrijft het kleven in nieuwe segmentlogica de bestaande logica.




1. Klik op **[!UICONTROL Create]**.

>[!MORELIKETHIS]
>
>* [Over Audience Management](audience-about.md)
>* [Instellingen publiek](audience-settings.md)
>* [Syntaxis voor Audience Segment Logic](audience-segment-logic-syntax.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)
>* [Een aangepast segment maken en implementeren](custom-segment-create.md)
>* [Een  [!UICONTROL CCPA Opt-Out-of-Sale] segment maken en implementeren](ccpa-opt-out-segment-create.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

