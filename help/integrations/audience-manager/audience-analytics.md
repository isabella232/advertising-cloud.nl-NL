---
title: '[!DNL Adobe] [!DNL Audience Analytics] voor Adobe Advertising Customers'
description: Leren gebruiken [!DNL Adobe] [!DNL Audience Analytics] voor reclamedoeleinden
feature: Integration with Adobe Audience Manager
exl-id: e05ba560-d3d5-4024-b1ba-956e878a2578
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# [!DNL Adobe] [!DNL Audience Analytics] voor klanten met Adobe-advertenties

[[!DNL Adobe] [!DNL Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html) is een integratie tussen Adobe Audience Manager en Adobe Analytics die klanten van de Audience Manager toestaat om segmenten te verzenden naar [!DNL Analytics] voor verrijkte inzichten in de activiteit van de site.

Adobe-advertenties die klanten kunnen gebruiken [!DNL Audience Analytics]. Dankzij de integratie kunt u:

* Adobe-advertentiegegevens rechtstreeks verzenden naar [!DNL Analytics] om de impact van de activiteit van de bovenschoorsteen op de activiteiten van de downstreamlocatie te bepalen.

* Bepaal de marketingkanalen en de toegangspunten van de site op basis van de blootstellingsadvertenties van de bovenste trechter.

* Laag maken voor de integratie met [!DNL Analytics for Advertising] integratie van demografische segmenten van derden uit [Audience Manager [!DNL Audience Marketplace]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/audience-marketplace/audience-marketplace.html) with [!DNL Analytics for Advertising] gegevens voor meer inzicht in gebruikersprofielen.

   [!DNL Audience Marketplace] biedt toegang tot gegevensfeeds van derden met abonnementmodellen voor activering, waarmee kopers gegevens naar een bestemming kunnen verzenden. Als de gegevens worden gebruikt binnen een [!DNL Analytics] bestemming, dan worden de activeringskosten niet toegepast.

* (Adverteerders met advertentie-DSP) Voeg extra blootstellingssegmenten toe voor holistische inzichten in het reisbeheer.

   Reclame DSP kan blootstellingsgegevens naar Audience Manager als activeerbare signalen door de implementatie van of Adobe Experience Platform of Audience Manager op het beeld-volgen pixel verzenden. Dezelfde gegevens doorsturen naar [!DNL Analytics] maakt geavanceerde gegevensanalyse mogelijk. Zie &quot;[Overzicht van Adobe Advertising Media Data Integration met Adobe Audience Manager](/help/integrations/audience-manager/media-data-integration/overview.md)&quot; voor meer informatie .

Meer informatie over [!DNL Audience Analytics], inclusief de voorwaarden en workflow, raadpleegt u &quot;[Overzicht van Audience Analytics](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).&quot;

## Voorbeelden van het gebruik van [!DNL Audience Analytics] Gegevens met Adobe-advertentiegegevens

Hieronder ziet u voorbeelden van het gebruik van gecombineerde gegevens in [!DNL Analytics] [!DNL Analysis Workspace].

### Zie de impact van de Activiteit van het hoger personeel op de downstreamactiviteit

Gebruik de blootstellingssegmenten van de Audience Manager om de impact van de activiteit van de bovenste schoorsteenlocatie op de activiteiten van de downstreamlocatie te zien. Neem Adobe-advertentie of macro-id&#39;s van derden op in de volgende pixels om de impact op een gedetailleerd niveau te volgen, van het campagneniveau tot het niveau van de site waarop de gebruiker is weergegeven.

Belangrijkste voordelen:

* Blootstelling aan sporen per trechter/advertentietype en gebruik [!DNL Audience Analytics] om de toegangspercentages en de overlapping met de volgende fase van de klantenreis te bepalen.

* Bepaal de impact van de activiteit van de bovenste trechter op de activiteiten van de downstreamlocatie.

* Verbinden [!DNL Analytics for Advertising]<!-- which doesn't include the last exposure event --> en [!DNL Audience Analytics] data <!-- (which includes the user's last exposure event) --> een holistische reis naar de locatie te bepalen.

Hieronder volgen voorbeelden van rapporten die u kunt maken in [!DNL Analysis Workspace].

![Zie de impact van de activiteit van de bovenste schoorsteen op de downstreamactiviteit](/help/integrations/assets/audience-analytics-upper-funnel-exposure.png)

### Gebruiken [!DNL Audience Analytics] Segmentgegevens van derden voor analyse gebruikersprofiel

De segmenten van de Audience Manager van de derde van het gebruik voor een rijkere analyse van hoe de gebruikers met uw plaats in wisselwerking staan. U kunt de informatie gebruiken om nieuw publiek van derde partijen te bepalen waarvoor om media te activeren, die op hoe de profielen van de derdesegmenten met zeer belangrijke prestatiesindicatoren voor de plaatsen van mediacampagnes verbinden.

>[!TIP]
> De Audience Manager gebruiken `Audiences ID` en `Audiences Name` de afmetingen [!DNL Analytics], net als andere dimensies die [!DNL Analytics] verzamelt.

Hieronder volgen voorbeelden van rapporten die u kunt maken in [!DNL Analysis Workspace].

![Het gebruiken van derdesegmenten om de analyse van het gebruikersprofiel te verrijken](/help/integrations/assets/audience-analytics-third-party-report.png)

>[!MORELIKETHIS]
>
>* [Adobe Advertising Integrations with Adobe Audience Manager](/help/integrations/audience-manager/overview.md)

