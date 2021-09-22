---
title: Over rapporten in Platform
description: Leer meer over de rapportgegevens die zijn opgenomen in de weergaven voor campagnebeheer.
feature: DSP Campaign Data Views
exl-id: e9f7dafe-e0db-4fec-bf5b-858cbcfdde45
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Over rapporten in Platform

<!-- rename "About Performance Reports in Campaign Management Views?" -->
De meningen van het campagnebeheer omvatten uitvoerige rapportgegevens. De beschikbare rapporten helpen u om de pakketten en de plaatsen te identificeren die goed presteren en die die uw aandacht vereisen. Met de knoppen voor snelle actie kunt u bovendien productiever werken.

## Alle campagnes

De weergave [!UICONTROL Campaigns] wordt geopend voor een lijst met alle campagnes in uw account. De [!UICONTROL Subtotals] rij toont of de som of de gemiddelde waarde van elke metrisch over alle zichtbare rijen.

![Lijst met campagnes](/help/dsp/assets/campaigns-list.png)

Standaard bevat elke campagnerij cijfers voor het plaatsen en leveren. Tot de maateenheden voor gegevenspakketten behoren [!UICONTROL Gross Spend (Lifetime)], die een omtrek bevat van de werkelijke doeluitgaven in vergelijking met de verwachte doeluitgaven voor alle pakketten in de campagne, zodat u in één oogopslag ondermaatse campagnes kunt identificeren. U kunt optioneel [de kolomweergave wijzigen](column-view-change.md) of zelfs [een aangepaste kolomweergave maken](column-view-create.md).

U kunt de gegevenstabellen [verder aanpassen](campaign-data-views-about.md) op extra manieren en [filter de zichtbare gegevens](campaign-data-filter.md).

Klik op de naam van de campagne als u een campagne gedetailleerder wilt weergeven.

## Single Campaign Reporting

Binnen een campagne kunt u gegevens filteren op basis van de campagneentiteit: [!UICONTROL Packages], [!UICONTROL Placements] en [!UICONTROL Ads]. U kunt [de zichtbare gegevens verder filteren](campaign-data-filter.md) om alleen de pakketten, plaatsen of advertenties op te nemen die u wilt zien.

![Tabbladen voor campagneentiteiten](/help/dsp/assets/campaign-subtabs.png)

In elk entiteitlusje, omvat elke rij het verpakken en leveringsmetriek, door gebrek, maar u kunt [de kolommening veranderen](column-view-change.md) of zelfs [een mening van de douanekolom tot stand brengen](column-view-create.md) om over alle subtabs voor de campagne van toepassing te zijn. U kunt de gegevenstabellen [verder op extra manieren aanpassen](campaign-data-views-about.md). Elke gegevenslijst omvat een [!UICONTROL Subtotals] rij, die of de som of de gemiddelde waarde van elke metrisch over alle zichtbare rijen toont.

Voor elke campagne, kunt u de grafieken van de tijdreekstrendtrend met drie metriek ook aanpassen, die in elke entiteitmening beschikbaar zijn. Standaard worden gegevens voor [!UICONTROL Net Spend], [!UICONTROL Impressions] en [!UICONTROL Net CPM] opgenomen in afzonderlijke diagrammen (diagrammen). U kunt de maatstaven desgewenst wijzigen.

![afzonderlijke trendgrafieken voor drie metriek](/help/dsp/assets/trend-chart-separate.png)

U kunt desgewenst ook de drie metriek bedekken, zodat u op eenvoudige wijze anomalieën en gebieden kunt detecteren waarin u de schaal of de prestaties kunt verbeteren.

![trenddiagram met overlay](/help/dsp/assets/trend-chart.png)

U kunt [de trendgrafieken ](campaign-data-visualization-manage.md) door campagne aanpassen, en de zelfde metriek worden voortgeduurd over alle trendgrafieken voor de campagne.

### Plaatsingscontrole

Voor elke plaatsing, kunt u [een (detailmening [!UICONTROL Inspector])](placement-details-view.md) openen, die de volgende diepgaande gegevens omvat:

* **[!UICONTROL Sites]:** Alle sites waarop de plaatsing is toegepast.

   Het tabblad [!UICONTROL Sites] bevat zoek- en filterfuncties, dezelfde standaard- en aangepaste kolomweergaveopties die beschikbaar zijn op de hoofdpagina en een [!UICONTROL Exclude]-knop in elke rij, zodat u een site snel kunt uitsluiten van de plaatsing.

* **[!UICONTROL Ads]:** Alle advertenties in de plaatsing.

   Het tabblad [!UICONTROL Ads] bevat zoek- en filterfuncties, dezelfde standaard- en aangepaste kolomweergaveopties die beschikbaar zijn op de hoofdpagina en snelle actieknoppen in elke rij, zoals [!UICONTROL Pause] (zodat u snel een advertentie kunt pauzeren).

* **[!UICONTROL Frequency]:** Gegevens voor elk advertentieniveau voor de plaatsing, met inbegrip van:
   * het ad-frequentieniveau (bijvoorbeeld &quot;1&quot; voor alle gevallen waarin gebruikers een advertentie één keer zagen)
   * het geschatte unieke aantal apparaten/browsers of personen (afhankelijk van het opgegeven [!UICONTROL Cross Device Level] voor de plaatsing) die op het opgegeven frequentieniveau afdrukken hebben ontvangen
   * het geschatte aantal indrukkingen op het opgegeven frequentieniveau
   * de geschatte gemiddelde frequentie voor het gespecificeerde frequentieniveau. Deze waarde is gelijk aan (Geschatte Impressies)/(Geschatte Uniques).

![Plaatsingscontrole](/help/dsp/assets/placement-inspector-sites.png)

U kunt de gegevens op [!UICONTROL Sites], [!UICONTROL Ads], of [!UICONTROL Frequency] lusje in de standaard downloadomslag van uw browser als rapport in formaat XLSM uitvoeren.

### Andere types van campagne-vlakke Rapportering

Voor andere gegevensbrainstormsessies bekijkt u [de oudere pagina&#39;s op campagnereniveau](/help/dsp/campaign-management/campaigns/campaign-view-report.md) van [!UICONTROL Campaigns Classic]. Het oudere rapport bevat secties over [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability] en [!UICONTROL Audience Performance] gegevens.

>[!MORELIKETHIS]
>
>* [De sites, advertenties en frequentiedetails voor een plaatsing weergeven](placement-details-view.md)
>* [Informatie over de weergaven van Campagnegegevens](campaign-data-views-about.md)
>* [Een aangepaste kolomweergave maken](column-view-create.md)
>* [De kolomweergave wijzigen](column-view-change.md)
>* [Gegevensvisualisatie beheren](campaign-data-visualization-manage.md)
>* [Gegevens exporteren uit een Campagnebeheerweergave](campaign-export-data.md)
>* [Gedetailleerd rapport voor een campagne weergeven](/help/dsp/campaign-management/campaigns/campaign-view-report.md)

