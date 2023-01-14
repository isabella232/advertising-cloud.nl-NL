---
title: Beste praktijken voor het Bouwen van een Doel van de Douane
description: Leer de beste praktijken voor het bouwen van douanedoelstellingen om uw succesgebeurtenissen te bepalen.
feature: DSP Optimization, DSP Best Practices
exl-id: 54b16325-4b72-48a3-a2e0-4e342229211c
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Beste praktijken voor het Bouwen van een Doel van de Douane

## Aangepaste doelen met één eigenschap

De volgende voorbeelden tonen hoe u doelstellingen zou kunnen vormen die één enkel (metrisch) bezit richten.

### Voorbeeld van een campagne met de opdracht &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot;Optimalisatiedoelstelling

Als het doel van uw campagne inkomsten is ([!UICONTROL Highest ROAS - Custom Goal]), bevat uw aangepaste doel (doel) de &quot;[!UICONTROL Revenue]&quot; eigendom met een gewicht van 1 (1).

![voorbeeld van een ROAS douanedoel met één enkel bezit](/help/dsp/assets/custom-goal-roas.png)

>[!NOTE]
>
> A [!UICONTROL Property Weight] van één staat gelijk aan een waarde van één voor elke $1 van opbrengst die wordt gevolgd.
>
> Een conversie van € 250 met een gewicht van één wordt bijvoorbeeld gerapporteerd als $250. Als de conversiemetrie een gewicht van 0,5 krijgt toegewezen, wordt de conversie van $250 gerapporteerd als $125 in advertentie van Adobe ($250 Conversie * 0,5) [!UICONTROL Property Weight] = $ 125).

### Voorbeeld van een campagne met de opdracht &quot;[!UICONTROL Lowest CPA - Custom Goal]&quot;Optimalisatiedoelstelling

Als uw campagnedoel de laagste kosten per verwerving (CPA) is en het slechts één succesgebeurtenis vereist, dan zult u dat één metrisch (in het volgende voorbeeld, &quot;Toepassing voorleggen&quot;) omvatten. De beste manier is om het gewicht in te stellen als één (1).

![voorbeeld van een aangepast CPA-doel met één eigenschap](/help/dsp/assets/custom-goal-roas.png)

>[!NOTE]
>
> A [!UICONTROL Property Weight] van één staat gelijk aan een waarde van één voor elke omzetting die wordt gevolgd.
>
> Als bijvoorbeeld 10 omzettingen van Toepassing verzenden worden bijgehouden, worden 10 omzettingen van Toepassing verzenden gerapporteerd.  Als aan de omzettingsmaatstaf een gewicht van 0,5 wordt toegekend, worden de 10 omzettingen gerapporteerd als vijf (5) in Adobe Advertising (10 Conversies * 0,5) [!UICONTROL Property Weight] = 5).

## Aangepaste doelen met meerdere eigenschappen

Er zijn twee scenario&#39;s waarin u veelvoudige eigenschappen in een douanedoel zou gebruiken:

* Uw campagnedoel heeft meerdere succesgebeurtenissen. U maakt bijvoorbeeld reclame voor meer dan één actie ter plekke, en alle acties worden toegeschreven aan uw CPA-doel. De volgende voorbeelddoelstelling omvat drie afzonderlijke eigenschappen (PDF Download, Contact met ons, en E-mailSign up), elk met een gewicht van één (1), die het [!DNL Adobe Sensei] algoritme dat elk van de eigenschappen even belangrijk is. Als u eigenschappen opneemt met verschillende kosten of belangrijkheid, kunt u de relatieve gewichten dienovereenkomstig aanpassen.

   ![voorbeeld van een aangepast doel met meerdere eigenschappen](/help/dsp/assets/custom-goal-multiple-properties.png)

* Het enige bezit in uw douanedoel bereikt niet het minimum van 10 omzettingen per dag die voor geoptimaliseerde prestaties wordt vereist. Dit kan gebeuren door minimale dagelijkse pakketuitgaven of een beperkt aantal natuurlijke omzettingen. Het toevoegen van extra ondersteunende eigenschappen aan het douanedoel kan u helpen de drempel 10-omzettingen-per-dag bereiken. Tien ondersteunende gebeurtenissen kunnen een pakket helpen aan de drempel van 10/dag te voldoen, zelfs als elk van hun gewichten onder één (1) is. Maar misschien hoeft u niet zoveel gebeurtenissen toe te voegen.

   Wanneer u ondersteunende eigenschappen toevoegt aan een aangepast doel, kunt u deze afwegen op hun relatieve belang voor de belangrijkste succesgebeurtenis en de hoeveelheid gegevenspunten in gedachten houden. Hierdoor kan het Adobe Sensei-algoritme meerdere eigenschappen in balans brengen en optimaliseren naar uw doel.

   De volgende voorbeelddoelstelling omvat drie eigenschappen, elk met een verschillend gewicht: Application Submit = 1, Application Start = 0.1 en Advertiser Landing Page = 0.01. Dit betekent dat elke omzetting van de Toepassing voorlegt de zelfde waarde aan uw zaken zoals gemiddeld 10 omzettingen van het Begin van de Toepassing en 100 Advertiser het Landing van de Pagina omzettingen heeft.

   ![voorbeeld van een aangepast doel met meerdere eigenschappen](/help/dsp/assets/custom-goal-multiple-properties2.png)

   Als u in plaats daarvan de Landing Page-bezoeken gelijkelijk aan Application Submits gewogen hebt, kan het natuurlijk hogere aantal landingspagina-bezoeken uw doel overweldigen en de pagina-bezoeken afschuinen.<!--reword-->

>[!MORELIKETHIS]
>
>* [Aangepaste doelen](custom-goal-about.md)
>* [Een aangepast doel maken](custom-goal-create.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)

