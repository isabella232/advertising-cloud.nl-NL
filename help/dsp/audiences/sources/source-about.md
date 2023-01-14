---
title: Ongeveer het Activeren van Authenticated Segmenten van de Bronnen van het Publiek
description: Leer over het opnemen van eerste-partijsegmenten van een platform van klantengegevens.
feature: DSP Audiences
exl-id: 3e6ede23-2b27-4b1d-bfa2-e823824633c4
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Ongeveer het Activeren van Authenticated Segmenten van de Bronnen van het Publiek

<!-- Doesn't specifically explain what you can do in our UI -->
*Beta, functie*

DSP kan eerste-partijsegmenten samenvoegen die van voor authentiek verklaarde signalen worden samengesteld die binnen een platform van klantengegevens (CDP) worden gebouwd. U kunt de opgenomen segmenten als doelen voor uw plaatsingen gebruiken.

## [!DNL Adobe Real-Time Customer Data Profile]

DSP is geïntegreerd met de [de [!DNL Adobe Real-Time Customer Data Profile (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html), die deel uitmaakt van de Adobe Experience Platform.

In [!DNL Real-time CDP], *bestemmingen* zijn verbindingen met externe gegevensplatforms die naadloze gegevensactivering toestaan. U kunt bijvoorbeeld bestemmingen gebruiken om uw bekende klantenrelaties (zoals gehashte e-mailadressen) te activeren voor gerichte reclame in digitale indelingen die door DSP worden ondersteund.

Voor meer informatie over bestemmingen, zie het Experience Platform [Doelgids](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html), inclusief een overzicht van het product, instructies voor [doelwerkruimten maken](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/destinations-workspace.html) en [doelverbindingen maken](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/connect-destination.html), en [gegevens activeren voor doelen](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/activate/activate-segment-streaming-destinations.html).

### Workflow voor het gebruik van de DSP integratie met [!DNL Real-time CDP] {#workflow-sources}

<!-- Make sure that titles make the distinctions clear -- everything can't be "Activate XXX." -->

1. [DSP toestaan om klantgegevenssegmenten te vertalen in [!DNL LiveRamp RampIDs]](source-durable-id.md) die herkenbaar zijn in een biedbare omgeving.<!-- I don't think I need this here: This requires DSP account-level and campaign-level settings to enable segment sharing with [!DNL LiveRamp], which will translate customer data to [!DNL RampIDs] to create targetable segments. Your DSP account team will perform this configuration. -->

1. [Een publieksbron maken](source-create.md) om soorten publiek te importeren naar uw DSP of een adverteerderaccount.

1. [Een [!DNL Real-Time CDP] doelverbinding in Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).

Neem voor extra ondersteuning contact op met uw [!DNL Adobe] accountteam of `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [Activeer Erkende Segmenten van de Duurzame Partners van identiteitskaart](source-durable-id.md)
>* [Creeer een Bron van het Publiek om Eerste Publiek te activeren](source-create.md)
>* [Broninstellingen voor publiek](source-settings.md)
>* [Adobe Adverteren DSP Verbinding](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [Overzicht van de doelcatalogus](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [Over Audience Management](/help/dsp/audiences/audience-about.md)

