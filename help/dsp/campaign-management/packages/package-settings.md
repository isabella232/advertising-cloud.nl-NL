---
title: Pakketinstellingen
description: Zie beschrijvingen van de beschikbare pakketinstellingen.
feature: Packages
exl-id: b4d415d1-86a5-40bd-b645-1709b267c174
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Pakketinstellingen

## [!UICONTROL Basic Details]

**[!UICONTROL Name]:** De pakketnaam. De maximumlengte is 60 tekens.

**[!UICONTROL Description]:** (Optioneel) Een beschrijving van het pakket.

**[!UICONTROL 3rd Party Billed Fees]:** (Optioneel) Een statische vergoeding van derden die als niet-factureerbare kosten moet worden bijgehouden:

>[!NOTE]
>
>Facultatieve vergoedingen worden weerspiegeld in de [!UICONTROL Net CPM]-norm.
* **[!UICONTROL CPM]:** De kosten per 1000 beelden (CPM).

* **[!UICONTROL CPM Description]:** Een beschrijving van de CPM-vergoeding.

U kunt het pakket-niveau plaatsen op [plaatsingsniveau](/help/dsp/campaign-management/placements/placement-settings.md) met voeten treden.

## [!UICONTROL Goals & Budget]

**[!UICONTROL Pacing & Capping]:** (Alleen-lezen voor bestaande pakketten) Op welk niveau moet de plaats en begrenzing in de verpakking worden bepaald:

* **[!UICONTROL Package level pacing]:** Deze pakketstrategie werkt door alle opgenomen plaatsen als een  *groep* in te pakken en te begrenzen. Deze strategie zorgt ervoor dat alle plaatsingen binnen een bepaald pakket holistisch worden geoptimaliseerd, waarbij uitgaven op basis van prestaties en schaal worden verdeeld naar geselecteerde prestatiekernindicatoren (KPI&#39;s).

* **[!UICONTROL Placement level pacing]:**  Deze pakketstrategie werkt door alle opgenomen plaatsen  *afzonderlijk* in te pakken en te begrenzen. De beste praktijk is om deze strategie alleen te gebruiken om gegarandeerde transacties op de particuliere markt uit te voeren.

**[!UICONTROL Flight Dates]:** De begindatum en einddatum van het pakket.

Selecteer *[!UICONTROL *Activate Custom Flighting]** en stel de aangepaste vluchten in de onderstaande sectie [!UICONTROL Flighting] in als u optioneel niet-gelijkmatige vluchten voor het pakket wilt maken. Wanneer u aangepaste flighting hebt ingeschakeld en het pakket hebt opgeslagen, kunt u aangepaste flighting niet uitschakelen.

>[!NOTE]
>
>* De vluchtdata moeten worden opgenomen in de vluchtdata voor de campagne. Bovendien moeten de vluchtdata voor alle plaatsen die aan dit pakket zijn toegewezen, binnen deze data worden opgenomen.
> * U kunt de begindatum van het pakket niet bewerken wanneer aangepaste flighting wordt geactiveerd.


**[!UICONTROL Budget]:** (Pakketten met alleen pakketniveau) Het bruto-begrotingsmaximum en het begrotingsinterval.

Voor pakketten met aangepaste flighting is de budgetinterval altijd *[!UICONTROL All time]*. Geef voor pakketten zonder aangepaste markering de budgetinterval op: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Gross Budget]:** (Pakketten met pakket-vlakke verpakking en dynamisch margebeheer slechts) Het bruto begrotingsmaximum voor de duur van het pakket.

**[!UICONTROL Optimization Goal]:** (Pakketten met pakket-vlakke verpakking slechts) het optimalisatiedoel voor het pakket. Zie beschrijvingen van elk optimalisatiedoel bij [Optimalisatiedoelstellingen en hoe te om hen ](/help/dsp/optimization/optimization-goals.md) te gebruiken.

**[!UICONTROL Custom Goals]:** (Pakketten met aangepaste optimalisatiedoelstellingen slechts) De  [aangepaste ](/help/dsp/optimization/custom-goal-about.md) doelstelling voor het pakket. Voor meer informatie over de beste praktijken voor douanedoelstellingen en campagnes die hen gebruiken, zie [Beste praktijken voor het Bouwen van een Doel van de Douane](/help/dsp/optimization/custom-goal-best-practices.md) en [Beste praktijken voor de Campagnes van Prestaties van de Opstelling](/help/dsp/optimization/campaign-best-practices-performance.md).

**[!UICONTROL Package Goal Type]:** (Pakketten met aangepaste optimalisatiedoelstellingen) Het doel van het pakket. Met deze instelling kunt u bepalen hoe het pakket moet worden geoptimaliseerd:

* *[!UICONTROL Prospecting]:* Verkenningspakketten richten zich op het verwerven van nieuwe klanten.

* *[!UICONTROL Retargeting]:* Wanneer pakketten opnieuw worden samengesteld, wordt de focus gericht op het opnieuw toegankelijk maken van eerdere bezoekers of klanten.

* *[!UICONTROL Other]:* Alle andere doeleinden.

**[!UICONTROL Linked Package for Optimization Learnings Carryover]:** (Pakketten met alleen aangepaste optimalisatiedoelen) Een ander pakket waarvan de historische gegevens worden gebruikt als invoer voor het optimaliseren van het pakket.

**[!UICONTROL Target]:** (Pakketten met pakket-vlakke het passen slechts) het doeldoel, dat wordt gebruikt om prestaties te volgen.

>[!NOTE]
>
>Dit veld is alleen een benchmark en wordt niet gebruikt voor beslissingen.

**[!UICONTROL Frequency Cap]:** (Pakketten met pakket-vlakke verpakking slechts) Het aantal tijden een uniek apparaat of een persoon (afhankelijk van het gespecificeerde  [!UICONTROL Cross Device Level]) kan advertenties van het pakket worden gediend. U kunt onder andere *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand opgeven.

>[!NOTE]
>
>* U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP respecteert de strengste frequentiegrens in de campagnehiërarchie.
>* De beste praktijken zijn het vaststellen van frequentiecappen voor zowel prospectie als herbestemming op pakketniveau.
> * Hogere frequentiecaps resulteren in hogere uitgaven en indrukken, maar in een lager bereik. Lagere frequentiecaps resulteren in minder uitgaven en indrukken, maar in een hoger bereik.


**[!UICONTROL Pace on]:** (Pakketten met pakket-vlakke het verpakken slechts) Wat het verpakken is gebaseerd op:

* *[!UICONTROL Budget]:* (Standaard) Deze optie biedt zoveel mogelijk afbeeldingen binnen het toegewezen pakketbudget.

* *[!UICONTROL Impressions]:* Deze optie levert beelden tot een gespecificeerde hoeveelheid binnen een gespecificeerd interval wordt bereikt. Wanneer u deze optie selecteert, geeft u het aantal afbeeldingen en het interval op: *Altijd,* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Pacing Fill Strategy]:** (Pakketten met pakket-vlakke het verpakken slechts) hoe te plaats en levering:

* *[!UICONTROL Even]:* Plaatst de levering op dezelfde wijze gedurende elke vlucht, met een doel van 50% van de levering in de eerste helft van de vlucht.

* *[!UICONTROL Slightly Ahead]:* (Het gebrek) versnelt levering zodat het 55-65% volledig halverwege de vliegduur is.

* *[!UICONTROL Frontload]:* Versnelt levering zodat het 65-75% volledig halverwege de vlucht is.

* *[!UICONTROL Aggressive Frontload]:* Versnelt levering zodat het 75-85% volledig halverwege de vlucht is.

## [!UICONTROL Flighting]

(Pakketten met pakket-vlakke verpakking en met &quot;[!UICONTROL Activate Custom Flighting]&quot;toegelaten) Aangepaste vliegperiodes binnen het algemene [!UICONTROL Flight Dates] gespecificeerd in [!UICONTROL Goals & Budget] sectie.

Voer voor elke vlucht de startdatum, de einddatum en het doelaantal indrukkingen in. Als u nog een vlucht wilt toevoegen, klikt u op **[!UICONTROL Add Flight]**.

>[!MORELIKETHIS]
>
>* [Info over Pakketbeheer](package-about.md)
>* [Een pakket maken](package-create.md)
>* [Een pakket bewerken](package-edit.md)
>* [Een plaatsing koppelen aan een pakket](package-attach-placement.md)
>* [Veelgestelde vragen over Campagnebeheer](/help/dsp/campaign-management/campaign-management-faq.md)

