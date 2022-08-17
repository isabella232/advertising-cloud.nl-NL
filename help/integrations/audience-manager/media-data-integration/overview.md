---
title: Overzicht van het verzenden van gegevens over DSP mediablootstelling naar Adobe Audience Manager
description: Leer hoe u Audience Manager-gebeurtenispixels kunt gebruiken om gegevens op beeldniveau vast te leggen en op klikniveau te klikken in Advertising Cloud DSP-campagnes
feature: Integration with Adobe Audience Manager
source-git-commit: e861fc53ba14d783c763b291cdc618e5f1d4124f
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Overzicht van het verzenden van gegevens over DSP mediablootstelling naar Adobe Audience Manager

*Adverteerders met alleen Advertising Cloud DSP*

*Adverteerders met alleen Advertising Cloud-Adobe Audience Manager-integratie*

Advertising Cloud DSP-klanten met Adobe Audience Manager kunnen gebeurtenispixels op Audience Manager gebruiken om gegevens op beeldniveau vast te leggen en gegevens op klikniveau van DSP campagnes te plaatsen. De gebeurtenispixels verzenden de gegevens als activeerbare signalen naar de Audience Manager. Deze signalen laten diverse DSP gebruiksgevallen toe, zoals geavanceerdere segmentatie, frequentiebeheer, marketinganalyses en rapportavergangen.

DSP brengt je niet op om deze signalen naar de Audience Manager te sturen. Nochtans, betaalt u standaard Audience Manager die kosten op servervraag worden gebaseerd, per uw contract van de Audience Manager. Audience Manager verwijdert dubbele gebeurtenissen die op twee verschillende manieren worden bijgehouden, zodat elke gebeurtenis slechts eenmaal wordt geladen.

>[!NOTE]
>
> Audience Manager ondersteunt ook het vastleggen van gegevens uit logbestanden van advertenties, wat minder flexibiliteit biedt. Dat proces wordt niet behandeld in deze documentatie.

## Primaire voordelen

* DSP campagnegegevens stromen in Audience Manager in echt - tijd, en u kunt het gebruiken om op regel-gebaseerde eigenschappen te bouwen die u gebruikt om segmenten te bepalen.

* De segmenten zijn beschikbaar voor het richten onmiddellijk na gebruikerseigenschap en segmentkwalificatie, die in real time het richten inspanningen verstevigen.

* U kunt de campagnegegevens voor dergelijke gebruiksgevallen gebruiken, zoals het aftappen van de frequentie over creatieve personen, het herrichten van gebruikers die aan vorige campagnes werden blootgesteld, en het analyseren van stroomafwaarts plaatsgedrag en ingangspunten.

* De geaggregeerde gegevens bieden een uniforme weergave van de campagneprestaties, helpen u aangepaste conversiepaden te identificeren en kunnen worden gebruikt om de volgorde van gebeurtenissen te verbeteren die tot conversies via Audience Manager leiden [!DNL Audience Optimization Reports] of via een [[!DNL Audience Analytics] integratie met Adobe Analytics](/help/integrations/audience-manager/audience-analytics.md).

## Hoe de gegevens worden bijgehouden

De Audience Manager die wordt weergegeven en waarop wordt geklikt, is gebaseerd op cookies. De pixels leggen geen gebeurtenissen vast die plaatsvinden in omgevingen zonder cookie, zoals mobiele apps en aangesloten tv (CTV).

### Pixels voor het bijhouden van indrukken

Audience Managers volgen de gegevens van de indruk voor een advertentie wanneer u een pixel-pixel transparante gebeurtenis aan de advertentie vastmaakt. De gebeurtenispixel wordt geladen telkens wanneer de advertentie aan een gebruiker wordt gediend en door Webbrowser wordt geladen. De pixel wordt geladen vanaf een clientspecifiek subdomein van [`demdex.net`](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/demdex-calls.html), dat een erfenisdomein voor Audience Manager is en parameters als sleutel-waardeparen bevat. De gebeurtenisvraag verzamelt indruk en omzettingsgegevens en verzendt het naar de servers van de de gegevensinzameling van de Audience Manager.

### Klikken en pixels bijhouden

Audience Manager houdt kliks op gelijkaardige wijze aan beelden, behalve dat het niet de transparante gebeurtenispixel laadt telkens als de advertentie wordt gediend. In plaats daarvan worden de klikgegevens bijgehouden in de doorklikURL van de advertentie. De advertentie verwijst naar een client-specifiek subdomein van [`demdex.net`](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/demdex-calls.html), dat een erfenisdomein voor Audience Manager is, voor verwerking door de servers van de de gegevensinzameling van de Audience Manager. De server leidt de gebruiker vervolgens om naar de bedoelde bestemmingspagina. De URL bevat parameters als sleutel-waardeparen.

>[!NOTE]
>
>Als uw organisatie [!DNL Analytics] gevolgd, dan hebt u misschien geen Audience Manager het klikken volgen nodig. Adobe Analytics legt kliksignalen vast en kan ze naar de Audience Manager verzenden [server-kant door:sturen](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

>[!MORELIKETHIS]
>
>* [Gegevens over klikken en indrukken verzamelen vanuit Advertising Cloud DSP-campagnes](collect.md)
>* [Gevallen gebruiken](use-cases.md)

