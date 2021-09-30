---
title: Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken
description: Verwijs naar de beschikbare voorbiedingsfilters op plaatsingsniveau en zie hoe u deze kunt gebruiken.
feature: DSP Optimization
exl-id: c699e970-84ca-429b-8062-81804e6c9f21
source-git-commit: 75ec6f54271542d56e0d16fbb7aa92ebcf00d765
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken

| Filter voor vooraf bieden | Beschrijving | Wanneer moet u dit filter gebruiken? |
| ---------------| ----------- | ---------------------- |
| [!UICONTROL Click Through Rate] | Hiermee stelt u een minimale voorspellingsdrempel in voor de waarschijnlijkheid dat een veiling een klikdoorhaling oplevert. Als u de drempel bijvoorbeeld instelt op 0,1%, biedt u geen bod op een veiling tenzij de voorspelde waarschijnlijkheid van een klik groter is dan of gelijk is aan 0,1%.<br><br><b>Opmerking:</b> Filters worden toegepast vóór optimalisatiedoelen. Als gevolg hiervan kunnen zeer strikte filters uitgaven voorkomen. | Gebruik wanneer u een minimumdoel KPI voor klikthrough tarief (CTR) hebt en uw begroting niet wilt uitgeven wanneer CTR onder de drempel is. Dit filter kan vrij restrictief zijn, zodat is het belangrijk om realistische doelstellingen te plaatsen. Afhankelijk van andere beperkingen op de plaatsing, is een doel van 0,03 - 07% over het algemeen een goed uitgangspunt. U kunt dit naar wens op siteniveau optimaliseren om de metingen te verbeteren.<br><br>Als uw doel een minimum CTR en best mogelijke CPM is te bereiken, dan is de geadviseerde opstelling een  [!UICONTROL Click Through Rate] filter met het optimalisatiedoel &quot;[!UICONTROL Lowest CPM].&quot;te combineren. Als uw doel een maximum CPM zonder echt voordeel voor het overbereiken, en een minimum CTR is, dan kan het verpakken van een [!UICONTROL Click Through Rate] filter met het optimalisatiedoel &quot;[!UICONTROL Always Max Bid + Highest CTR]&quot;geschikter zijn. |
| [!UICONTROL 100% Completion Rate] | Hiermee stelt u een vereiste minimale voltooiingsfactor in waaraan moet worden voldaan voordat je op een bepaald idee biedt. | Gebruik dit filter wanneer het belangrijkste doel van de campagne voltooiingspercentages is. Factor in andere het richten parameters, maar 65% is het geadviseerde beginnende percentage. |
| [!UICONTROL Player Size - Adobe] | Hiermee stelt u een vereiste minimale spelergrootte in met behulp van gegevens uit Advertising Cloud DSP. Je biedt een indruk wanneer aan de [!UICONTROL Player Size]-drempel wordt voldaan. | Gebruik deze optie om te zorgen dat u de spelervoorraad voor een volledige aflevering aanbiedt met behulp van gegevens uit DSP. |
| [!UICONTROL Player Size 3rdParty (Moat/IAS)] | Hiermee stelt u een vereiste minimale spelergrootte in met gegevens van [!DNL Moat] of [!DNL Integral Ad Science] ([!DNL IAS]). Je biedt een indruk wanneer aan de [!UICONTROL Player Size]-drempel wordt voldaan. | Gebruik deze optie om ervoor te zorgen dat u de spelervoorraad voor volledige uitlevering aanbiedt met behulp van platformbrede [!DNL Moat]- of [!DNL IAS]-gegevens.<br><br><b>Opmerking:</b> gebruik dit filter alleen wanneer de campagne is geconfigureerd voor gebruik  [!DNL Moat] of  [!DNL IAS] gegevens. |
| [!UICONTROL Viewability Adobe (MRC or [!DNL GroupM])] | Hiermee stelt u een minimaal weergavepercentage in met Advertising Cloud DSP-weergavegetallen en -metingen. Je kunt een bod uitbrengen als de opgegeven drempel is bereikt.<br><br><b>Opmerkingen:</b><ul><li>Als de [!UICONTROL Viewability Sensitivity] het plaatsen van de campagne &quot;[!UICONTROL Standard (50% of ad in view for 2 consecutive seconds)],&quot;is, dan wordt [!DNL Media Rating Council] (MRC) viewability metingsnorm gebruikt voor de campagne. Als de [!UICONTROL Viewability Sensitivity]-instelling &quot;[!UICONTROL Strict (100% of ad in view & audio on for 50% duration)]&quot; is, wordt de [!DNL GroupM]-standaard voor de meting van de weergavekwaliteit gebruikt voor de campagne.</li><li>Adobe-meetdefinities verschillen van definities van derden, zodat er kleine verschillen kunnen zijn met gegevens van derden.</li></ul> | De beste manier is om het optimalisatiedoel en om het even welke vooraf biedende filtermontages met de het plaatsen van [!UICONTROL Viewability Sensitivity] van de campagne aan te passen. |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
>* [Campagne-instellingen](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)

