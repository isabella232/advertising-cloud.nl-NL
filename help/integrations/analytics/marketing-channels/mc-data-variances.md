---
title: Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]
description: Leer waarom de kanaalgegevens die door AMO ID worden gevolgd van kanaalgegevens kunnen variëren die door worden gevolgd [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
exl-id: 4605dc7d-43d7-414f-a509-6096c6cf5fd2
source-git-commit: b99d0ce78dc2adc16e555ef618393ef2fc11067d
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Een gemeenschappelijke vraag van gebruikers die leren over de integratie van de Advertising Cloud en [!DNL Marketing Channels] gegevenssets is &quot;Wat veroorzaakt de variatie in gegevens tussen de AMO-id en [!DNL Marketing Channels]?&quot; Of soms: &quot;Waarom worden de gegevens gebroken? Ik heb alle metriek nodig om over de rapporten te passen.&quot; Gelukkig geven discrepanties niet aan dat de gegevens &quot;gebroken&quot; zijn, en worden discrepanties verwacht en zelfs gewenst. Laten we eens kijken waarom de integratie zo is opgezet.

De twee gegevenssets hebben verschillende hoofdgebruikscenario&#39;s:

* [!DNL Marketing Channels]: Het primaire gebruiksgeval voor [!DNL Marketing Channels] is gegevens over meerdere kanalen te vergelijken met een algemeen toewijzingsmodel. De analisten kunnen de [!UICONTROL Marketing Channel] dimensie om meer inzicht te krijgen in de manier waarop kanalen met elkaar communiceren. Dit inzicht kan helpen besluiten op macroniveau over hoe te in elk kanaal te investeren en kan tot inzicht leiden hoe de bezoekers van elk kanaal met de website in wisselwerking staan.

   De [!DNL Analytics] [!UICONTROL Marketing Channel] dimensie, daarom, wordt gevormd om alle kanalen te vangen en te volgen. [!DNL Marketing Channels] kan ook worden geconfigureerd om Advertising Cloud DSP-weergaven en doorklikbewerkingen vast te leggen, en dit gebeurt met betrekking tot de andere marketingkanalen.

* Advertising Cloud AMO-id: Het belangrijkste geval van de Advertising Cloud AMO ID-gegevens is dat Advertising Cloud&#39;s geavanceerde [!DNL Adobe Sensei]-powered bidding algorithms. De algoritmen maken automatisch duizenden biedbeslissingen op microniveau die dagelijks worden genomen om de uitgaven voor reclame te maximaliseren en de doelstellingen van de [!DNL DSP] campagne of [!DNL Search] portfolio. Hoe meer conversiegegevens de algoritmen kunnen verbinden met campagnes, hoe beter de algoritmen deze biedbeslissingen kunnen nemen.

   Om deze gegevens te verzamelen, [!DNL Analytics for Advertising Cloud] integratie geeft onbewerkte AMO-id&#39;s door die kunnen worden vertaald als doorklikcodes en doorkijkcodes in de AMO-id-dimensie van Adobe Analytics. Deze worden opgeslagen als een aangepaste variabele (eVar) of een gereserveerde variabele (rVar). Doorklikken voor andere kanalen wordt niet ingesteld in de AMO ID-dimensie, zodat de AMO ID-dimensie de invoer van deze andere kanalen niet kan bijhouden. Het resultaat is dat de AMO-id doorloopt [!DNL Marketing Channels] toegangspunten.

Voor meer informatie over mogelijke gegevensvariaties tussen door Advertising Cloud bijgehouden gegevens en [!DNL Analytics]-tracked data, zie &quot;[Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](../data-variances.md).&quot;

>[!MORELIKETHIS]
>
>* [Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](/help/integrations/analytics/data-variances.md)
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Advertising Cloud-id&#39;s gebruiken om te maken [!DNL Marketing Channels] Verwerkingsregels](mc-ids.md)
>* [Gebruiken [!DNL Analytics Marketing Channels] met Advertising Cloud-gegevens](mc-ac-data.md)
>* [Video: Rapporten met Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)

