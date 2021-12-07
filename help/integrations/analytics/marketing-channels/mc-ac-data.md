---
title: Gebruiken [!DNL Marketing Channels] met Advertising Cloud-gegevens
description: Meer informatie over het gebruik van Advertising Cloud-gegevens in [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
source-git-commit: 1ae45d0ceee2efc4fc52b86fd6737d4c7467a6ca
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Gebruiken [!DNL Analytics Marketing Channels] met Advertising Cloud-gegevens

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Door zowel de Advertising Cloud als [!DNL Marketing Channels] rapporten, kunt u waardevol inzicht in krijgen hoe uw digitale media plaatsactiviteit beïnvloedt.

<!-- from video: By using Marketing Channels with your Advertising Cloud data, you can get a more holistic view of how your advertising efforts are affecting site behavior. In particular, you can see the value of your view-through and click-through data, and how your advertising assists or is assisted by other channels. -->

In de volgende afbeelding ziet u hoe Advertising Cloud en [!DNL Marketing Channels] de individuele bezoeken van één bezoeker volgen. Advertising Cloud-rapporten in [!DNL Analytics] beperkt zijn tot alleen betaalde uitgeverij- en zoekadvertenties die via Advertising Cloud worden verhandeld, met behulp van de AMO-id. Maar [!DNL Marketing Channels] volgt alle kanalen die in [!DNL Marketing Channels] Verwerkingsregels.

![Hoe Advertising Cloud en [!DNL Marketing Channels] individuele bezoeken op de reis van een bezoeker volgen](/help/integrations/assets/a4adc-mc-sample-journey2.png)

Tijdens het eerste bezoek heeft de gebruiker de website ingevoerd via een e-mailcampagne, tien paginaweergaven uitgevoerd en vervolgens vertrokken. Tijdens het tweede bezoek heeft de gebruiker de site ingevoerd via een advertentie, tien paginaweergaven uitgevoerd en vervolgens links. Tijdens het derde bezoek heeft de gebruiker de site betreden via een natuurlijke zoekopdracht, vijf paginaweergaven uitgevoerd, een conversie van € 250 uitgevoerd en links. Let op het verschil in reeksspatiëring tussen [!DNL Marketing Channels] en Advertising Cloud. Het enige kanaal dat Advertising Cloud in deze reis volgt, is [!UICONTROL Display]. Advertising Cloud volgt de [!UICONTROL Display] kanaalbezoek en kenmerken de daaropvolgende betrokkenheidsgegevens (zoals paginaweergaven) en conversies terug naar de invloed van die advertentie. [!DNL Marketing Channels]geeft daarentegen een volledig beeld van alle kanalen.

Omdat de AMO-id tijdens de reis van de bezoeker blijft bestaan, kunt u de AMO-id-gegevens gebruiken om te zien hoe Advertising Cloud andere marketingkanalen beïnvloedt. De AMO-id [standaard 60 dagen aanhoudt](/help/integrations/analytics/overview.md), maar u kunt de persistentie naar wens configureren.

## Hoe te om de Gegevens van de Kanalen van Advertising Cloud en van de Marketing te combineren om de Prestaties van Media te analyseren

Within [!DNL Analytics], kunt u de Advertising Cloud-gegevens die nog betaalbaar zijn, combineren met de [!DNL Marketing Channels] uitgebreide bezoekgegevens om uw mediaprestaties beter te analyseren zodat u de reis van de klant beter kunt beïnvloeden.

In de volgende analyse worden de Advertising Cloud-gegevens gebruikt om verschillende versies weer te geven van de invloed van een weergaveadvertentie op siteconversie. Alle drie de kolommen gebruiken de zelfde omzettingsmetriek, maar elke kolom vertelt een verschillend verhaal:

* In kolom 1 worden de AMO-id-gegevens weergegeven die blijvend zijn over de reis van de bezoeker. Kolom 1 geeft aan dat 641 toepassingen op één punt zijn gekoppeld aan een Advertising Cloud-advertentie, via een doorkijkgebeurtenis of via een doorklikgebeurtenis. Deze weergave neemt geen andere [!DNL Marketing Channels] toerekening in aanmerking genomen.

* In de [!DNL Marketing Channels] de gegevensset, echter, de 641 Toepassingen begint worden toegeschreven aan andere marketing kanalen. De laatste twee kolommen nemen 641 Toepassingen begint en beperken de gegevens tot [!UICONTROL Display Click-Through] en [!UICONTROL Display View-Through] kanalen, die de omzettingen tonen die in een laatste aanraakattributiemodel voorkomen.

![voorbeeld van hoe een weergave en de conversie van sites beïnvloeden](/help/integrations/assets/a4adc-mc-display-impact.png)

U kunt deze analyse een stap verder zetten. U kunt de rij van Advertising Cloud verder door marketing kanaal verdelen om te zien waar de omzettingen van Advertising Cloud aan de 641 Beginnen van Toepassingen worden toegewezen. U weet al dat vijf van deze omzettingen worden toegeschreven aan een laatste aanraakscherm en dat er 19 worden toegewezen aan een laatste aanraakscherm. Hierdoor blijven 617 toepassingen aan andere marketingkanalen toegewezen. U kunt de afmeting Laatste aanraakkanaal boven op het Advertising Cloud DSP-regelitem slepen en neerzetten om de kanaaltoewijzing voor de rest van de toepassingen zichtbaar te maken en de kanaalinvloed van het weergavekanaal te tonen.

![hoe u de afmeting Laatste aanraakkanaal toevoegt](/help/integrations/assets/a4adc-mc-display-impact-ltc.png)

Nu kunt u zien hoe de resterende Toepassingen worden toegewezen. E-mail krijgt krediet voor 357 meest recente aanraaktoepassingen Start waarvoor een AMO-id werd gebruikt. Met dit type analyse kunt u zien wat de impact was van advertenties in Advertising Cloud op alle kanalen. Met slechts één gegevensset en attributiemodel zou dit type inzicht niet beschikbaar zijn.

![voorbeeld van de kanaaleffecten van de weergavekanalen](/help/integrations/assets/a4adc-mc-display-impact-x-channel.png)

U kunt de analyse verder verbeteren door een Stapelgrafiek te gebruiken die aan &quot;100% wordt geplaatst gestapeld&quot;om trended gegevens in tijd te tonen. Dankzij deze visualisatie kunt u gemakkelijker controleren welke laatste aanraakmarketingkanalen zwaarder worden beïnvloed door uw marketingcampagnes voor beeldschermen.

![voorbeeld van de trendale invloed van de kanalen van de Vertoning](/help/integrations/assets/a4adc-mc-display-impact-x-channel-trend.png)

>[!MORELIKETHIS]
>
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Advertising Cloud-id&#39;s gebruiken om te maken [!DNL Marketing Channels] Verwerkingsregels](mc-ids.md)
>* [Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]](mc-data-variances.md)
>* [Video: Rapporten met Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](/help/integrations/analytics/overview.md)

