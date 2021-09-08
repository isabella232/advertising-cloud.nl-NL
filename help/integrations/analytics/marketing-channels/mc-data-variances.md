---
title: Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]
description: Leer waarom de kanaalgegevens die door AMO ID worden gevolgd van kanaalgegevens kunnen variëren die door  [!DNL Analytics Marketing Channels] worden gevolgd.
feature: Integration with Adobe Analytics
exl-id: null
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Een veelvoorkomende vraag van gebruikers die leren over de integratie van de Advertising Cloud- en [!DNL Marketing Channels]-gegevenssets is &quot;Wat veroorzaakt de variatie in gegevens tussen de AMO-id en [!DNL Marketing Channels]?&quot; Of soms: &quot;Waarom worden de gegevens gebroken? Ik heb alle metriek nodig om over de rapporten te passen.&quot; Gelukkig geven discrepanties niet aan dat de gegevens &quot;gebroken&quot; zijn, en worden discrepanties verwacht en zelfs gewenst. Laten we eens kijken waarom de integratie zo is opgezet.

De twee gegevenssets hebben verschillende hoofdgebruikscenario&#39;s:

* [!DNL Marketing Channels]: Het primaire gebruik voor  [!DNL Marketing Channels] is gegevens over meerdere kanalen te vergelijken met een gemeenschappelijk attributiemodel. De analisten kunnen de [!UICONTROL Marketing Channel] dimensie gebruiken om verhoogde inzichten in te winnen hoe de kanalen met elkaar in wisselwerking staan. Dit inzicht kan helpen besluiten op macroniveau over hoe te in elk kanaal te investeren en kan tot inzicht leiden hoe de bezoekers van elk kanaal met de website in wisselwerking staan.

   De [!DNL Analytics] [!UICONTROL Marketing Channel] dimensie, daarom, wordt gevormd om alle kanalen te vangen en te volgen. [!DNL Marketing Channels] kan ook worden geconfigureerd om Advertising Cloud DSP-weergaven en doorklikbewerkingen vast te leggen, en dit gebeurt met betrekking tot de andere marketingkanalen.

* Advertising Cloud AMO-id: Het belangrijkste gebruik van de Advertising Cloud AMO ID-gegevens is het doorvoeren van geavanceerde [!DNL Adobe Sensei]-georiënteerde biedalgoritmen van Advertising Cloud. De algoritmen maken automatisch duizenden biedbeslissingen op microniveau die dagelijks worden genomen om de uitgaven voor reclame te maximaliseren en de doelstellingen van de [!DNL DSP] campagne of [!DNL Search] portefeuille te bereiken. Hoe meer conversiegegevens de algoritmen kunnen verbinden met campagnes, hoe beter de algoritmen deze biedbeslissingen kunnen nemen.

   Om deze gegevens te verzamelen, gaat de integratie [!DNL Analytics for Advertising Cloud] ruwe AMO IDs over die als klikthrough en mening-door het volgen codes in de dimensie van identiteitskaart AMO van Adobe Analytics kunnen worden vertaald — die of als douanevariabele (eVar) of een gereserveerde variabele (rVar) wordt opgeslagen. Doorklikken voor andere kanalen wordt niet ingesteld in de AMO ID-dimensie, zodat de AMO ID-dimensie de invoer van deze andere kanalen niet kan bijhouden. Het resultaat is dat de AMO-id doorloopt tot en met [!DNL Marketing Channes]l-ingangspunten.

Zie &quot;[Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](../data-variances.md)&quot; voor meer informatie over mogelijke gegevensvariaties tussen door Advertising Cloud bijgehouden gegevens en [!DNL Analytics] bijgehouden gegevens.

>[!MORELIKETHIS]
>
>* [Gegevensvariaties  [!DNL Analytics] tussen en Advertising Cloud verwacht](/help/integrations/analytics/data-variances.md)
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Advertising Cloud-id&#39;s gebruiken om  [!DNL Marketing Channels] CreateProcessing-regels te maken](mc-ids.md)
>* [Advertising Cloud-gegevens  [!DNL Analytics Marketing Channels] gebruiken](mc-ac-data.md)
>* [Video: Rapporten met Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)

