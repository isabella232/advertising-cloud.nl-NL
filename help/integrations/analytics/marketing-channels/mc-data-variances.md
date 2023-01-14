---
title: Waarom kanaalgegevens kunnen verschillen tussen Adobe-reclame en [!DNL Marketing Channels]
description: Leer waarom de kanaalgegevens die door AMO ID worden gevolgd van kanaalgegevens kunnen variëren die door worden gevolgd [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
exl-id: 4605dc7d-43d7-414f-a509-6096c6cf5fd2
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Waarom kanaalgegevens kunnen verschillen tussen Adobe-reclame en [!DNL Marketing Channels]

*Adverteerders met een Adobe Advertising-Adobe Analytics Integration Only*

Een gemeenschappelijke vraag van gebruikers die leren over de integratie van de Adobe-reclame en [!DNL Marketing Channels] gegevenssets is &quot;Wat veroorzaakt de variatie in gegevens tussen de AMO-id en [!DNL Marketing Channels]?&quot; Of soms: &quot;Waarom worden de gegevens gebroken? Ik heb alle metriek nodig om over de rapporten te passen.&quot; Gelukkig geven discrepanties niet aan dat de gegevens &quot;gebroken&quot; zijn, en worden discrepanties verwacht en zelfs gewenst. Laten we eens kijken waarom de integratie zo is opgezet.

De twee gegevenssets hebben verschillende hoofdgebruikscenario&#39;s:

* [!DNL Marketing Channels]: Het primaire gebruiksgeval voor [!DNL Marketing Channels] is gegevens over meerdere kanalen te vergelijken met een algemeen toewijzingsmodel. De analisten kunnen de [!UICONTROL Marketing Channel] dimensie om meer inzicht te krijgen in de manier waarop kanalen met elkaar communiceren. Dit inzicht kan helpen besluiten op macroniveau over hoe te in elk kanaal te investeren en kan tot inzicht leiden hoe de bezoekers van elk kanaal met de website in wisselwerking staan.

   De [!DNL Analytics] [!UICONTROL Marketing Channel] dimensie, daarom, wordt gevormd om alle kanalen te vangen en te volgen. [!DNL Marketing Channels] kan ook worden geconfigureerd voor het vastleggen van advertenties DSP doorzoeken en doorklikken met betrekking tot andere marketingkanalen.

* AMO-id voor reclame-Adobe: Het belangrijkste gebruik van de AMO-id-gegevens voor reclame van Adobe is om de geavanceerde [!DNL Adobe Sensei]-powered bidding algorithms. De algoritmen maken automatisch duizenden biedbeslissingen op microniveau die dagelijks worden genomen om de uitgaven voor reclame te maximaliseren en de doelstellingen van de [!DNL DSP] de [!DNL Search] portfolio. Hoe meer conversiegegevens de algoritmen kunnen verbinden met campagnes, hoe beter de algoritmen deze biedbeslissingen kunnen nemen.

   Om deze gegevens te verzamelen, [!DNL Analytics for Advertising] integratie geeft onbewerkte AMO-id&#39;s door die kunnen worden vertaald als doorklikcodes en doorkijkcodes in de AMO-id-dimensie van Adobe Analytics. Deze worden opgeslagen als een aangepaste variabele (eVar) of een gereserveerde variabele (rVar). Doorklikken voor andere kanalen wordt niet ingesteld in de AMO ID-dimensie, zodat de AMO ID-dimensie de invoer van deze andere kanalen niet kan bijhouden. Het resultaat is dat de AMO-id doorloopt [!DNL Marketing Channels] toegangspunten.

Voor meer informatie over mogelijke gegevensvariaties tussen Adobe Advertising Tracked data en [!DNL Analytics]-tracked data, zie &quot;[Verwachte gegevensvariaties tussen [!DNL Analytics] en Adobe-reclame](../data-variances.md).&quot;

>[!MORELIKETHIS]
>
>* [Verwachte gegevensvariaties tussen [!DNL Analytics] en Adobe-reclame](/help/integrations/analytics/data-variances.md)
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Adobe-advertentie-id&#39;s gebruiken om te maken [!DNL Marketing Channels] Verwerkingsregels](mc-ids.md)
>* [Gebruiken [!DNL Analytics Marketing Channels] met Adobe-advertentiegegevens](mc-ac-data.md)
>* [Video: Gebruiken [!DNL Marketing Channels] voor Adobe Advertising Reporting](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)

