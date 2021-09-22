---
title: Hoe DSP uw campagnes optimaliseert
description: Leer hoe DSP de pakketten in uw campagnes optimaliseert.
feature: DSP Optimization
exl-id: 054582ef-b677-4725-b25c-b82bf3e5b43e
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Hoe DSP uw campagnes optimaliseert

Deze pagina beschrijft hoe de Advertising Cloud DSP optimization engine, die wordt aangedreven door [!DNL Adobe Sensei], de pakketten in uw campagnes optimaliseert. Neem voor tips en trucs voor het handmatig optimaliseren van uw campagnes contact op met uw Adobe-accountmanager. <!-- add link to trading playbook if we add it to help -->

De optimalisatiedoelstellingen van het pakket werken op twee niveaus:

* Voor elk pakket: DSP wijst budget toe aan elke plaatsing binnen het pakket op basis van de prestaties van de plaatsing ten opzichte van de geselecteerde KPI.

* Voor elke plaatsing/veiling in het pakket: DSP berekent de economische PKI-waarde in real time voor elke veiling per plaatsing en gebruikt deze waarde vervolgens om het bod te bepalen.

   >[!NOTE]
   >
   >De economische waarde kan zwaar worden gewogen op basis van hoe goed een plaatsing uitgaven. Als een plaatsing achter zijn uitgavendoel staat, dan zal het worden toegestaan veilingen van lagere kwaliteit te kopen. Als een plaatsing gemakkelijk zijn uitgavendoel bereikt, dan zal het zich op hogere kwaliteitsveilingen concentreren.

## Pakketoptimalisatie

DSP kan uw levering op twee fundamentele manieren optimaliseren, met 20 beschikbare variaties om zich aan uw specifiek prestatiesdoel te richten. U kunt kiezen:

* Prioriteit geven aan de prestatiesnelheid

* Prioriteit geven aan kostenefficiëntie voor balancering met prestatiesnelheid

Zie [Optimalisatiedoelstellingen en hoe te om hen ](optimization-goals.md) te gebruiken om te bepalen welk optimalisatiedoel u uw KPI(s) zal helpen bereiken.

### Pakketten die de Tarief van Prestaties voorrang geven

Voor optimalisatiedoelen die voorrang geven aan de prestatiesnelheid, voorspelt DSP de prestaties van elke veiling en biedt altijd een bod op de Max-bod. Voorbeelden van toepasselijke optimalisatiedoelstellingen zijn [!UICONTROL Highest Viewability Rate], [!UICONTROL Highest Clickthrough Rate] enzovoort.

Deze optimalisatiemodus werkt goed als:

* U kent reeds het effectieve/aanvaardbare CPM niveau (bijvoorbeeld, een historische benchmark).

* U bent bereid om [!UICONTROL Max Bid] voor elke plaatsing manueel aan te passen als u uitdagingen met het schrapen ervaart.

* U geeft prioriteit aan schaal boven efficiëntie.

#### Logica voor spatiëring {#pacing-logic-performance}

* Als de uitgaven op tijd zijn, wordt het bieden selectiever, zodat je alleen op veilingen biedt die hoge prestatietarieven zullen hebben.

* Als de bestedingen achterblijven, wordt het bieden minder selectief, zodat je op veilingen kunt bieden die lagere prestatietarieven zullen hebben om de pakketdoelstelling te halen.

#### Prijs/biedarcering wissen {#clearing-price-performance}

Nadat de prijsbepalingslogica is uitgevoerd, voert DSP het voorgestelde bod uit via een prijsvoorspellingsmodel voor clearing. Als de voorspelling aangeeft dat het bod kan worden verlaagd met een minimale verlaging van de win-rente, wordt het bod verlaagd volgens de voorspelling.

### Pakketten die prioriteit geven aan het in evenwicht brengen van kostenefficiëntie met prestatiesnelheid

Voor sommige optimalisatiedoelstellingen, voorspelt DSP de prestaties van elke veiling en past biedprijzen automatisch aan, nooit overschrijdt een plaatsing [!UICONTROL Max Bid]. Voorbeelden van toepasselijke optimalisatiedoelstellingen zijn [!UICONTROL Lowest CPM], [!UICONTROL Lowest CPA], [!UICONTROL Lowest Cost per View], [!UICONTROL Lowest Cost per Click] enzovoort.

#### Pacing Logic {#pacing-logic-balanced}

* Als de uitgaven in een tempo plaatsvinden, wordt DSP prijsgevoeliger en bieden lagere bedragen aan de handel van de win rate met het pacingplan.

* Als de prestaties metrisch ook (alle doelstellingen behalve [!UICONTROL Lowest CPM]) in evenwicht zijn, dan wordt voorspelde KPI gemengd in het bedrag dat wordt geboden. Je biedt dus een hogere biedprijs voor veilingen waarvan wordt verwacht dat ze beter presteren op basis van de kosten per.

* Als de uitgaven achter het tempo liggen, wordt DSP minder prijsgevoelig en biedt hij hogere bedragen, tot aan de [!UICONTROL Max Bid], om de win rate af te zetten met het pacing plan.

#### Prijs/biedarcering wissen {#clearing-price-balanced}

Nadat de prijsbepalingslogica is uitgevoerd, voert DSP het voorgestelde bod uit via een prijsvoorspellingsmodel voor clearing. Als de voorspelling aangeeft dat het bod kan worden verlaagd met een minimale verlaging van de win-rente, wordt het bod verlaagd volgens de voorspelling.

## Plaatsing optimaliseren

Plaatsingsfilters voor voorbiedingen zijn de strengste manier om goede prestaties te garanderen. DSP gebruikt voorbiedingsfilters strategisch voor verschillende advertentietypen om prestatiedoelen te bereiken voor verschillende plaatsen binnen elk pakket. U kunt voorbiedingsfilters gebruiken in combinatie met optimalisatie op pakketniveau of onafhankelijk van elkaar.

>[!NOTE]
>
>De beschikbare filters voor voorbiedingen variëren per advertentietype. Voor een standaardplaatsing van het beeldscherm kunt u bijvoorbeeld filteren op doorklikfrequentie en gezichtsvermogen, maar niet op voltooiingsfrequentie.

Zie [Pre-Bodfilters op plaatsingsniveau en Hoe deze te gebruiken](optimization-pre-bid-filters.md) om te bepalen welke pre-Bodmanager filter u zal helpen uw KPI(s) bereiken.

>[!MORELIKETHIS]
>
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken](optimization-pre-bid-filters.md)
>* [Problemen oplossen](/help/dsp/optimization/troubleshooting-performance.md)

