---
title: "[!DNL Analytics] Gegevens in Adobe Advertising"
description: "[!DNL Analytics] Gegevens in Adobe Advertising"
feature: Integration with Adobe Analytics
exl-id: 79fbc809-9965-41c1-971f-3652cc78fee3
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# [!DNL Analytics] Gegevens in Adobe-reclame

*Adverteerders met een Adobe Advertising-Adobe Analytics Integration Only*

## Analysesegmenten

Alle segmenten gemaakt in [!DNL Analytics] en gepubliceerd aan Experience Cloud.

Het duurt 24 tot 48 uur om nieuwe segmenten weer te geven in Adobe Advertising. Updates voor bestaande segmenten worden binnen ongeveer acht uur gesynchroniseerd.

<!-- I added "metric" to some of the links below, even though it looks redundant, because of syntax limitations: If you use [!DNL] or [!UICONTROL] as the sole text of a link (such as [[!UICONTROL Revenue]], the tag is included in the link text (such as "[!UICONTROL Revenue]") when it's published. -->

## Metrische gegevens over betrokkenheid site

>[!NOTE]
>
>* [!DNL Analytics] geeft gebeurtenissen voor de EF-id-eVar door aan Adobe-reclame.  De standaardintegratie ondersteunt niet het verzenden van berekende metriek of andere dimensies (eVars) naar Adobe Advertising. Als de berekende metrische waarde echter volledig kan worden vastgelegd in een aangepaste gebeurtenis, kan Adobe Advertising de aangepaste gebeurtenis opnemen.
>* [!DNL Analytics] geeft gegevens door aan Adobe Advertising per uur.


* [!UICONTROL Timespent_secs_1stvisit]: Het aantal seconden dat de bezoeker tijdens zijn eerste bezoek aan de site heeft doorgebracht.
* [!UICONTROL Timespent_secs_total]: Het totale aantal seconden dat aan de plaats over alle bezoeken binnen het klikraadplegingsvenster wordt doorgebracht.
* [!UICONTROL Pageviews_1stvisit]: Het aantal paginaweergaven op de site tijdens het eerste bezoek van de bezoeker.
* [!UICONTROL Pageviews_total]: Het totale aantal paginaweergaven op de site voor alle bezoeken in het venster voor terugzoeken van klikken.
* [[!UICONTROL Bounces] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/bounces.html)
* [[!UICONTROL Visits] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html)
* [!UICONTROL ef_id_instances]: Het aantal keren dat [!DNL Analytics] een [!UICONTROL EF ID].

## Conversiedetecties

[!DNL Analytics] geeft conversiemetriek door aan Adobe Advertising per dag.

### Standaardomzettingscijfers

* [[!UICONTROL Revenue] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/revenue.html)
* [[!UICONTROL Orders] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/orders.html)
* [[!UICONTROL Units] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/units.html)
* [[!UICONTROL Carts] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/carts.html)
* [[!UICONTROL Cart Views] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-views.html)
* [[!UICONTROL Checkouts] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/checkouts.html)
* [[!UICONTROL Cart Additions] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-additions.html)
* [[!UICONTROL Cart Removals] metrisch](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-removals.html)

### Aangepaste omzettingscijfers

Deze metriek is specifiek voor de rapportreeks, zodat variëren de beschikbare metriek voor elke klant en rapportreeks.

### Gereserveerde omzettingsstatistieken

Deze metriek is specifiek voor de rapportreeks, zodat variëren de beschikbare metriek voor elke klant en rapportreeks.

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising]](overview.md)
>* [Adobe Advertising Metrics in Analysis Workspace](/help/integrations/analytics/advertising-cloud-metrics-in-analytics.md)

