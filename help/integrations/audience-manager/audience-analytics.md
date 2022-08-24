---
title: '''[!DNL Adobe] [!DNL Audience Analytics] voor Advertising Cloud-klanten'
description: Leren gebruiken [!DNL Adobe] [!DNL Audience Analytics] voor reclamedoeleinden
feature: Integration with Adobe Audience Manager
exl-id: e05ba560-d3d5-4024-b1ba-956e878a2578
source-git-commit: 4a7766e92ffaa8f32f0fe8941f6c85405bd2df3e
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# [!DNL Adobe] [!DNL Audience Analytics] voor Advertising Cloud-klanten

[[!DNL Adobe] [!DNL Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html) is een integratie tussen Adobe Audience Manager en Adobe Analytics die klanten van de Audience Manager toestaat om segmenten te verzenden naar [!DNL Analytics] voor verrijkte inzichten in de activiteit van de site.

Advertising Cloud-klanten kunnen profiteren van [!DNL Audience Analytics]. Dankzij de integratie kunt u:

* Advertising Cloud-belichtingsgegevens rechtstreeks verzenden naar [!DNL Analytics] om de impact van de activiteit van de bovenschoorsteen op de activiteiten van de downstreamlocatie te bepalen.

* Bepaal de marketingkanalen en de toegangspunten van de site op basis van de blootstellingsadvertenties van de bovenste trechter.

* Laag maken voor de integratie met [!DNL Analytics for Advertising Cloud] integratie van demografische segmenten van derden uit [Audience Manager [!DNL Audience Marketplace]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/audience-marketplace/audience-marketplace.html) with [!DNL Analytics for Advertising Cloud] gegevens voor meer inzicht in gebruikersprofielen.

   [!DNL Audience Marketplace] biedt toegang tot gegevensfeeds van derden met abonnementmodellen voor activering, waarmee kopers gegevens naar een bestemming kunnen verzenden. Als de gegevens worden gebruikt binnen een [!DNL Analytics] bestemming, dan worden de activeringskosten niet toegepast.

* (Advertisers met Advertising Cloud DSP) Voeg extra blootstellingssegmenten toe voor holistische inzichten in het reisbeheer.

   Advertising Cloud DSP kan belichtingsgegevens naar Audience Manager verzenden als activeerbare signalen via de implementatie van Adobe Experience Platform of Audience Manager-tracking pixels. Dezelfde gegevens doorsturen naar [!DNL Analytics] maakt geavanceerde gegevensanalyse mogelijk. Zie &quot;[Overzicht van Advertising Cloud Media Data Integration met Adobe Audience Manager](/help/integrations/audience-manager/media-data-integration/overview.md)&quot; voor meer informatie .

Meer informatie over [!DNL Audience Analytics], inclusief de voorwaarden en workflow, raadpleegt u &quot;[Overzicht van Audience Analytics](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).&quot;

## Voorbeelden van het gebruik van [!DNL Audience Analytics] Gegevens met Advertising Cloud-gegevens

Hieronder ziet u voorbeelden van het gebruik van gecombineerde gegevens in [!DNL Analytics] [!DNL Analysis Workspace].

### Zie de impact van de Activiteit van het hoger personeel op de downstreamactiviteit

Gebruik de blootstellingssegmenten van de Audience Manager om de impact van de activiteit van de bovenste schoorsteenlocatie op de activiteiten van de downstreamlocatie te zien. Neem Advertising Cloud- of externe macro-id&#39;s op in de volgende pixels om de impact op een gedetailleerd niveau te volgen, van het campagneniveau tot het niveau van de site waarop de gebruiker is weergegeven.

Belangrijkste voordelen:

* Blootstelling aan sporen per trechter/advertentietype en gebruik [!DNL Audience Analytics] om de toegangspercentages en de overlapping met de volgende fase van de klantenreis te bepalen.

* Bepaal de impact van de activiteit van de bovenste trechter op de activiteiten van de downstreamlocatie.

* Verbinden [!DNL Analytics for Advertising Cloud]<!-- which doesn't include the last exposure event --> en [!DNL Audience Analytics] data <!-- (which includes the user's last exposure event) --> een holistische reis naar de locatie te bepalen.

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
>* [Advertising Cloud-integratie met Adobe Audience Manager](/help/integrations/audience-manager/overview.md)

