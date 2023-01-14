---
title: Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken
description: Verwijs naar de beschikbare voorbiedingsfilters op plaatsingsniveau en zie hoe u deze kunt gebruiken.
feature: DSP Optimization
exl-id: c699e970-84ca-429b-8062-81804e6c9f21
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken

| Filter voor vooraf bieden | Beschrijving | Wanneer moet u dit filter gebruiken? |
| ---------------| ----------- | ---------------------- |
| [!UICONTROL Click Through Rate] | Hiermee stelt u een minimale voorspellingsdrempel in voor de waarschijnlijkheid dat een veiling leidt tot doorklikken. Als u bijvoorbeeld de drempel instelt op 0,1%, biedt u alleen op een veiling een bod uit als de voorspelde waarschijnlijkheid van een klik groter is dan of gelijk is aan 0,1%.<br><br><b>Opmerking:</b> Filters worden toegepast vóór optimalisatiedoelen. Als gevolg hiervan kunnen zeer strikte filters uitgaven voorkomen. | Gebruik wanneer u een minimumKPI-doel voor doorkliktarief (CTR) hebt en uw budget niet wilt besteden wanneer CTR onder de drempel is. Dit filter kan vrij restrictief zijn, zodat is het belangrijk om realistische doelstellingen te plaatsen. Afhankelijk van andere beperkingen op de plaatsing, is een doel van 0,03 - 07% over het algemeen een goed uitgangspunt. U kunt dit naar wens op siteniveau optimaliseren om de metingen te verbeteren.<br><br>Als uw doel een minimum CTR en best mogelijke CPM is te bereiken, dan is de geadviseerde opstelling om een [!UICONTROL Click Through Rate] filteren met de optimalisatiedoelstelling &quot;[!UICONTROL Lowest CPM].&quot; Als uw doel een maximum CPM zonder echt voordeel voor het overbereiken, en een minimum CTR is, dan het verpakken van een [!UICONTROL Click Through Rate] filteren met de optimalisatiedoelstelling &quot;[!UICONTROL Always Max Bid + Highest CTR]&quot;kan geschikter zijn. |
| [!UICONTROL 100% Completion Rate] | Hiermee stelt u een vereiste minimale voltooiingsfactor in waaraan moet worden voldaan voordat je op een bepaald idee biedt. | Gebruik dit filter wanneer het belangrijkste doel van de campagne voltooiingspercentages is. Factor in andere het richten parameters, maar 65% is het geadviseerde beginnende percentage. |
| [!UICONTROL Player Size - Adobe] | Hiermee stelt u een vereiste minimale spelergrootte in met behulp van gegevens uit DSP. Je biedt op een indruk wanneer de [!UICONTROL Player Size] drempelwaarde is bereikt. | Gebruik deze optie om te zorgen dat u de spelervoorraad voor een volledige aflevering aanbiedt met behulp van gegevens uit DSP. |
| [!UICONTROL Player Size 3rdParty (Moat/IAS)] | Hiermee wordt een vereiste minimale spelergrootte ingesteld, waarbij gegevens worden gebruikt van [!DNL Moat] of [!DNL Integral Ad Science] ([!DNL IAS]). Je biedt op een indruk wanneer de [!UICONTROL Player Size] drempelwaarde is bereikt. | Gebruik deze optie om te zorgen dat u op platformbrede schaal een volledige-episodespelervoorraad aanbiedt [!DNL Moat] of [!DNL IAS] gegevens.<br><br><b>Opmerking:</b> Gebruik dit filter slechts wanneer de campagne wordt gevormd om te gebruiken [!DNL Moat] of [!DNL IAS] gegevens. |
| [!UICONTROL Viewability Adobe (MRC or [!DNL GroupM])] | Hiermee stelt u een minimaal weergavepercentage in met DSP weergavegetallen en metingen. Je kunt een bod uitbrengen als de opgegeven drempel is bereikt.<br><br><b>Opmerkingen:</b><ul><li>Als de campagne [!UICONTROL Viewability Sensitivity] instelling is &quot;[!UICONTROL Standard (50% of ad in view for 2 consecutive seconds)],&quot; dan de [!DNL Media Rating Council] (MRC) de norm van de viewability meting wordt gebruikt voor de campagne. Als de [!UICONTROL Viewability Sensitivity] instelling is &quot;[!UICONTROL Strict (100% of ad in view & audio on for 50% duration)],&quot; dan de [!DNL GroupM] voor de campagne wordt de standaard voor de meting van de gezichtsvermogen gebruikt.</li><li>Adobe-meetdefinities verschillen van definities van derden, zodat er kleine verschillen kunnen zijn met gegevens van derden.</li></ul> | De beste manier is om de optimalisatiedoelstelling en eventuele filterinstellingen vóór het bieden te laten aansluiten op de campagne [!UICONTROL Viewability Sensitivity] instellen. |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
>* [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)

