---
title: Overzicht van [!DNL Analytics for Advertising Cloud]
description: Overzicht van [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 31367c8b-3410-4110-9ae6-11defe625355
source-git-commit: b40c6f08b94e546e5fc068c46b279292a4d8a14f
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%

---

# Overzicht van [!DNL Analytics for Advertising Cloud]

*Adverteerders met Advertising Cloud DSP en Advertising Cloud Search*

[!DNL Analytics for Advertising Cloud] Adobe Analytics en Adobe Advertising Cloud integreren om de mogelijkheden van elk product uit te breiden en te verbeteren.

Dankzij de integratie kunnen adverteerders doorklikken en de interacties van sites bekijken in hun [!DNL Analytics] exemplaren, zodat merknamen kunnen zien hoe hun advertentiepijfer leidt tot betrokkenheid van sites en kritieke bedrijfsdoelstellingen.

Bovendien heeft Advertising Cloud toegang tot de grote gegevens van de eerste partij die [!DNL Analytics] verzamelt met [!DNL Analytics] tags die al op de site staan. Dit maakt een robuuster reisbeheer, hermarketing van de eerste partij en rapportage van betaalde mediasites mogelijk. Advertising Cloud kan de [!DNL Analytics] gegevens voor optimalisatie van uitgaven en biedingen.

Indien naar behoren in dienst genomen, [!DNL Analytics for Advertising Cloud] vervaagt de lijnen tussen twee traditionele rollen: het maken van reclame voor reisbeheer ( het verzenden van gebruikers naar de site via advertenties ) en het begrijpen van die betrokkenheid via webanalyse .

Primaire voordelen:

* Verzenden [!DNL Analytics] segmenten rechtstreeks naar Advertising Cloud voor hermarketing op de eerste locatie.
* Gebruiken [!DNL Analytics] aangepaste en standaardgebeurtenissen als conversiesignalen voor het optimaliseren van betaalde mediaclame.
* Profiteer van [!DNL Analytics] Analysis Workspace voor een beter begrip van de toegangspunten van sites en het gedrag van bezoekers.
* Nauwere samenwerking tussen webanalisten en betaalde medieteams mogelijk maken.
* Ononderbroken Advertising Cloud-weergave-via- en doorklikid&#39;s gebruiken binnen [!DNL Analytics] de betrokkenheid van de site te begrijpen.
* Verbeter traditionele betaalde mediapporten in Analysis Workspace met aangepaste meetwaarden, aangepaste afmetingen en sitetaken die niet haalbaar zijn wanneer u gegevens of pixels exporteert naar servers of andere DSP.
* Profiteer van [!DNL Analytics] code die al op uw website staat voor tracering en optimalisatie in Advertising Cloud.

>[!TIP]
>
> Kijk eens naar [videoverleiding naar [!DNL Analytics for Advertising Cloud]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html?lang=en#analytics).

## Analyses gebruiken voor rapportage van betaalde media

[!DNL Analytics for Advertising Cloud] verbetert de rapportage en het inzicht in de manier waarop uw advertenties het gedrag van sites beïnvloeden door het volgende toe te staan:

* Ononderbroken Advertising Cloud-weergave-via- en doorklikid&#39;s gebruiken binnen [!DNL Analytics] de betrokkenheid van de site te begrijpen.
* Profiteer van Analysis Workspace voor een beter begrip van de toegangspunten voor sites en het gedrag van bezoekers. U kunt betaalde media dimensionaal en gebeurtenisgegevens, die namen van de de campagneentiteit van Advertising Cloud (tot plaatsen en advertenties) en hun bijbehorende metriek, zoals kliks, beelden, en kosten omvatten.

Te gebruiken [!DNL Analytics] uw organisatie heeft als betaalmiddel voor mediarapportage een Experience Cloud-aanmelding met toegang tot Analysis Workspace nodig. Uw Advertising Cloud-team helpt u uw Advertising Cloud-gegevens toe te wijzen aan individuele rapportsuite in Analysis Workspace. U kunt Advertising Cloud-gegevens naar elke rapportsuite verzenden, maar u dient op de hoogte te zijn van de rapportsuites die aan Advertising Cloud zijn toegewezen en van de suites die dat nog niet hebben gedaan. Afhankelijk van de rapportsuite kunnen de gerapporteerde gegevens hierdoor worden gewijzigd.

[Advertising Cloud-id&#39;s binnen [!DNL Analytics]](ids.md) werkt zoals andere eVars, met een aangepaste, blijvende vervaldatum. Standaard wordt het terugzoekvenster voor toewijzing ingesteld op 60 dagen tijdens de Advertising Cloud-implementatie. Werk met uw [!DNL Adobe] accountteam.

Advertising Cloud-afmetingen worden toegevoegd met het achtervoegsel &quot;(AMO-id)&quot; (zoals &quot;Advertentietype (AMO-id)&quot;). Zie &quot;[Advertising Cloud Metrics in Analysis Workspace](advertising-cloud-metrics-in-analytics.md)&quot; voor een lijst van de beschikbare afmetingen.

>[!NOTE]
>
> Wanneer u Advertising Cloud-gegevens (of een gegevensset) bekijkt in [!DNL Analytics], moet u er rekening mee houden dat metriek en rapporten zijn gebaseerd op de regels die binnen [!DNL Analytics]. De gegevens kunnen anders zijn dan wat u ziet in andere rapportsystemen, zoals advertentierapporten. [!DNL DSP] rapporten of rapporten van zoekprogramma&#39;s. Om inzicht te krijgen in de gegevensverschillen in [!DNL Analytics]Bovendien moet u weten wanneer de gegevens van de eVar verlopen, wat een bezoek bepaalt, wat als laatste aanraakattributie tegenover totale persisterende attributie wordt beschouwd, en andere factoren. Zie voor meer informatie [Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](data-variances.md).

## Analyses gebruiken voor Power Advertising Cloud-campagnes en -Portfolio

Zonder extra pixels te vereisen, [!DNL Analytics for Advertising Cloud] maakt betere optimalisatie en eenvoudigere publiekssegmentatie mogelijk door twee hoofdsignalen naar Advertising Cloud te verzenden:

* Omrekeningswaarden die als biedsignalen moeten worden gebruikt:
   * standaardwaarden, zoals [!UICONTROL Revenue] en [!UICONTROL Cart Views].
   * metriek voor de betrokkenheid van de site, zoals de paginaweergave en de meetgegevens voor bezoeken.
   * maatstaven voor aangepaste omzet.
   * gereserveerde inkomstenwaarden.
* Segmenten gemaakt in [!DNL Analytics] en gepubliceerd aan Experience Cloud.

   U kunt [!DNL Analytics] segmenten voor herbestemming van eerste site in [!DNL DSP] en betaalde zoekopdrachten.

   (Alleen Advertising Cloud Search) Adverteerders met [!DNL Analytics] maar Audience Managers kunnen ook op tags gebaseerde soorten publiek (remarketing lijsten) en publiek met klantovereenkomsten (klantlijsten) maken op basis van Google-websites [!DNL Analytics] segmenten die met Experience Cloud worden gedeeld.

### Metrische gegevens voor siteconversie als biedsignalen

U kunt uw standaardgebeurtenissen en aangepaste gebeurtenissen gebruiken vanuit [!DNL Analytics] het opbouwen van gewogen doelstellingen in Advertising Cloud. Doelstellingen informeren biedingsbeslissingen voor je [!DNL DSP] pakketten en zoekportfolio&#39;s.

>[!NOTE]
>
> U kunt berekende metriek niet toewijzen van [!DNL Analytics] naar Advertising Cloud.

Uw Advertising Cloud-team helpt u de gebeurtenissen die van toepassing zijn op betaalde mediaprestaties te identificeren en in kaart te brengen in Advertising Cloud, waar ze worden weergegeven in [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

Zie &quot;[Analytische gegevens in Advertising Cloud](analytics-data-in-advertising-cloud.md)&quot; voor een lijst van beschikbare metriek.

### Analysesegmenten voor het opnieuw oprichten van sites

Advertising Cloud kan worden opgenomen [!DNL Analytics] segmenten voor hermarketingdoeleinden voor Advertising Cloud DSP en [!DNL Search] advertenties die gebruikmaken van de native Experience Cloud-publieksintegratie tussen [!DNL Analytics] en Experience Cloud.

Om toegang te krijgen tot [!DNL Analytics] segmenten, moet een adverteerderaccount de [Experience Cloud ID-service](https://experienceleague.adobe.com/docs/id-service/using/home.html) ingeschakeld. Wanneer de Dienst van identiteitskaart wordt toegelaten, alle segmenten van Experience Cloud (met inbegrip van segmenten die in worden gecreeerd [!DNL Analytics] en gepubliceerd naar Experience Cloud, in Adobe Audience Manager gemaakte segmenten, in Experience Cloud gemaakte segmenten met behulp van de [!DNL People core service]en segmenten die in Adobe Experience Platform zijn gemaakt en via Audience Manager naar Advertising Cloud worden verzonden), worden in Advertising Cloud beschikbaar zodra ze worden verwerkt.

[!DNL Analytics] segmenten zijn binnen 24 uur beschikbaar en worden dagelijks bijgewerkt.

Voor meer informatie over de dienst van het Soorten publiek van de Experience Cloud, zie [Experience Cloud publiek](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html).

## Voorbeelden van hoe te om de Integratie te gebruiken

### Advertising Cloud-gegevens gebruiken in Analysis Workspace

Bekijk de video &quot;[Inleiding tot werkruimte en rapportage](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html).&quot;

### Advertising Cloud-dashboards maken

Bekijk de video &quot;[Advertising Cloud-dashboards maken met Adobe Analytics](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-dashboards-a4adc.html).&quot;

### Advertising Cloud-id gebruiken voor analyse van siteinvoer

Als u wilt zien hoe u een Advertising Cloud-sitemelding kunt maken om de dag-van-week, tijd-van-dag, browser en geografische invloeden te controleren, raadpleegt u de video &quot;[Rapporten Advertising Cloud-site-item maken](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-site-entry-a4adc.html).&quot;

>[!MORELIKETHIS]
>
>* [Video: Inleiding tot [!DNL Analytics for Advertising Cloud]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html)
>* [Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]](prerequisites.md)
>* [Advertising Cloud-id&#39;s gebruikt door Analytics](ids.md)
>* [JavaScript-code voor analyse voor Advertising Cloud](/help/integrations/analytics/javascript.md)
>* [Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](data-variances.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
>* [[!DNL Analytics] Gegevens in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)

