---
title: Een herbruikbaar publiek maken
description: Leer hoe u een herbruikbaar publiek kunt maken dat bestaat uit doelsegmenten en andere opgeslagen soorten publiek.
feature: DSP Audiences
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Een herbruikbaar publiek maken

<!-- "Saved audience" is used in UI (where?), but "saved" is a state, not a type. "Reusable audience" sounds better in a description. "Audience template" isn't right, either, since it implies you can edit it on the fly to create a new, different audience. Some other term? -->

U kunt herbruikbare soorten publiek opslaan en beheren. Dit zijn groepen publiekssegmenten en zelfs andere opgeslagen soorten publiek, die u kunt gebruiken als doelen of uitsluitingen voor meerdere plaatsen.

1. Klik in het hoofdmenu op **[!UICONTROL Audiences]>[!UICONTROL All Audiences]**.

1. Klik boven de gegevenstabel op **[!UICONTROL Create]**.

1. Voer een unieke waarde in [!UICONTROL Audience Name].

1. (Optioneel) Schakel de optie uit om **[!UICONTROL Share with all advertisers in my account]**.

   Wanneer u een publiek deelt, wordt het publiek beschikbaar als doel of uitsluiting voor alle adverteerders binnen de account. De afzonderlijke segmenten in het publiek zijn echter alleen beschikbaar voor gebruikers waarop de segmenten worden gedeeld. Als u bijvoorbeeld een publiek deelt dat Adobe Analytics-segmenten bevat, met een adverteerder die niet aan dezelfde groep is toegewezen [!DNL Analytics] dan zal het segment geen voorvertoning voor die adverteerder in dat publiek weergeven. Alleen de segmenten die voor die adverteerder beschikbaar zijn, worden in het publiek voorvertoond.

1. Klik op **[!UICONTROL Save]**.

1. Maak het publiek:

   >[!NOTE]
   >
   >Tijdens het samenstellen van het publiek, gedetailleerd [gegevens over doelgrootte](audience-about.md) wordt bijgewerkt in het rechterdeelvenster

   * Om de segmentlogica manueel tot stand te brengen, gebruikend segmenten beschikbaar op [[!UICONTROL Third Party Segments], [!UICONTROL First Party Segments], [!UICONTROL Adobe Segments], [!UICONTROL Custom Segments], en [!UICONTROL Saved Audiences] tabs](audience-settings.md), doe het volgende.

      * Als u het eerste segment wilt toevoegen, zoekt u het segment in het linkerdeelvenster en schakelt u het selectievakje naast de segmentnaam in.

      * Een segment toevoegen aan een bestaande segmentgroep:

         1. Klik op de segmentgroep in het rechterdeelvenster.

         1. (Optioneel) Wijzig de logica van de groep in *[!UICONTROL Include Any]*, *[!UICONTROL Include All]*, of *[!UICONTROL Exclude All]*, indien nodig.

            *[!UICONTROL Exclude All]* is niet beschikbaar aan de eerste segmentgroep. Voor een publiek dat alleen uitsluitingen bevat, bouwt u dit publiek als *[!UICONTROL Include Any]* en selecteer vervolgens binnen een plaatsing dat publiek in het menu Uitgesloten soorten publiek.

         1. Zoek het nieuwe segment in het linkerdeelvenster en schakel het selectievakje naast de segmentnaam in.

            De segmentgroep wordt automatisch bijgewerkt met het nieuwe segment.
      * Een nieuwe segmentgroep toevoegen:

         1. Klikken **[!UICONTROL + New Group]** in het rechterdeelvenster.

         1. (Optioneel) Wijzig de logica tussen de vorige groep en de nieuwe groep in *[!UICONTROL And]* of *[!UICONTROL Or]*, indien nodig.

         1. Zoek de segmenten voor de nieuwe groep in het linkerdeelvenster en selecteer de selectievakjes naast de segmentnamen.

         1. (Optioneel) Wijzig de logica van de groep in *[!UICONTROL Include Any]*, *[!UICONTROL Include All]*, of *[!UICONTROL Exclude All]*, indien nodig.
   * Segmentlogica van een bestaand publiek gebruiken:

      1. Kopieer de segmentlogica van het bestaande publiek op een van de volgende manieren:

         * Houd in de weergave Alle soorten publiek de cursor boven de personenrij en klik vervolgens op **[!UICONTROL More]>[!UICONTROL Copy to Clipboard]**.

         * Klik in de instellingen voor het bestaande publiek boven aan het deelvenster voor segmentlogica op **[!UICONTROL More]>[!UICONTROL Copy to Clipboard]**.

         * Maak in een teksteditor handmatig de segmentlogica met alfanumerieke segment-id&#39;s en [Booleaanse syntaxis](audience-segment-logic-syntax.md)en kopieer deze naar het klembord.
      1. Klikken **[!UICONTROL paste in an audience rule to begin building]** plakt u de bestaande segmentlogica in het invoerveld en klikt u vervolgens op **[!UICONTROL Apply]**.

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
>* [Een [!UICONTROL CCPA Opt-Out-of-Sale] Segment](ccpa-opt-out-segment-create.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

