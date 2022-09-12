---
title: Pakketinstellingen
description: Zie beschrijvingen van de beschikbare pakketinstellingen.
feature: DSP Packages
exl-id: b4d415d1-86a5-40bd-b645-1709b267c174
source-git-commit: 6331166f563e1404c077eb848eed049b4eb0706d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Pakketinstellingen

## [!UICONTROL Basic Details]

**[!UICONTROL Name]:** De pakketnaam. De maximumlengte is 60 tekens.

**[!UICONTROL Description]:** (Optioneel) Een beschrijving van het pakket.

**[!UICONTROL 3rd Party Billed Fees]:** (Optioneel) Een statische vergoeding voor derden die als niet-factureerbare kosten moet worden bijgehouden:

>[!NOTE]
>
>Facultatieve vergoedingen worden weerspiegeld in de [!UICONTROL Net CPM] metrisch.
* **[!UICONTROL CPM]:** De kosten per 1000 impressies (CPM).

* **[!UICONTROL CPM Description]:** Een beschrijving van de CPM-vergoeding.

U kunt de instelling op pakketniveau overschrijven in het dialoogvenster [plaatsingsniveau](/help/dsp/campaign-management/placements/placement-settings.md).

## [!UICONTROL Goals & Budget]

**[!UICONTROL Pacing & Capping]:** (Alleen-lezen voor bestaande pakketten) Op welk niveau moet de plaatsing van de verpakking worden geplaatst en gelimiteerd:

* **[!UICONTROL Package level pacing]:** Deze pakketstrategie werkt door alle inbegrepen plaatsingen als een pakket te plaatsen en te begrenzen *groep*. Deze strategie zorgt ervoor dat alle plaatsingen binnen een bepaald pakket holistisch worden geoptimaliseerd, waarbij uitgaven op basis van prestaties en schaal worden verdeeld naar geselecteerde prestatiekernindicatoren (KPI&#39;s).

* **[!UICONTROL Placement level pacing]:**  Deze pakketstrategie werkt door alle meegeleverde plaatsingen te plaatsen en te begrenzen *individueel*. De beste praktijk is om deze strategie alleen te gebruiken om gegarandeerde transacties op de particuliere markt uit te voeren.

**[!UICONTROL Flight Dates]:** De begindatum en einddatum van het pakket.

Selecteer *[!UICONTROL *Activate Custom Flighting]** en zet aangepaste vluchten op in de [!UICONTROL Flighting] hieronder. Wanneer u aangepaste flighting hebt ingeschakeld en het pakket hebt opgeslagen, kunt u aangepaste flighting niet uitschakelen.

>[!NOTE]
>
>* De vluchtdata moeten worden opgenomen in de vluchtdata voor de campagne. Bovendien moeten de vluchtdata voor alle plaatsen die aan dit pakket zijn toegewezen, binnen deze data worden opgenomen.
> * U kunt de begindatum van het pakket niet bewerken wanneer aangepaste flighting wordt geactiveerd.


**[!UICONTROL Budget]:** (Pakketten met alleen pakketniveau) Het bruto-begrotingsmaximum en het begrotingsinterval.

Voor pakketten met aangepaste flighting is de budgetinterval altijd *[!UICONTROL All time]*. Geef voor pakketten zonder aangepaste markering de budgetinterval op: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Gross Budget]:** (Pakketten met alleen pakketniveau en dynamisch margebeheer) Het bruto-begrotingsmaximum voor de duur van het pakket.

**[!UICONTROL Optimization Goal]:** (Pakketten met alleen pakketniveau) Het optimalisatiedoel voor het pakket. Zie beschrijvingen van elk optimalisatiedoel op [Optimalisatiedoelstellingen en hoe deze te gebruiken](/help/dsp/optimization/optimization-goals.md).

**[!UICONTROL Custom Goals]:** (Pakketten met alleen aangepaste optimalisatiedoelen) De [aangepast doel](/help/dsp/optimization/custom-goal-about.md) voor het pakket. Voor meer informatie over de beste praktijken voor douanedoelstellingen en campagnes die hen gebruiken, zie  [Beste praktijken voor het Bouwen van een Doel van de Douane](/help/dsp/optimization/custom-goal-best-practices.md) en [Beste praktijken voor de Campagnes van Prestaties van de Opstelling](/help/dsp/optimization/campaign-best-practices-performance.md).

**[!UICONTROL Package Goal Type]:** (Pakketten met alleen aangepaste optimalisatiedoelen) Het doel van het pakket. Met deze instelling kunt u bepalen hoe het pakket moet worden geoptimaliseerd:

* *[!UICONTROL Prospecting]:* Pakketten met vooruitzichten zijn gericht op het aanschaffen van nieuwe klanten.

* *[!UICONTROL Retargeting]:* Bij het opnieuw samenstellen van pakketten worden eerdere bezoekers of klanten opnieuw belicht.

* *[!UICONTROL Other]:* Alle andere doeleinden.

**[!UICONTROL Linked Package for Optimization Learnings Carryover]:** (Pakketten met alleen aangepaste optimalisatiedoelen) Een ander pakket waarvan de historische gegevens worden gebruikt als invoer voor het optimaliseren van het pakket.

**[!UICONTROL Target]:** (Pakketten met pakket-vlakke het verpakken slechts) het doeldoel, dat wordt gebruikt om prestaties te volgen.

>[!NOTE]
>
>Dit veld is alleen een benchmark en wordt niet gebruikt voor beslissingen.

**[!UICONTROL Frequency Cap]:** (Pakketten met alleen pakketniveau) Het aantal keren dat een uniek apparaat of een unieke persoon (afhankelijk van het opgegeven [!UICONTROL Cross Device Level] voor de campagne ) kunt u advertenties uit het pakket krijgen . Opties omvatten *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand.

>[!NOTE]
>
>* U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP respecteert de strengste frequentiegrens in de campagnehiërarchie.
>* De beste praktijken zijn het vaststellen van frequentiecappen voor zowel prospectie als herbestemming op pakketniveau.
> * Hogere frequentiecaps resulteren in hogere uitgaven en indrukken, maar in een lager bereik. Lagere frequentiecaps resulteren in minder uitgaven en indrukken, maar in een hoger bereik.


**[!UICONTROL Pace on]:** (Pakketten met alleen pakketniveau) Waarop de verpakking is gebaseerd:

* *[!UICONTROL Budget]:* (Standaard) Met deze optie krijgt u zoveel mogelijk indruk binnen het toegewezen pakketbudget.

* *[!UICONTROL Impressions]:* Met deze optie worden afbeeldingen afgedrukt totdat een opgegeven hoeveelheid binnen een opgegeven interval wordt bereikt. Wanneer u deze optie selecteert, geeft u het aantal afbeeldingen en het interval op: *Alle tijd,* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* of *[!UICONTROL Weekly]*.

**[!UICONTROL Flight pacing]:** (Pakketten met alleen pakketniveau) Hoe plaats en levering over de volledige vlucht:

* *[!UICONTROL Even]:* Plaatst de levering op dezelfde wijze gedurende elke vlucht, met als doel 50% van de levering in de eerste helft van de vlucht.

* *[!UICONTROL Slightly Ahead]:* (De standaardwaarde) versnelt de levering zodat deze 55-65% volledig halverwege de vliegduur is.

* *[!UICONTROL Frontload]:* Versnelt de levering, zodat deze 65-75% volledig is halverwege de vlucht.

* *[!UICONTROL Aggressive Frontload]:* Versnelt levering zodat het 75-85% volledig halverwege de vlucht is.

**[!UICONTROL Intraday pacing]:** (Pakketten met alleen pakketniveau) Hoe plaats en levering elke dag binnen de vlucht:

* *[!UICONTROL Even]:* (De standaardinstelling) Schaalt de levering op basis van de beschikbaarheid van de voorraad. Over het algemeen worden meer advertenties overdag per uur geleverd, wanneer het veilingsvolume hoger is en er minder advertenties &#39;s ochtends en &#39;s avonds worden geleverd.

* *[!UICONTROL ASAP]:* Versnelt levering aan tweemaal de snelheid van *Even*.

   >[!CAUTION]
   >
   >Deze optie kan de prestaties negatief beïnvloeden. Gebruik dit alleen als u volledige prioriteit geeft aan levering en meer geld besteedt aan optimalisatie van prestaties.

## [!UICONTROL Flighting]

(Pakketten met pakket-vlakke verpakking en met &quot;[!UICONTROL Activate Custom Flighting]&quot; ingeschakeld) Aangepaste vliegperioden binnen het totaal [!UICONTROL Flight Dates] in de [!UICONTROL Goals & Budget] sectie.

Voer voor elke vlucht de startdatum, de einddatum en het doelaantal indrukkingen in. Als u nog een vlucht wilt toevoegen, klikt u op **[!UICONTROL Add Flight]**.

>[!MORELIKETHIS]
>
>* [Info over Pakketbeheer](package-about.md)
>* [Een pakket maken](package-create.md)
>* [Een pakket bewerken](package-edit.md)
>* [Een plaatsing koppelen aan een pakket](package-attach-placement.md)
>* [Veelgestelde vragen over Campaign Management](/help/dsp/campaign-management/campaign-management-faq.md)

