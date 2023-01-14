---
title: Overzicht van [!DNL Analytics for Advertising]
description: Overzicht van [!DNL Analytics for Advertising]
feature: Integration with Adobe Analytics
exl-id: 31367c8b-3410-4110-9ae6-11defe625355
source-git-commit: 17482b831c5db7ef6c211f87b2e408443180746e
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Overzicht van [!DNL Analytics for Advertising]

*Adverteerders met DSP en[!DNL Advertising Search]*

[!DNL Analytics for Advertising] Adobe Analytics en Adobe Advertising worden geïntegreerd om de mogelijkheden van elk product uit te breiden en te verbeteren.

Dankzij de integratie kunnen adverteerders doorklikken en de interacties van sites bekijken in hun [!DNL Analytics] exemplaren, zodat merknamen kunnen zien hoe hun advertentiepijfer leidt tot betrokkenheid van sites en kritieke bedrijfsdoelstellingen.

Daarnaast heeft Adobe Advertising toegang tot de grote gegevens van de eerste partij die [!DNL Analytics] verzamelt met [!DNL Analytics] tags die al op de site staan. Dit maakt een robuuster reisbeheer, hermarketing van de eerste partij en rapportage van betaalde mediasites mogelijk. Adobe Adverteren kan verder gebruikmaken van de [!DNL Analytics] gegevens voor optimalisatie van uitgaven en biedingen.

Indien naar behoren in dienst genomen, [!DNL Analytics for Advertising] vervaagt de lijnen tussen twee traditionele rollen: het maken van reclame voor reisbeheer ( het verzenden van gebruikers naar de site via advertenties ) en het begrijpen van die betrokkenheid via webanalyse .

Primaire voordelen:

* Verzenden [!DNL Analytics] segmenten rechtstreeks naar Adobe Advertising voor eerderangs sites.
* Gebruiken [!DNL Analytics] aangepaste en standaardgebeurtenissen als conversiesignalen voor het optimaliseren van betaalde mediacereclame.
* Profiteer van [!DNL Analytics] Analysis Workspace voor een beter begrip van de toegangspunten van sites en het gedrag van bezoekers.
* Nauwere samenwerking tussen webanalisten en betaalde medieteams mogelijk maken.
* Doorlopende permanente Adobe-advertentieweergave en doorklikid&#39;s gebruiken binnen [!DNL Analytics] de betrokkenheid van de site te begrijpen.
* Verbeter traditionele betaalde mediapporten in Analysis Workspace met aangepaste meetwaarden, aangepaste afmetingen en sitetaken die niet haalbaar zijn wanneer u gegevens of pixels exporteert naar servers of andere DSP.
* Profiteer van [!DNL Analytics] code die al op uw website staat voor het bijhouden en optimaliseren van Adobe Advertising.

>[!TIP]
>
> Kijk eens naar [videoverleiding naar [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html?lang=en#analytics).

## Analyses gebruiken voor rapportage van betaalde media

[!DNL Analytics for Advertising] verbetert de rapportage en het inzicht in de manier waarop uw advertenties het gedrag van sites beïnvloeden door het volgende toe te staan:

* Doorlopende permanente Adobe-advertentieweergave en doorklikid&#39;s gebruiken binnen [!DNL Analytics] de betrokkenheid van de site te begrijpen.
* Profiteer van Analysis Workspace voor een beter begrip van de toegangspunten voor sites en het gedrag van bezoekers. U hebt toegang tot betaalde media-dimensionale gegevens en gebeurtenisgegevens, waaronder namen van campagneentiteiten voor Adobe Advertising (tot plaatsen en advertenties) en de bijbehorende meetgegevens, zoals klikken, indrukken en kosten.

Te gebruiken [!DNL Analytics] uw organisatie heeft als betaalmiddel voor mediarapportage een Experience Cloud-aanmelding met toegang tot Analysis Workspace nodig. Uw Adobe-advertentieteam helpt u bij het toewijzen van uw Adobe Advertising-gegevens aan individuele rapportensuites in Analysis Workspace. U kunt Adobe Advertising-gegevens naar elke rapportsuite verzenden, maar u dient op de hoogte te zijn van de rapportsuites die zijn toegewezen aan Adobe Advertising en andere die dat nog niet hebben gedaan. Afhankelijk van de rapportsuite kunnen de gerapporteerde gegevens hierdoor worden gewijzigd.

[Reclame-id&#39;s Adobe binnen [!DNL Analytics]](ids.md) werkt zoals andere eVars, met een aangepaste, blijvende vervaldatum. Standaard wordt het terugkijkvenster voor toewijzingen ingesteld op 60 dagen tijdens de Adobe-advertentie-implementatie. Werk met uw [!DNL Adobe] accountteam.

Adobe De advertentiedrempels worden toegevoegd met het achtervoegsel &quot;(AMO ID)&quot; (zoals &quot;Advertentietype (AMO ID)&quot;). Zie &quot;[Adobe Advertising Metrics in Analysis Workspace](advertising-metrics-in-analytics.md)&quot; voor een lijst van de beschikbare afmetingen.

>[!NOTE]
>
> Wanneer u Adobe Advertising-gegevens (of een gegevensset) bekijkt in [!DNL Analytics], moet u er rekening mee houden dat metriek en rapporten zijn gebaseerd op de regels die binnen [!DNL Analytics]. De gegevens kunnen anders zijn dan wat u ziet in andere rapportsystemen, zoals advertentierapporten. [!DNL DSP] rapporten of rapporten van zoekprogramma&#39;s. Om inzicht te krijgen in de gegevensverschillen in [!DNL Analytics]Bovendien moet u weten wanneer de gegevens van de eVar verlopen, wat een bezoek bepaalt, wat als laatste aanraakattributie tegenover totale persisterende attributie wordt beschouwd, en andere factoren. Zie voor meer informatie [Verwachte gegevensvariaties tussen [!DNL Analytics] en Adobe-reclame](data-variances.md).

## Analyses gebruiken voor reclamecampagnes en -Portfolio van Power Adobe

Zonder extra pixels te vereisen, [!DNL Analytics for Advertising] maakt een betere optimalisatie en eenvoudigere publiekssegmentatie mogelijk door twee hoofdsignalen naar Adobe Advertising te verzenden:

* Omrekeningswaarden die als biedsignalen moeten worden gebruikt:
   * standaardwaarden, zoals [!UICONTROL Revenue] en [!UICONTROL Cart Views].
   * metriek voor de betrokkenheid van de site, zoals de paginaweergave en de meetgegevens voor bezoeken.
   * maatstaven voor aangepaste omzet.
   * gereserveerde inkomstenwaarden.
* Segmenten gemaakt in [!DNL Analytics] en gepubliceerd aan Experience Cloud.

   U kunt [!DNL Analytics] segmenten voor herbestemming van eerste site in [!DNL DSP] en betaalde zoekopdrachten.

   ([!DNL Search] alleen) Adverteerders met [!DNL Analytics] maar Audience Managers kunnen ook op tags gebaseerde soorten publiek (remarketing lijsten) en publiek met klantovereenkomsten (klantlijsten) maken op basis van Google-websites [!DNL Analytics] segmenten die met Experience Cloud worden gedeeld.

### Metrische gegevens voor siteconversie als biedsignalen

U kunt uw standaardgebeurtenissen en aangepaste gebeurtenissen gebruiken vanuit [!DNL Analytics] gewogen doelstellingen in de reclame voor Adobe op te stellen. Doelstellingen informeren biedingsbeslissingen voor je [!DNL DSP] pakketten en zoekportfolio&#39;s.

>[!NOTE]
>
> U kunt berekende metriek niet toewijzen van [!DNL Analytics] in Adobe Advertising.

Uw Adobe-advertentieteam helpt u de gebeurtenissen die van toepassing zijn op betaalde mediaprestaties te identificeren en in kaart te brengen in Adobe-advertentie, waar ze worden weergegeven in [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

Zie &quot;[Analysemetriek in Adobe-reclame](analytics-data-in-advertising.md)&quot; voor een lijst van beschikbare metriek.

### Analysesegmenten voor het opnieuw oprichten van sites

Adobe-reclame kan worden opgenomen [!DNL Analytics] segmenten voor het opnieuw in de handel brengen van DSP en [!DNL Search] advertenties die gebruikmaken van de native Experience Cloud-publieksintegratie tussen [!DNL Analytics] en Experience Cloud.

Om toegang te krijgen tot [!DNL Analytics] segmenten, moet een adverteerderaccount de [Experience Cloud ID-service](https://experienceleague.adobe.com/docs/id-service/using/home.html) ingeschakeld. Wanneer de Dienst van identiteitskaart wordt toegelaten, alle segmenten van Experience Cloud (met inbegrip van segmenten die in worden gecreeerd [!DNL Analytics] en gepubliceerd naar Experience Cloud, in Adobe Audience Manager gemaakte segmenten, in Experience Cloud gemaakte segmenten met behulp van de [!DNL People core service], en segmenten die in Adobe Experience Platform zijn gemaakt en via Audience Manager naar Adobe-reclame zijn verzonden) worden beschikbaar in Adobe Advertising zodra ze zijn verwerkt.

[!DNL Analytics] segmenten zijn binnen 24 uur beschikbaar en worden dagelijks bijgewerkt.

Voor meer informatie over de dienst van het Soorten publiek van de Experience Cloud, zie [Experience Cloud publiek](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html).

## Voorbeelden van hoe te om de Integratie te gebruiken

### Reclamegegevens van Adobe gebruiken in Analysis Workspace

Bekijk de video &quot;[Inleiding tot werkruimte en rapportage](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html).&quot;

### Adobe-publicatiedashboards maken

Als u wilt weten hoe u uw Adobe-advertentiegegevens kunt bijhouden op basis van uw doelstellingen in Analysis Workspace, raadpleegt u de video &quot;[Adobe-publicatiedashboards maken met Adobe Analytics](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-dashboards-a4adc.html).&quot;

### De Adobe-advertentie-id gebruiken voor de analyse van site-invoer

Als u wilt zien hoe u een Adobe Advertising site-ingrapport kunt maken voor de dag-van-week, tijd-van-dag, browser en geografische invloeden, raadpleegt u de video &quot;[Rapporten over Adobe-advertentiesite-invoer maken](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-site-entry-a4adc.html).&quot;

>[!MORELIKETHIS]
>
>* [Video: Inleiding tot [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html)
>* [Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising]](prerequisites.md)
>* [Adobe-advertentie-id&#39;s gebruikt door Analytics](ids.md)
>* [JavaScript-code voor analyses voor advertenties](/help/integrations/analytics/javascript.md)
>* [Verwachte gegevensvariaties tussen [!DNL Analytics] en Adobe-reclame](data-variances.md)
>* [Adobe Advertising Metrics in Analysis Workspace](/help/integrations/analytics/advertising-metrics-in-analytics.md)
>* [[!DNL Analytics] Gegevens in Adobe-reclame](/help/integrations/analytics/analytics-data-in-advertising.md)

