---
title: Advertising Cloud Metrics in Analysis Workspace
description: Advertising Cloud Metrics in Analysis Workspace
feature: Integration with Adobe Analytics
exl-id: d740bd19-c643-4917-9cfd-f9cf0affd07e
source-git-commit: 56ac178bf10d8c934297521ca3075783e1bc2c36
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Advertising Cloud Metrics in Analysis Workspace

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

>[!NOTE]
>
>* Advertising Cloud geeft de verkeersmaatstaven en -afmetingen dagelijks door aan [!DNL Analytics].
>* [!DNL Analytics] legt Advertising Cloud-doorklikbewerkingen en weergavedoorhalingen in real-time vast.


## Verkeersmetriek van Advertising Cloud

>[!NOTE]
>
>Alle Advertising Cloud-verkeersmetriek in [!DNL Analytics] beginnen met &quot;AMO.&quot;

| Verkeersmetrisch | Beschrijving |
| -------------- | ----------- |
| [!UICONTROL AMO Impressions] | Het aantal Advertising Cloud-afbeeldingen. |
| [!UICONTROL AMO Clicks] | Het aantal totale kliks van Advertising Cloud. |
| [!UICONTROL AMO Cost] | De Advertising Cloud besteedt geld in de valuta van de rapportensuite. |
| [!UICONTROL AMO ID Instance] | Het aantal keren dat de Advertising Cloud-id is ingesteld. |
| [!UICONTROL AMO Minutes Viewed] | Het aantal minuten dat een Advertising Cloud-video is bekeken. |
| [!UICONTROL AMO Views] | Het aantal weergaven op een advertentie. Een weergave wordt geteld wanneer de viewer de Advertising Cloud-video start. |
| [!UICONTROL AMO Views 25% Complete] | Het aantal weergaven waarvoor ten minste 25% van een Advertising Cloud-video is bekeken. |
| [!UICONTROL AMO Views 50% Complete] | Het aantal weergaven waarvoor ten minste 50% van een Advertising Cloud-video is bekeken. |
| [!UICONTROL AMO Views 75% Complete] | Het aantal weergaven waarvoor ten minste 75% van een Advertising Cloud-video is bekeken. |
| [!UICONTROL AMO Views 100% Complete] | Het aantal weergaven waarvoor 100% van een Advertising Cloud-video is bekeken. |
| [!UICONTROL AMO Viewable Impressions] | Het aantal indrukkingen dat is gemeten om te kunnen worden weergegeven volgens de plaatsingsconfiguratie. |
| [!UICONTROL AMO Not Viewable Impressions] | Het aantal indrukkingen waarvan is vastgesteld dat ze niet kunnen worden weergegeven. Deze waarde wordt berekend als ([!UICONTROL AMO Measurable Impressions] - [!UICONTROL AMO Viewable ]). |
| [!UICONTROL AMO Measurable Impressions] | Het aantal indrukkingen waarvoor de viewability instrumentatie met succes werd geïnitialiseerd. Deze waarde wordt berekend als (geïndexeerde indrukken - het aantal niet-meetbare indrukken). |

## Nuttige aangepaste berekende cijfers voor Advertising Cloud

U kunt de volgende meetgegevens voor uw Advertising Cloud-gegevens maken.

* Klik op de instantie Openingspagina ([!UICONTROL AMO ID Instances] / [!UICONTROL AMO Clicks]): Dit is het percentage mensen dat op de advertentie klikte en deze naar de landingspagina maakte.
* Meetbare snelheid ([!UICONTROL AMO Viewable Impressions] / [!UICONTROL AMO Impressions] * 100)
* Weergavegraad voor indrukking ([!UICONTROL AMO Viewable Impressions] / [!UICONTROL AMO Measureable Impressions] * 100)
* Kosten per weergave ([!UICONTROL AMO Cost] / [!UICONTROL AMO Views])
* Kosten per klik ([!UICONTROL AMO Cost] / [!UICONTROL AMO Clicks])

## Advertising Cloud Dimension

>[!NOTE]
>
>Alle Advertising Cloud-afmetingen in [!DNL Analytics] worden gevolgd door &quot;(AMO ID)&quot;.

| Dimension | Toepasselijke Advertising Cloud-gegevens | Beschrijving |
| ----------- | ---------- | ---------- |
| [!UICONTROL Ad Platform (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | Advertising Cloud DSP of de naam van de zoekmachine |
| [!UICONTROL Account (AMO ID] | [!DNL DSP] en  [!DNL Search] gegevens | De accountnaam. |
| [!UICONTROL Network (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | RTB ([!DNL DSP]) of de naam van het advertentienetwerk ([!DNL Search]) |
| [!UICONTROL Campaign (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | De naam van de campagne. |
| [!UICONTROL Optimization (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | De naam van het pakket ([!DNL DSP]) of het portfolio ([!DNL Search]). |
| [!UICONTROL Placement (AMO ID)] | [!DNL DSP] data | De plaatsingsnaam. |
| [!UICONTROL Ad Group (AMO ID)] | [!DNL Search] data | De naam van de advertentiegroep. |
| [!UICONTROL Keyword (AMO ID)] | [!DNL Search] data | Het trefwoord. |
| [!UICONTROL Match Type (AMO ID)] | [!DNL Search] data | Het type zoekovereenkomst. |
| [!UICONTROL Keyword Match Type (AMO ID)] | [!DNL Search] data | Het trefwoord en het overeenkomende type. |
| [!UICONTROL Ad Type (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | Het advertentietype, zoals `text`, `video`, `display` of `native`. |
| [!UICONTROL Ad Title (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | Het advertentietype ([!DNL DSP]) of advertentietechniek ([!DNL Search]). |
| [!UICONTROL Ad Description (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | De beschrijving van de advertentie ([!DNL DSP]) of het ad body ([!DNL Search]). |
| [!UICONTROL Ad Display URL (AMO ID)] | [!DNL Search] data | De URL die wordt weergegeven in de advertentie. |
| [!UICONTROL Ad Destination URL (AMO ID)] | [!DNL Search] data | De doel-URL voor de advertentie. |
| [!UICONTROL Landing Type (AMO ID)] | [!DNL DSP] en  [!DNL Search] gegevens | Hiermee wordt aangegeven of het item van de openingspagina een doorkijkeffect of een doorklikeffect heeft. |
| [!UICONTROL Product Target (AMO ID)] | [!DNL Search] data | Het productdoel voor een advertentie voor een productaanbieding. |

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [[!DNL Analytics] Gegevens in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)

