---
title: Problemen oplossen
description: Verwijzing gemeenschappelijke prestatieskwesties en zie hoe te om hen problemen op te lossen.
feature: Optimization
exl-id: adb32257-dede-4623-9840-33221c218443
source-git-commit: 185fc7d79798a0a3a9ad5829b701aeb53a4a47c1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Problemen oplossen

| Probleem | Mogelijke oorzaak | Te nemen handelingen |
| --- | --- | --- |
| Geen uitgaven voor plaatsing | De plaatsing bevat geen advertenties en/of de advertenties zijn niet actief. | Controleer of alle verwachte advertenties zijn gekoppeld aan de plaatsing en zijn goedgekeurd en actief.<br><br>Zie ook of de plaatsing een aangepast advertentieschema bevat, waardoor de vliegperiode voor elke advertentie kan worden beperkt. Als u het advertentieschema voor een plaatsing wilt weergeven vanuit de weergave Plaatsen, klikt u op **[!UICONTROL ...]>[!UICONTROL Ad schedule]** naast de plaatsingsnaam. |
|  | De betrokken datums vallen niet binnen de geconfigureerde vluchtdatums. | Controleer of de vluchtdatums geldig zijn op de campagne, het pakket en het plaatsingsniveau &#x200B; s. |
|  | Het begrotingsdoel is bereikt en/of is niet hoog genoeg. | Controleer de budgetinstellingen op de campagne-, pakket- en plaatsingsniveaus. |
|  | De rekening heeft niet genoeg financiering. | Ga naar **[!UICONTROL Settings]>[!UICONTROL Account]** en bekijk de hoeveelheid [!UICONTROL Usable Funds] om te zien of uw account voldoende is gefinancierd. Neem contact op met uw accountmanager van Adobe als u meer middelen wilt toevoegen. |
|  | Er is geen voorraad beschikbaar. | Controleer of de opgegeven inventarisbronnen ([!UICONTROL Public], [!UICONTROL Private] of [!UICONTROL On Demand]):<ul><li>Correcte instelling.</li><li>Actief en via veilingen verzenden.</li><li>Compatibel met het toepasselijke advertentie- en plaatsingstype.</li></ul><br>Als de inventarisbronnen allemaal geldig en actief zijn, richt u zich waar mogelijk op aanvullende of alle inventarisbronnen. |
|  | Er zijn geen gebruikers beschikbaar. | Controleer of de opgegeven doelgroepen voldoende actieve gebruikers bevatten. Als ze dat niet doen, breidt u de doelen uit door meer publiek toe te voegen. |
| Lage uitgaven voor plaatsing | In het gedeelte [!UICONTROL Non Bids] van het rapport voor plaatsingsdiagnostiek worden mogelijke redenen getoond waarom de plaatsing niet is geboden. | [Bekijk het  [!UICONTROL Non Bids] ](/help/dsp/campaign-management/reports/placement-diagnostics.md) rapport om te begrijpen waarom er niet is geboden.   <!-- add link/edit text when file available: See the [in-depth guide to possible Non-Bid Reasons (NBR)](link) for more information. --> |
|  | Voor de plaatsing worden [filters voor vooraf bieden gebruikt](/help/dsp/campaign-management/placements/placement-settings.md) om bieden te beperken. | Verlaag de drempelwaarden van de filters voor het vooraf bieden met 5% om de balans tussen besteding en prestaties te beoordelen. <!-- wording? and are users just supposed to manually monitor whether it makes a difference? --><br><br>Houd er rekening mee dat het gebruik van meerdere plaatsingsdoelen, zoals voorbiedingsfilters, geo&#39;s, voorraad en soorten publiek, het bieden en uitgeven van objecten cumulatief kan beperken. |
|  | De prijs van de plaatsing is laag. | Verhoog [!UICONTROL Max Bid] om het win tarief te verbeteren.<br><br><b>OPMERKING:</b> De inventarisprijzen kunnen variëren afhankelijk van de bestemming van de plaatsing.<br><br>Een 10%-win-percentage wordt als gezond beschouwd. |
|  | Er is een laag aantal voorraden beschikbaar. | Indien mogelijk aanvullende of alle inventarisbronnen als doel instellen.<br><br>Houd er rekening mee dat het gebruik van meerdere plaatsingsdoelen, zoals voorbiedingsfilters, geo&#39;s, voorraad en soorten publiek, het bieden en uitgeven van objecten cumulatief kan beperken. |
|  | Er zijn weinig gebruikers beschikbaar. | Controleer of de opgegeven doelgroepen voldoende actieve gebruikers bevatten. Als ze dat niet doen, breidt u de doelen uit door meer publiek toe te voegen.<br><br>Houd er rekening mee dat het gebruik van meerdere plaatsingsdoelen, zoals voorbiedingsfilters, geo&#39;s, voorraad en soorten publiek, het bieden en uitgeven van objecten cumulatief kan beperken. |
|  | Het pakket bevat een groot aantal actieve plaatsingen. | Het aantal actieve stages binnen het pakket verminderen of het totale budget verhogen.<br><br>Als het pakket veel plaatsen maar niet genoeg budget heeft, kan DSP mogelijk niet genoeg budget aan elke plaatsing toewijzen. Elke plaatsing moet de mogelijkheid hebben om ten minste 2 USD/dag te besteden. Als uw pakket bijvoorbeeld een budget van 10 dollar per dag heeft, kunt u het beste vijf of minder plaatsen opnemen. &#x200B; |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md)

