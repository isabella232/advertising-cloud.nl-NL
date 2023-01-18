---
title: Veelgestelde vragen over Campaign Management
description: Meer informatie over campagnebeheer, waaronder de latentieperiode voor wijzigingen en wat er gebeurt wanneer u budgetwijzigingen aanbrengt tijdens een vlucht.
feature: DSP Packages, DSP Placements
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Veelgestelde vragen over Campaign Management

<!-- Most of this information should be moved into the relevant topics (especially editing topics). -->

## Latentie van wijzigingen instellen

* Wanneer u een plaatsing of pakketinstelling wijzigt, wanneer wordt de wijziging van kracht?

   Wijzigingen in instellingen worden gewoonlijk onmiddellijk van kracht, maar kunnen tot 12 uur in beslag nemen.

   Als het de laatste dag van levering is, breng veranderingen vroeg in de dag aan zodat DSP genoeg tijd heeft om het pakket opnieuw te kalibreren dat op de veranderingen wordt gebaseerd. Als u bijvoorbeeld overschakelt van plaatsing naar vooraf laden, moet DSP opnieuw beoordelen hoe de uitgaven gedurende de rest van de vlucht worden verdeeld. Breng dat soort verandering niet aan als je maar één uur over hebt om op de laatste dag van de vlucht te leveren.

## Tussentijdse begrotingsupdates

* Wanneer u een wijziging aanbrengt in een plaatsing, hoe lang duurt DSP dan om het pakketbudget opnieuw toe te wijzen?

   De begrotingstoewijzing is gebaseerd op de prestaties bij plaatsing, die worden beoordeeld aan de hand van een gemiddelde van 14 dagen. Wijzigingen in een plaatsing leiden alleen tot wijzigingen in de begrotingstoewijzing wanneer de prestaties tijdens het gemiddelde van 14 dagen worden gewijzigd.

   Wanneer de prestaties veranderen, DSP het pakketbudget onder de plaatsen dienovereenkomstig tijdens de volgende cyclus van de begrotingsoptimalisering, die om ongeveer middernacht (00:00) in de tijdzone van de campagne voorkomt.

* Hoe wordt het budget opnieuw toegewezen wanneer een plaatsing uit een pakket wordt verwijderd en aan een ander pakket wordt toegevoegd?

   De volledige doorloophistorie van een plaatsing wordt aan de plaatsing gekoppeld en wordt hiermee van pakket naar pakket verplaatst.

   Wanneer u een plaatsing uit een pakket verwijdert, heeft het pakket niet langer een geschiedenis van de uitgaven van de plaatsing. Het pakketbudget wordt (budget voor pakketreizen - budget voor plaatsing verwijderd) / het resterende tijdsinterval tijdens de vlucht. De pakketbegroting wordt vervolgens toegewezen aan de overblijvende plaatsen in het pakket.

   Als u dezelfde plaatsing aan een ander pakket toevoegt, houdt DSP rekening met de doorloopgeschiedenis van de plaatsing wanneer het budget voor alle plaatsingen in het nieuwe pakket wordt toegewezen.

* Hoe verandert het pakket op de laatste dag van een vlucht?

   Op de laatste dag van een vlucht wordt de dag verkort van 24 uur tot 23 uur, zodat het budget voor het pakket niet wordt overschreden. De strategie voor het vullen met pakketten wordt ook automatisch gewijzigd in &quot;[!UICONTROL Frontload],&quot; zelfs als deze is ingesteld op &quot;[!UICONTROL even].&quot; Dit betekent dat 65% van de dagelijkse begroting voor 2011:30 uur EST moet zijn.

>[!MORELIKETHIS]
>
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
>* [Beste praktijken voor de Campagnes van Prestaties van de Opstelling](/help/dsp/optimization/campaign-best-practices-performance.md)

