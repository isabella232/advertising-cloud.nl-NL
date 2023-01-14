---
title: Adobe Advertising Integrations with Adobe Audience Manager
description: Meer informatie over de verschillende manieren waarop Adobe Advertising gegevens kan uitwisselen met Adobe Audience Manager.
feature: Integration with Adobe Audience Manager
exl-id: 0f88235b-6f9c-4b97-9517-22e8c47e1846
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Adobe Advertising Integrations with Adobe Audience Manager

U kunt Adobe-reclame op de volgende manieren integreren met Audience Manager.

## Audience Manager en andere synchroniseren [!DNL Adobe] Segmenten voor advertentiedoeleinden

[!DNL Search] en DSP kunnen metagegevens, hiërarchische gegevens en unieke publieksgegevens ophalen voor alle Audience Managers en andere [!DNL Adobe] publiek. Deze unieke verbinding is alleen beschikbaar voor marketers die Adobe Advertising gebruiken. Zie &quot;[Adobe Audience Manager-segmenten importeren voor advertentiedoeleinden](/help/integrations/audience-manager/import-audiences.md).&quot;

### Audience Manager en overige gebruiken [!DNL Adobe] Te maken segmenten [!DNL Google Ads Audiences] {#audience-manager-google-audiences}

*Geopende adverteerders met [!DNL Advertising Search] alleen*

Binnen [!DNL [!DNL Search]], kunt u maken [!DNL Google Ads] Google-klanten komen overeen met gebruikers-id&#39;s die uw bestaande Audience Manager-segmenten gebruiken die [!UICONTROL Adobe Media Optimizer (HTTP)] en [!UICONTROL Adobe Media Optimizer Batch Destination] als bestemmingen. ([!DNL Media Optimizer] is een vroegere naam voor [!DNL [!DNL Search]].) Dit omvat Adobe Analytics-segmenten die naar Adobe Experience Cloud worden gepubliceerd en segmenten die in Adobe Experience Cloud worden gemaakt met behulp van de [!DNL People core service]. Raadpleeg de Help in het product binnen [!DNL [!DNL Search]].

[Klanten komen overeen met gebruikers-id&#39;s](https://support.google.com/google-ads/answer/9199250) werkt net als publiek met tags op de website, maar een niet-PII-id wordt toegewezen aan unieke publieksleden voor duidelijke voordelen ten opzichte van standaardklantovereenkomsten en op websites gebaseerde doelgroepen.

Als u de benodigde gebruikers-id&#39;s wilt maken, moet u een JavaScript-tag voor reclame voor Adobe gebruiken <!-- with a user ID parameter -->op uw websites. Neem contact op met uw [!DNL [!DNL Search]] accountteam voor meer informatie.

![segmentaanmaakproces](/help/integrations/assets/ad_search_user_id_pic.png)

Wanneer u het publiek hebt gemaakt, kunt u deze gebruiken in [!DNL Google Ads] campagnes als [streefcijfers of uitsluitingen op campagneniveau of op ad-groepsniveau](#audience-manager-targets).

### Audience Manager en andere [!DNL Adobe] Segmenten voor doel- of uitsluitingsadvertenties {#audience-manager-targets}

* (Geopende adverteerders met [!DNL [!DNL Search]]) U kunt alle [!DNL Google Ads] publiek dat [gemaakt met [!DNL Adobe] segmenten](#audience-manager-google-audiences) als streefdoelen of uitsluitingen op campagnereniveau of op ad-groepsniveau in uw [!DNL Google Ads] campagnes.

* (Adverteerders met DSP) U kunt uw bestaande [!DNL Adobe] segmenten als doelen voor uw advertentieplaatsen. U kunt de segmenten desgewenst opnemen in herbruikbare doelgroepen, die u kunt gebruiken als doelen of uitsluitingen voor meerdere plaatsingen.

* (Adverteerders met Creatief Adverteren) U kunt uw bestaande [!DNL Adobe] segmenten als doelen voor specifieke creatieve objecten in uw advertentie.

>[!NOTE]
>
>Voor meer informatie over hoe te om publiek in de Audience Manager en de Experience Cloud tot stand te brengen [!DNL Audience Library] interfaces, en gemeenschappelijke gebruiksgevallen voor verschillende publiekstypes, zie &quot;[Opties voor het maken van publiek](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html).&quot;

## Gegevens over belichting van DSP media naar Audience Manager verzenden

*Adverteerders met alleen DSP*

DSP klanten met Adobe Audience Manager kunnen gegevens uit advertentiecampagnes vastleggen met behulp van pixelaanroepen naar Audience Manager. U kunt de campagnegegevens dan gebruiken om op regel-gebaseerde eigenschappen te bouwen, die u kunt gebruiken om nieuwe segmenten te bepalen om diverse DSP gebruiksgevallen, zoals geavanceerdere segmentatie, frequentiebeheer, marketing analyses, en het melden van inzichten toe te laten.

Zie &quot;[Overzicht van het verzenden van gegevens over DSP mediablootstelling naar Adobe Audience Manager](/help/integrations/audience-manager/media-data-integration/overview.md)&quot; voor meer informatie .

## Ruwere inzichten in de activiteit van de Plaats met Audience Analytics krijgen

Adobe Adverteren van klanten met [[!DNL Adobe][!DNL Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html) kan zowel Adobe Advertising-trackgegevens als Audience Manager-segmenten verzenden naar [!DNL Analytics] voor verrijkte inzichten in de activiteit van de site.

Zie voor meer informatie &quot;[[!DNL Adobe][!DNL Audience Analytics] voor klanten met Adobe-advertenties](/help/integrations/audience-manager/audience-analytics.md).&quot;
