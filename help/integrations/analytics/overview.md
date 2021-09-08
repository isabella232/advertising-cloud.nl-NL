---
title: Overzicht van [!DNL Analytics for Advertising Cloud]
description: Overzicht van [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 31367c8b-3410-4110-9ae6-11defe625355
source-git-commit: 56ac178bf10d8c934297521ca3075783e1bc2c36
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Overzicht van [!DNL Analytics for Advertising Cloud]

*Adverteerders met Advertising Cloud DSP en Advertising Cloud Search*

[!DNL Analytics for Advertising Cloud] Adobe Analytics en Adobe Advertising Cloud integreren om de mogelijkheden van elk product uit te breiden en te verbeteren.

Dankzij de integratie kunnen adverteerders op hun [!DNL Analytics]-exemplaren doorklikken en interacties op de site doorzien, zodat ze merken kunnen zien hoe hun advertentieuitgaven leiden tot de betrokkenheid van de site en kritieke bedrijfsdoelstellingen.

Daarnaast heeft Advertising Cloud toegang tot de grote gegevens van de eerste partij die [!DNL Analytics] verzamelt met behulp van [!DNL Analytics]-tags die al op de site staan. Dit maakt een robuuster reisbeheer, hermarketing van de eerste partij en rapportage van betaalde mediasites mogelijk. Advertising Cloud kan de [!DNL Analytics]-gegevens verder gebruiken voor optimalisatie van uitgaven en biedingen.

Als [!DNL Analytics for Advertising Cloud] correct wordt gebruikt, vervaagt u de lijnen tussen twee traditionele rollen: het maken van reclame voor reisbeheer ( het verzenden van gebruikers naar de site via advertenties ) en het begrijpen van die betrokkenheid via webanalyse .

Primaire voordelen:

* Verzend [!DNL Analytics] segmenten rechtstreeks naar Advertising Cloud voor hermarketing van de eerste site.
* Gebruik [!DNL Analytics] aangepaste en standaardgebeurtenissen als conversiesignalen voor het optimaliseren van betaalde mediacereclame.
* Profiteer van [!DNL Analytics] Analysis Workspace voor een beter begrip van de toegangspunten van sites en het gedrag van bezoekers.
* Nauwere samenwerking tussen webanalisten en betaalde medieteams mogelijk maken.
* Gebruik doorlopende Advertising Cloud-weergave en doorklikid&#39;s binnen [!DNL Analytics] om de betrokkenheid van de site te begrijpen.
* Verbeter traditionele betaalde mediapporten in Analysis Workspace met aangepaste meetwaarden, aangepaste afmetingen en sitetaken die niet haalbaar zijn wanneer u gegevens of pixels exporteert naar servers of andere DSP.
* Profiteer van [!DNL Analytics]-code die al op uw website staat voor tracering en optimalisatie in Advertising Cloud.

>[!TIP]
>
> Bekijk een [videoinleiding aan [!DNL Analytics for Advertising Cloud]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html?lang=en#analytics).

## Analyses gebruiken voor rapportage van betaalde media

[!DNL Analytics for Advertising Cloud] verbetert de rapportage en het inzicht in de manier waarop uw advertenties het gedrag van sites beïnvloeden door het volgende toe te staan:

* Gebruik doorlopende Advertising Cloud-weergave en doorklikid&#39;s binnen [!DNL Analytics] om de betrokkenheid van de site te begrijpen.
* Profiteer van Analysis Workspace voor een beter begrip van de toegangspunten voor sites en het gedrag van bezoekers. U kunt betaalde media dimensionaal en gebeurtenisgegevens, die namen van de de campagneentiteit van Advertising Cloud (tot plaatsen en advertenties) en hun bijbehorende metriek, zoals kliks, beelden, en kosten omvatten.

Als u [!DNL Analytics] wilt gebruiken als betaalmedia rapportageprogramma, heeft uw organisatie een Experience Cloud-aanmelding nodig met toegang tot Analysis Workspace. Uw Advertising Cloud-team helpt u uw Advertising Cloud-gegevens toe te wijzen aan individuele rapportsuite in Analysis Workspace. U kunt Advertising Cloud-gegevens naar elke rapportsuite verzenden, maar u dient op de hoogte te zijn van de rapportsuites die aan Advertising Cloud zijn toegewezen en van de suites die dat nog niet hebben gedaan. Afhankelijk van de rapportsuite kunnen de gerapporteerde gegevens hierdoor worden gewijzigd.

[Advertising Cloud-id&#39;s werken  [!DNL Analytics]](ids.md) net als andere eVars, met een aangepaste, permanente vervaldatum. Standaard wordt het terugzoekvenster voor toewijzing ingesteld op 60 dagen tijdens de Advertising Cloud-implementatie. Werk met uw Adobe-accountmanager om deze instelling te wijzigen.

Advertising Cloud-afmetingen worden toegevoegd met het achtervoegsel &quot;(AMO-id)&quot; (zoals &quot;Advertentietype (AMO-id)&quot;). Zie &quot;[Advertising Cloud Metrics in Analysis Workspace](advertising-cloud-metrics-in-analytics.md)&quot; voor een lijst van de beschikbare afmetingen.

>[!NOTE]
>
> Wanneer u Advertising Cloud-gegevens (of een gegevensset) weergeeft in [!DNL Analytics], moet u er rekening mee houden dat metrische gegevens en rapporten zijn gebaseerd op de regels die binnen [!DNL Analytics] zijn ingesteld. De gegevens kunnen anders zijn dan wat u ziet in andere rapportagesystemen, zoals serverrapporten, [!DNL DSP]-rapporten of zoekprogrammarapporten. Om de gegevensverschillen in [!DNL Analytics] te begrijpen, moet u weten wanneer de gegevens van de eVar verlopen, wat een bezoek bepaalt, wat als laatste aanrakingsattributie tegenover totale persisterende attributie, en andere factoren wordt beschouwd. Zie [Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](data-variances.md) voor meer informatie.

## Analyses gebruiken voor Power Advertising Cloud-campagnes en -Portfolio

[!DNL Analytics for Advertising Cloud] vereist geen extra pixels en maakt een betere optimalisatie en eenvoudigere publiekssegmentatie mogelijk door twee hoofdsignalen naar Advertising Cloud te verzenden:

* Omrekeningswaarden die als biedsignalen moeten worden gebruikt:
   * standaardmetriek, zoals [!UICONTROL Revenue] en [!UICONTROL Cart Views].
   * metriek voor de betrokkenheid van de site, zoals de paginaweergave en de meetgegevens voor bezoeken.
   * maatstaven voor aangepaste omzet.
   * gereserveerde inkomstenwaarden.
* Segmenten gemaakt in [!DNL Analytics] en gepubliceerd naar Experience Cloud.

   U kunt [!DNL Analytics] segmenten voor eerste-partijplaats gebruiken herrichtend in [!DNL DSP] en betaalde onderzoeksreclame.

   (Alleen Advertising Cloud Search) Adverteerders met [!DNL Analytics] maar niet Audience Manager kunnen ook een op tags gebaseerd publiek op de Google-website maken (remarketinglijsten) en een publiek dat overeenkomt met de klant (klantlijsten) uit [!DNL Analytics]-segmenten die met Experience Cloud worden gedeeld.

### Metrische gegevens voor siteconversie als biedsignalen

U kunt uw standaardgebeurtenissen en aangepaste gebeurtenissen van [!DNL Analytics] gebruiken om gewogen doelstellingen te maken in Advertising Cloud. Doelstellingen informeren biedingsbeslissingen voor uw [!DNL DSP]-pakketten en zoekportfolio&#39;s.

>[!NOTE]
>
> U kunt berekende metriek van [!DNL Analytics] niet in Advertising Cloud in kaart brengen.

Uw Advertising Cloud-team helpt u de gebeurtenissen die van toepassing zijn op betaalde mediaprestaties te identificeren en in kaart te brengen in Advertising Cloud, waar deze gebeurtenissen worden weergegeven in [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

Zie &quot;[Metrische gegevens voor analyse in Advertising Cloud](analytics-data-in-advertising-cloud.md)&quot; voor een lijst met beschikbare metriek.

### Analysesegmenten voor het opnieuw oprichten van sites

Advertising Cloud kan [!DNL Analytics] segmenten voor hermarketingdoeleinden voor Advertising Cloud DSP- en [!DNL Search]-advertenties opnemen met behulp van de native Experience Cloud-publieksintegratie tussen [!DNL Analytics] en Experience Cloud.

Om tot de [!DNL Analytics] segmenten toegang te hebben, moet een adverteerderaccount [Experience Cloud ID Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) hebben toegelaten. Wanneer de Dienst van identiteitskaart wordt toegelaten, worden alle segmenten van de Experience Cloud (met inbegrip van segmenten die in [!DNL Analytics] worden gecreeerd en aan Experience Cloud worden gepubliceerd, segmenten die in Adobe Audience Manager worden gecreeerd, die in Experience Cloud worden gecreeerd gebruikend [!DNL People core service], en segmenten die in Adobe Experience Platform worden gecreeerd en via Audience Manager naar Advertising Cloud worden verzonden) beschikbaar binnen Advertising Cloud zodra zij worden verwerkt.

[!DNL Analytics] segmenten zijn binnen 24 uur beschikbaar en worden dagelijks bijgewerkt.

Voor meer informatie over de dienst van het Soorten publiek van de Experience Cloud, zie [Experience Cloud Soorten publiek](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html).

## Voorbeelden van hoe te om de Integratie te gebruiken

### Advertising Cloud-gegevens gebruiken in Analysis Workspace

Als u wilt leren hoe u Advertising Cloud-gegevens kunt gebruiken om visuele rapporten te maken in Analysis Workspace, raadpleegt u de video &quot;[Inleiding tot werkruimte en rapportage](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html)&quot;.

### Advertising Cloud-dashboards maken

Als u wilt leren hoe u uw Advertising Cloud-gegevens kunt bijhouden op basis van uw doelstellingen in Analysis Workspace, raadpleegt u de video &quot;[Advertising Cloud-dashboards maken met Adobe Analytics](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-dashboards-a4adc.html)&quot;.

### Advertising Cloud-id gebruiken voor analyse van siteinvoer

Als u wilt zien hoe u een Advertising Cloud-rapport voor siteinvoer kunt maken om de dag-van-week, het tijdstip-van-dag, de browser en geografische invloeden te controleren, raadpleegt u de video &quot;[Rapporten van Advertising Cloud-siteinvoer maken](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-site-entry-a4adc.html)&quot;.

>[!MORELIKETHIS]
>
>* [Video: Inleiding tot [!DNL Analytics for Advertising Cloud]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html)
>* [Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]](prerequisites.md)
>* [Advertising Cloud-id&#39;s gebruikt door Analytics](ids.md)
>* [JavaScript-code voor analyse voor Advertising Cloud](/help/integrations/analytics/javascript.md)
>* [Gegevensvariaties  [!DNL Analytics] tussen en Advertising Cloud verwacht](data-variances.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
>* [[!DNL Analytics] Gegevens in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)

