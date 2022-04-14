---
title: Over rapporten in Platform
description: Leer meer over de rapportgegevens die zijn opgenomen in de weergaven voor campagnebeheer.
feature: DSP Campaign Data Views
exl-id: e9f7dafe-e0db-4fec-bf5b-858cbcfdde45
source-git-commit: 0adbb7876e38a8fc7b8c42e9897492bb6255e2c3
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Over rapporten in Platform

<!-- rename "About Performance Reports in Campaign Management Views?" -->
De meningen van het campagnebeheer omvatten uitvoerige rapportgegevens. De beschikbare rapporten helpen u om de pakketten en de plaatsen te identificeren die goed presteren en die die uw aandacht vereisen. Met de knoppen voor snelle actie kunt u bovendien productiever werken.

## Alle campagnes

De [!UICONTROL Campaigns] wordt geopend voor een lijst met alle campagnes in uw account. De [!UICONTROL Subtotals] De rij toont of de som of de gemiddelde waarde van elke metrisch over alle zichtbare rijen.

![Lijst met campagnes](/help/dsp/assets/campaigns-list.png)

Standaard bevat elke campagnerij cijfers voor het plaatsen en leveren. Metrische gegevens voor paginering zijn inclusief [!UICONTROL Gross Spend (Lifetime)], die een raming bevat van de werkelijke doeluitgaven in vergelijking met de verwachte doeluitgaven voor alle pakketten in de campagne, zodat u in één oogopslag ondermaatse campagnes kunt identificeren. U kunt desgewenst [de kolomweergave wijzigen](column-view-change.md) of zelfs [een aangepaste kolomweergave maken](column-view-create.md).

U kunt [de gegevenstabellen aanpassen](campaign-data-views-about.md) op aanvullende manieren en [de zichtbare gegevens filteren](campaign-data-filter.md).

Klik op de naam van de campagne als u een campagne gedetailleerder wilt weergeven.

## Single Campaign Reporting {#single-campaign-reporting}

Binnen een campagne kunt u gegevens filteren op basis van de campagneentiteit: [!UICONTROL Packages], [!UICONTROL Placements], en [!UICONTROL Ads]. U kunt [de zichtbare gegevens filteren](campaign-data-filter.md) om alleen de pakketten, plaatsen of advertenties op te nemen die u wilt zien.

![Tabbladen voor campagneentiteiten](/help/dsp/assets/campaign-subtabs.png)

Op elk entiteitlusje, omvat elke rij het afvangen en leveringsmetriek, door gebrek, maar u kunt [de kolomweergave wijzigen](column-view-change.md) of zelfs [een aangepaste kolomweergave maken](column-view-create.md) om toe te passen op alle subtabbladen voor de campagne. U kunt [de gegevenstabellen aanpassen](campaign-data-views-about.md) op aanvullende manieren. Elke gegevenstabel bevat een [!UICONTROL Subtotals] rij, die of de som of de gemiddelde waarde van elke metrisch over alle zichtbare rijen toont.

Voor elke campagne, kunt u de grafieken van de tijdreekstrendtrend met drie metriek ook aanpassen, die in elke entiteitmening beschikbaar zijn. Standaard, gegevens voor [!UICONTROL Net Spend], [!UICONTROL Impressions], en [!UICONTROL Net CPM] zijn opgenomen in afzonderlijke grafieken ( trellis - grafieken ) . U kunt de maatstaven desgewenst wijzigen. Om uurgegevens in de grafieken van de tijdreekstrendtrend toe te laten, verander uw datumselectie in één enkele dag ([!UICONTROL Today], [!UICONTROL Yesterday], of een specifieke dag).

![afzonderlijke trendgrafieken voor drie metriek](/help/dsp/assets/trend-chart-separate.png)

U kunt desgewenst ook de drie metriek bedekken, zodat u op eenvoudige wijze anomalieën en gebieden kunt detecteren waarin u de schaal of de prestaties kunt verbeteren.

![trenddiagram met overlay](/help/dsp/assets/trend-chart.png)

U kunt [aanpassen van de trenddiagrammen](campaign-data-visualization-manage.md) per campagne en dezelfde cijfers blijven in alle trendgrafieken van de campagne bestaan .

### Plaatsing [!UICONTROL Inspector] {#placement-inspector}

Voor elke plaatsing kunt u [openen a (detailweergave) [!UICONTROL Inspector])](placement-details-view.md), die de volgende gedetailleerde gegevens bevat:

* **[!UICONTROL Sites]:** Alle sites waarop de plaatsing indrukt.

   De [!UICONTROL Sites] tab bevat zoek- en filterfuncties, dezelfde standaard- en aangepaste kolomweergaveopties die beschikbaar zijn op de hoofdpagina, en een [!UICONTROL Exclude] in elke rij zodat u een site snel van de plaatsing kunt uitsluiten.

* **[!UICONTROL Ads]:** Alle advertenties in de plaatsing.

   De [!UICONTROL Ads] tab bevat zoek- en filterfuncties, dezelfde standaard- en aangepaste kolomweergaveopties die beschikbaar zijn op de hoofdpagina, en snelle actieknoppen in elke rij, zoals [!UICONTROL Pause] (zodat u snel een advertentie kunt pauzeren).

* **[!UICONTROL Frequency]:** Gegevens voor elk ad-frequentieniveau voor de plaatsing, met inbegrip van:
   * het ad-frequentieniveau (bijvoorbeeld &quot;1&quot; voor alle gevallen waarin gebruikers een advertentie één keer zagen)
   * het geschatte unieke aantal apparaten/browsers of personen (afhankelijk van het opgegeven aantal [!UICONTROL Cross Device Level] voor de plaatsing) die indrukkingen hebben ontvangen op het opgegeven frequentieniveau
   * het geschatte aantal indrukkingen op het opgegeven frequentieniveau
   * de geschatte gemiddelde frequentie voor het gespecificeerde frequentieniveau. Deze waarde is gelijk aan (Geschatte Impressies)/(Geschatte Uniques).

* **[!UICONTROL Inventory]:** Informatie over alle overeenkomsten waarop de plaatsing betrekking heeft.

   De [!UICONTROL Inventory] tab bevat zoek- en filterfuncties, dezelfde standaard- en aangepaste kolomweergaveopties die beschikbaar zijn op de hoofdpagina, en snelle actieknoppen in elke rij, zoals [!UICONTROL Edit] en [!UICONTROL View Report]. De [!UICONTROL Inventory] het lusje laat snelle het oplossen van problemen door prestatiesstatistieken te tonen, zoals [!UICONTROL Auctions], [!UICONTROL Bids], en [!UICONTROL Win Rate].

#### Probleeminventarisatie

| Probleem | Mogelijke oorzaak | Te nemen handelingen |
| -----------| ---------- | ---------- |
| [!UICONTROL Zero Auctions] | De uitgever is niet begonnen met het verzenden van biedingsaanvragen. | Contacteer de uitgever om de overeenkomst te activeren. |
|  | De overeenkomst werd opstelling verkeerd, zoals door een onjuiste externe overeenkomstenidentiteitskaart in te gaan. | Bevestig de overeenkomstendetails en geef de overeenkomst uit. |
| [!UICONTROL Auctions but no Bids] | De plaatsing richt zich niet op de inkomende biedingsverzoeken voor de overeenkomst. <br><br> Bijvoorbeeld, zou een plaatsing zich op een geografie kunnen richten die niet voor de overeenkomst in aanmerking komt. | Bewerk indien nodig de plaatsingsdoelen om te voorkomen dat problemen bij de plaatsing onder de aandacht worden gebracht. |
|  | De plaatsing heeft geen actieve advertentie met het vereiste media type voor de overeenkomst. | Maak een advertentie met het juiste mediatype en koppel deze aan de plaatsing. |
|  | De plaatsing heeft geen toereikend budget. | Verhoog het budget voor plaatsing zodat u op inkomende aanvragen kunt bieden. |
|  | De datums van de plaatsingsvlucht overlappen niet met de data van de beeldlevering voor de overeenkomst. | Bewerk indien nodig de vluchtdatums van de plaatsing. |
| [!UICONTROL Low Win Rate] | Het maximumbod van de plaatsing (ondergrens of vast) is lager dan het minimum dat door de transactie wordt vereist. | De plaatsing verhogen [!UICONTROL Max Bid] indien nodig. |
|  | De plaatsing gebruikt vooraf geboden filters die het bieden beperken. | Verlaag de drempelwaarden van de filters vóór het bod om meer biedingen mogelijk te maken. |
|  | De doelgerichtheid van het publiek voor de plaatsing is te restrictief. | Controleer of de opgegeven doelgroepen voldoende actieve gebruikers hebben en vouw zo mogelijk het publiek uit. |

![Plaatsingscontrole](/help/dsp/assets/placement-inspector.png)

U kunt de gegevens in de [!UICONTROL Sites], [!UICONTROL Ads], of [!UICONTROL Frequency] naar de standaarddownloadmap van uw browser als een rapport in XLSM-indeling.

### Andere types van campagne-vlakke Rapportering

Voor andere gegevensbrainstormsessies, weergave [de oudere pagina&#39;s voor rapportage op campagnereniveau](/help/dsp/campaign-management/campaigns/campaign-view-report.md). Het oudere rapport bevat secties over [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability], en [!UICONTROL Audience Performance] gegevens.

>[!MORELIKETHIS]
>
>* [De sites, advertenties en frequentiedetails voor een plaatsing weergeven](placement-details-view.md)
>* [Informatie over de weergaven van Campagnegegevens](campaign-data-views-about.md)
>* [Een aangepaste kolomweergave maken](column-view-create.md)
>* [De kolomweergave wijzigen](column-view-change.md)
>* [Gegevensvisualisatie beheren](campaign-data-visualization-manage.md)
>* [Gegevens exporteren uit een Campaign Management-weergave](campaign-export-data.md)
>* [Gedetailleerd rapport voor een campagne weergeven](/help/dsp/campaign-management/campaigns/campaign-view-report.md)

