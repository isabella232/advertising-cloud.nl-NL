---
title: Gevallen gebruiken
description: Meer informatie over gebruiksgevallen voor het delen van Advertising Cloud DSP-mediagegevens met Audience Manager
feature: Integration with Adobe Audience Manager
source-git-commit: 3980af19efa785c437cacbf479ca3eabbed73b1b
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Gevallen gebruiken voor het vastleggen van belichtingsgegevens van media in Adobe Audience Manager

*Adverteerders met alleen Advertising Cloud DSP*

*Adverteerders met alleen Advertising Cloud-Adobe Audience Manager-integratie*

Hieronder vindt u enkele manieren waarop u de belichtingsgegevens van Advertising Cloud DSP-media kunt vastleggen <!-- ad impression data? --> in de Audience Manager.

## Recente- en frequentiebeheer

Door impliciete gegevens vast te leggen in Audience Manager kunt u uw frequentiebeheer verbeteren door segmenten van gebruikers te maken die zijn blootgesteld aan een bepaalde advertentie of campagne. U kunt deze segmenten gebruiken voor het opgeven van doelen als u de frequentie wilt verhogen of voor het onderdrukken van advertenties als u de frequentie wilt beperken.

Ook, met Audience Manager [!DNL Segment Builder]kunt u [recensie- en frequentiecontroles](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/recency-and-frequency.html) aan [op regels gebaseerde kenmerken](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html) die actioneerbare signalen bevatten. Zo kunt u bijvoorbeeld het aantal keren beperken dat een gebruiker een bepaalde creatieve vertoning weergeeft in een mediacampagne. Lees &quot;[Onmiddellijke ondersteuning voor apparaten](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/profile-merge-rules/instant-cross-device-suppression.html)&quot; leren hoe u dit kunt doen.<!-- The AM pulled this paragraph verbatim from AEM doc; I change only a word or two. -->

## Opeenvolgend bericht

Door het vangen van beeldgegevens, kunt u een segment van gebruikers tot stand brengen die aan een campagne of een advertentie zijn blootgesteld en dit segment voor opeenvolgend overseinen of onderdrukking gebruiken. U kunt bijvoorbeeld gebruikers die creatief hebben gezien, opnieuw als doelgroep instellen `123` maar u hebt niet geklikt of geconverteerd door ze creatief weer te geven `456`.

Voer de volgende stappen uit om dit voorbeeld in de Audience Manager uit te voeren:<!-- The AM pulled this example/procedure verbatim from AEM doc; I changed only a word or two. -->

1. Maak een eigenschap om gebruikers vast te leggen die de creatieve foto&#39;s hebben gezien.

   Als u bijvoorbeeld de eigenschap een naam wilt geven `Creative Trait 123`en gebruikt u de volgende regel:

   `d_creative == 123 AND d_event == imp`

1. Maak een eigenschap om gebruikers vast te leggen die klikken of converteren.

   Als u deze eigenschap bijvoorbeeld een naam wilt geven `Click and Converter`en gebruikt u de volgende regel:

   `d_event == click OR d_event=conv`

1. Een segment maken met de naam `Retarget Users` vullen met gebruikers die creatief hebben gezien `123` maar u hebt niet geklikt of geconverteerd. Gebruik de volgende gedragslijn:

   `Creative Trait 123 AND NOT Click and Converter`

1. Het segment toewijzen `Retarget Users` naar een bestemming en doelgebruikers op de bestemming met creatieve `456`.

## [!DNL Adobe Audience Analytics] en Campagne-belichtingsgegevens

Zodra de campagneindruk en de klikgegevens binnen Audience Manager beschikbaar zijn, kunt u eigenschappen en segmenten van gebruikers tot stand brengen die aan, of interactie met, een bepaalde campagne of een tactiek werden blootgesteld. Met een [[!DNL Audience Analytics] integratie](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)kunt u de segmenten van uw Audience Manager synchroniseren met [!DNL Analytics] voor verdere analyse. Mogelijke gevallen van gebruik zijn onder meer:

* **Interactieanalyse tussen DSP- en Advertising Cloud Search-advertenties:** De norm [[!DNL Analytics for Advertising Cloud] integratie](/help/integrations/analytics/overview.md) biedt geen inzicht in de interactie tussen DSP en [!DNL Search] omdat beide kanalen AMO-id&#39;s gebruiken die de toewijzingsregels voor AMO-id&#39;s volgen, waarvoor een zoekopdracht een weergaveweergave overschrijft. Door een DSP belichtingssegment in de Audience Manager te maken, kunt u [!DNL Audience Analytics] de interactie tussen DSP en [!DNL Search] advertenties in [!DNL Analytics].

* **Frequentieanalyse:** U kunt segmenten in Audience Manager maken op basis van het aantal keren dat een gebruiker aan een bepaalde advertentie of campagne is blootgesteld. Vervolgens kunt u de verschillende belichtingssegmenten in Analytics analyseren om te zien hoe het gedrag van de gebruiker verandert afhankelijk van het aantal DSP belichtingen.

## [!DNL Audience Optimization Reports]

U kunt [Audience Manager [!DNL Audience Optimization Reports]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-reports.html) om potentiële prestatiemogelijkheden voor segmenten over uw campagnes te identificeren. Deze rapporten combineren campagneindruk, klik, en omzettingsgegevens met segmentmetriek om segment-centric optimalisaties en een efficiënte kanaalmengeling te informeren.

### Typen relevante Audience Optimization-rapporten

| Rapport | Beschrijving |
| ------ | ----------- |
| [[!UICONTROL Segment Performance] Rapport](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/segment-performance.html) | Vergelijkt in kaart gebrachte en unmapped segmenten door beelden en omzettingspercentages. |
| [[!UICONTROL Trend Analysis and Volume Analysis] Rapporten]9https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/trend-analysis-volume-analysis.html) | Retourneer gegevens over afbeeldingen, doorkliksnelheden en conversies voor een groot aantal verschillende advertentiemetingen. |
| [[!UICONTROL Optimal Frequency] Rapport](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/optimal-frequency.html) | Helpt u de optimale balans tussen het aantal gediende indrukkingen en omzettingen te ontdekken. Zo kunt u het aantal afbeeldingen dat wordt weergegeven aanpassen voordat u dalende resultaten ziet. |
| [[!UICONTROL Unique User Reach] Rapport](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/unique-user-reach.html) | Een bubbelgrafiek, waarin elke bel in direct verhouding aan het aantal unieke gebruikers voor uw geselecteerde afmeting wordt gerangschikt. |

### Overwegingen

* Indien [!DNL Audience Optimization Reports] gebruikers hebben op rol-gebaseerde toegangscontroles (RBAC), dan [!DNL Adobe Customer Care] moet een afbeelding tussen Advertiser identiteitskaart en de code van de de gegevensbronintegratie van de Audience Manager van de organisatie vormen. Beheerders kunnen vervolgens RBAC-rechten aan verschillende gebruikers verstrekken.

* Conversierapportage in [!DNL Audience Optimization Reports] vereist enige opstelling door de eindgebruiker. Gebruikers moeten metagegevensbestanden invullen.

* [!DNL Audience Optimization Reports] ondersteunt geen wijzigingen in campagnemetagegevens (zoals naam van de campagne of naam van de plaatsing).

* Klik op zoekopdrachten zijn opgenomen in [!DNL Audience Optimization Reports] alleen als ze gecorreleerd zijn met impressies. Met andere woorden, zoekklikken worden na indrukken beschouwd als omzettingen. Hierdoor is het mogelijk dat veel zoekklikken niet zijn opgenomen in [!DNL Audience Optimization Reports].

>[!MORELIKETHIS]
>
>* [Overzicht van het verzenden van gegevens over DSP mediablootstelling naar Adobe Audience Manager](overview.md)
>* [Gegevens over klikken en indrukken verzamelen vanuit Advertising Cloud DSP-campagnes](collect.md)

