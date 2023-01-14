---
title: Adobe Audience Manager-segmenten importeren voor advertentiedoeleinden
description: Leer hoe u uw [!DNL Adobe] publiek naar DSP en zoeken met Adobe Audience Manager
feature: Integration with Adobe Audience Manager
exl-id: 08a40148-b7d2-442b-81e8-f3aec4fca7df
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Adobe Audience Manager-segmenten importeren voor advertentiedoeleinden

DSP en [!DNL Advertising Search] kan elke gebruiker metagegevens, hiërarchiegegevens en unieke publieksgegevens voor alle adverteerders of agentschappen ophalen [!DNL Adobe] publiek<!-- segments or audiences? Standardize terms per AAM's docs -->. Dit omvat gegevens voor:

* Adobe Audience Manager-segmenten

* Adobe Analytics-segmenten die naar Adobe Experience Cloud worden gepubliceerd

* Segmenten die in Adobe Experience Cloud zijn gemaakt met de opdracht [!DNL People core service]

* Segmenten die in Adobe Experience Platform zijn gemaakt en via Audience Manager naar Adobe Advertising worden verzonden

Toegang tot [!DNL Adobe] publiek in DSP of [!DNL Creative], moet u het publiek in DSP importeren. Toegang tot [!DNL Adobe] publiek in [!DNL [!DNL Search]], moet u het publiek importeren in [!DNL [!DNL Search]].

## Vereisten

* De adverteerder moet [de [!DNL Adobe Experience Cloud Identity (ECID) Service]](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) versie 2.0 of hoger. De [!DNL Identity Service] biedt een universele, permanente id die uw bezoekers identificeert voor alle oplossingen in Experience Cloud.

   Implementatie omvat het toevoegen van de [!DNL Identity service] code naar elke webpagina op de sites van de adverteerder.

* De organisatie moet [ingeschakeld voor Experience Cloud-services](https://experienceleague.adobe.com/docs/core-services/interface/services/core-services.html) en een Experience Cloud hebben [!DNL Organization ID] (voorheen [!DNL IMS org ID]).

   De [!UICONTROL Organization ID] kunnen organisaties met meerdere Adobe Experience Cloud-producten gegevens uitwisselen tussen bepaalde producten.

* (Adverteerders met [!DNL Analytics]) De adverteerder moet [uitvoeren [!DNL Analytics] gebruiken `appMeasurement.js`](https://experienceleague.adobe.com/docs/analytics/implementation/js/overview.html) versie 1.6.4 of hoger.

* De bezoekers van de website van de adverteerder hebben geen groot aantal [!DNL Apple Safari] gebruikers.

* (Aanbevolen wanneer de adverteerder zowel Audience Manager als [!DNL Analytics]) Als u aanroepen naar elke webpagina wilt beperken, verwijdert u de bestaande Audience Manager [!DNL Data Integration Library] code voor gegevensinzameling en laat server-zijhet door:sturen voor elk toe [!DNL Analytics] rapportsuite. Zie voor meer informatie &quot;[Server-kant door:sturen overzicht](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

* (Aanbevolen) Als de tarieven hoger zijn, verzendt u alleen de gegevens van de website van de eerste partij naar Adobe Advertising. Als de adverteerder gegevens van derden of offlinegegevens van een systeem voor het beheer van klantrelaties bundelt, kan gegevenslekken tot een lagere frequentie leiden.

## Soorten publiek in Audience Manager importeren naar DSP

### Stappen voor het importeren van soorten publiek naar DSP

De [!DNL Adobe] team voor account- en gegevensbewerkingen voert de volgende stappen uit.

1. De [!DNL Adobe] accountteam moet de instelling op adverteerderniveau configureren &quot;[!UICONTROL Adobe Analytics Cloud].&quot;

1. De [!DNL Adobe] accountteam moet een aanvraag indienen<!-- Submit a request as a JIRA task? --> aan het team van gegevensverrichtingen<!-- implementation team? --> om de segmenten van de Audience Manager van de organisatie te importeren met behulp van de integratie van Advertising DSP native API.

### Welke veranderingen resulteren in Audience Manager?

De API automatisch:

* Maakt twee DSP doelen in Audience Manager:

   * **[!UICONTROL Adobe Ad Cloud Cross-Channel (real-time)]**

   * **[!UICONTROL Adobe AdCloud Cross-Channel (batch)])**

* Zet de twee bestemmingen aan alle segmenten van de Audience Manager in kaart, toestaand Audience Manager om de segmenten met de DSP adverteerderrekening te delen die met zelfde Experience Cloud wordt geassocieerd [!DNL Organization ID] gebruikt voor Audience Manager. <!-- Verify -->

   De organisatie kan naar keuze ongewenste segmenten uit de bestemmingen binnen Audience Manager verwijderen.

* Voegt de volgende uitwisselingskoekje-synchronisatiepixel aan de container van de Audience Manager van de organisatie toe om het bereik van klantencampagnes te verbeteren:

   * Adobe AdCloud: 411 (Dit wordt standaard en automatisch als onderdeel van [!DNL Identity Service] versie 2.0. Organisaties met [!DNL Identity Service] In versies onder 2.0 moet u deze pixel toevoegen aan de container van de Audience Manager.

## Soorten publiek in Audience Manager importeren naar [!DNL Search]

### Stappen voor het importeren van soorten publiek naar [!DNL Search]

[!DNL Adobe] het personeel zal de meeste of alle volgende stappen uitvoeren.

1. De [!DNL Adobe] het accountteam moet een verzoek indienen bij het team voor gegevensbewerkingen om een integratie in te stellen tussen [!DNL Search] en Audience Manager. Neem de namen op van de Audience Manager-segmenten waarnaar u wilt exporteren [!DNL Search].

1. Binnen Audience Manager, vorm bestemmingen voor [!DNL Search]:

   1. Maak twee nieuwe doelen: `[!UICONTROL Adobe Media Optimizer (HTTP)]` en `[!UICONTROL Adobe Media Optimizer Batch Destination]`.

      [!DNL Media Optimizer] is een vroegere naam voor [!DNL Search].

   1. Geef de segmenten voor elk van de bestemmingen op.

      Met de [!UICONTROL Automatically map all current and future segments] alle segmenten worden dagelijks toegewezen en gesynchroniseerd.

      De [!UICONTROL Manually map segments] kunt u de segmenten handmatig toewijzen aan synchronisatie met de batchbestemming (`[!UICONTROL Adobe Media Optimizer Batch Destination]`). Er hoeven geen segmenten handmatig te worden toegewezen aan de HTTP-bestemming.

1. Within [!DNL Search]de [!DNL Search] het implementatieteam of een gebruiker met de directe rol van de manager van de toegangscliënt zou de invoer van moeten in werking stellen [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Audience Manager Setup].

   U moet de Experience Cloud van de organisatie invoeren [!DNL Organization ID] ([!DNL IMS org ID]). De id moet dezelfde zijn als de id die wordt gebruikt voor de account van de Audience Manager van de organisatie.

### Welke veranderingen resulteren in Audience Manager?

De organisatie ziet twee [!DNL Search] bestemmingen in Audience Manager:

* **[!UICONTROL Adobe Media Optimizer (HTTP)]**
* **[!UICONTROL Adobe Media Optimizer Batch Destination])**

## Gegevenssynchronisatie

De eerste importbewerking duurt ongeveer 24 uur. Na de eerste importbewerking worden de gegevens in real-time gesynchroniseerd met een vertraging van 1 tot 2 seconden.

<!--
### How DSP Syncs the Data

DSP syncs the data automatically using the [!DNL Adobe Experience Cloud Identity (ECID) Service]. During synchronization, the [!DNL ECID Service] calls Adobe Advertising at [!DNL cm.eversttech.net]. Because Adobe Advertising is a trusted domain, ID syncs take place from parent pages rather than within the destination publishing iframes, as they do with most third-party activation partners. Audience Manager identifies unique users by device IDs, using the [Audience Manager [!DNL Unique User ID (AAM UUID)]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html#global-device-ids), also called the [!DNL Device ID].
 
![Synchronization of [!DNL Adobe] audiences in DSP](/help/integrations/assets/audience-manager-sync.png)

### How Search Syncs the Data
-->

<!-- 
Segment membership data is sent only after one of the following events occurs:

* (Advertisers with DSP):

  * The segment is targeted in an Adobe Advertising display ad.

  * The segment is added to the [!DNL Adobe AdCloud Cross-Channel] batch and real-time destinations within the Audience Manager user interface.

* (Advertisers with [!DNL Search]):

  * The segment is targeted in an Adobe Advertising search ad.

  * The segment is added to the [!DNL Adobe Media Optimizer] batch and HTTP destinations within the Audience Manager user interface.
 -->
<!-- Is membership data/whatever available in Creative? If so, does it show the same as DSP? -->

## Waar kunt u uw gesynchroniseerde segmenten vinden

### In DSP

In DSP, worden de segmentnamen georganiseerd door de taxonomie van de Audience Manager en beschikbaar met de overeenkomstige tellingen van het segmentlidmaatschap in:

* [Plaatsingsinstellingen](https://experienceleague.adobe.com/docs/advertising-cloud/dsp/campaign-management/placements/placement-settings.html?#audience-targeting): Op de [!UICONTROL Adobe Segments] tabblad van het dialoogvenster [!UICONTROL Audience Targeting] sectie.

* In [doelinstellingen](/help/dsp/audiences/audience-settings.md): Op de [!UICONTROL Adobe Segments] tab.

### In advertentiegerelateerde

In [!DNL Creative], zijn de segmenten beschikbaar in de ervaringsmontages voor doelknopen.

### In [!DNL Advertising Search]

In [!DNL [!DNL Search]], zijn de segmenten beschikbaar wanneer u een [!DNL Google] publiek dat [!UICONTROL Data Source] &quot;[!UICONTROL Adobe Audience]&quot; van [!UICONTROL Campaigns] > [!UICONTROL Audiences] > [!UICONTROL Library].

Voor elke [!DNL Google] publiek dat u maakt, [!DNL Google] levert de omvang van het publiek.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Integrations with Adobe Audience Manager](/help/integrations/audience-manager/overview.md)

