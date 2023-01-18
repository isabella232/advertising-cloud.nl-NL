---
title: Gebruiken [!DNL Marketing Channels] met Adobe-advertentiegegevens
description: Leer hoe u Adobe-advertentiegegevens kunt gebruiken in [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Gebruiken [!DNL Analytics Marketing Channels] met Adobe-advertentiegegevens

*Adverteerders met een Adobe Advertising-Adobe Analytics Integration Only*

Door zowel Adobe-reclame als [!DNL Analytics Marketing Channels] rapporten, kunt u waardevol inzicht in krijgen hoe uw digitale media plaatsactiviteit beïnvloedt.

<!-- from video: By using Marketing Channels with your Adobe Advertising data, you can get a more holistic view of how your advertising efforts are affecting site behavior. In particular, you can see the value of your view-through and click-through data, and how your advertising assists or is assisted by other channels. -->

In de volgende afbeelding ziet u hoe Adobe Advertising en [!DNL Marketing Channels] de individuele bezoeken van één bezoeker volgen. Adobe Reclamerapporten in [!DNL Analytics] beperkt zich tot alleen betaalde reclame voor display, search, social en commerce die via Adobe Advertising via de AMO-id wordt verhandeld. Maar [!DNL Marketing Channels] volgt alle kanalen die in [!DNL Marketing Channels] Verwerkingsregels.

![Hoe Adobe-reclame en [!DNL Marketing Channels] individuele bezoeken op de reis van een bezoeker volgen](/help/integrations/assets/a4adc-mc-sample-journey2.png)

Tijdens het eerste bezoek heeft de gebruiker de website ingevoerd via een e-mailcampagne, tien paginaweergaven uitgevoerd en vervolgens vertrokken. Tijdens het tweede bezoek heeft de gebruiker de site ingevoerd via een advertentie, tien paginaweergaven uitgevoerd en vervolgens links. Tijdens het derde bezoek heeft de gebruiker de site betreden via een natuurlijke zoekopdracht, vijf paginaweergaven uitgevoerd, een conversie van € 250 uitgevoerd en links. Let op het verschil in reeksspatiëring tussen [!DNL Marketing Channels] en Adobe-reclame. Het enige kanaal dat Adobe Advertising volgt op deze reis is [!UICONTROL Display]. Adobe Adverteren volgt de [!UICONTROL Display] kanaalbezoek en kenmerken de daaropvolgende betrokkenheidsgegevens (zoals paginaweergaven) en conversies terug naar de invloed van die advertentie. [!DNL Marketing Channels]geeft daarentegen een volledig beeld van alle kanalen.

Omdat de AMO-id tijdens de reis van de bezoeker blijft bestaan, kunt u de AMO-id-gegevens gebruiken om te zien hoe Adobe Advertising andere marketingkanalen beïnvloedt. De AMO-id [standaard 60 dagen aanhoudt](/help/integrations/analytics/overview.md), maar u kunt de persistentie naar wens configureren.

## Hoe te om Adobe te combineren reclame en de Gegevens van de Kanalen van de Marketing om de Prestaties van Media te analyseren

Within [!DNL Analytics], kunt u de nog steeds betaalde advertentiegegevens van de Adobe combineren met de [!DNL Marketing Channels] uitgebreide bezoekgegevens om uw mediaprestaties beter te analyseren zodat u de reis van de klant beter kunt beïnvloeden.

In de volgende analyse worden de advertentiegegevens van de Adobe gebruikt om verschillende versies van de invloed van een weergaveadvertentie op de siteconversie te laten zien. Alle drie de kolommen gebruiken de zelfde omzettingsmetriek, maar elke kolom vertelt een verschillend verhaal:

* In kolom 1 worden de AMO-id-gegevens weergegeven die blijvend zijn over de reis van de bezoeker. Kolom 1 geeft aan dat 641 toepassingen op één punt zijn gekoppeld aan een advertentie voor advertentie voor Adobe-advertenties, via een doorkijkgebeurtenis of via een doorklikgebeurtenis. Deze weergave neemt geen andere [!DNL Marketing Channels] toerekening in aanmerking genomen.

* In de [!DNL Marketing Channels] de gegevensset, echter, de 641 Toepassingen begint worden toegeschreven aan andere marketing kanalen. De laatste twee kolommen nemen 641 Toepassingen begint en beperken de gegevens tot [!UICONTROL Display Click-Through] en [!UICONTROL Display View-Through] kanalen, die de omzettingen tonen die in een laatste aanraakattributiemodel voorkomen.

![voorbeeld van hoe een weergave en de conversie van sites beïnvloeden](/help/integrations/assets/a4adc-mc-display-impact.png)

U kunt deze analyse een stap verder zetten. U kunt de Adobe-advertentierij verder opsplitsen met marketingkanalen om te zien waar de Adobe Advertising-conversies worden toegewezen aan de 641 Applications Start. U weet al dat vijf van deze omzettingen worden toegeschreven aan een laatste aanraakscherm en dat er 19 worden toegewezen aan een laatste aanraakscherm. Hierdoor blijven 617 toepassingen aan andere marketingkanalen toegewezen. U kunt de afmeting Laatste aanraakkanaal boven op het DSP voor adverteren slepen om de kanaaltoewijzing voor de rest van de toepassingen zichtbaar te maken en de kanaalinvloed van het weergavekanaal te tonen.

![hoe u de afmeting Laatste aanraakkanaal toevoegt](/help/integrations/assets/a4adc-mc-display-impact-ltc.png)

Nu kunt u zien hoe de resterende Toepassingen worden toegewezen. E-mail krijgt krediet voor 357 meest recente aanraaktoepassingen Start waarvoor een AMO-id werd gebruikt. Met dit type analyse kunt u zien wat de impact was van advertenties in Adobe Advertising op alle kanalen. Met slechts één gegevensset en attributiemodel zou dit type inzicht niet beschikbaar zijn.

![voorbeeld van de kanaaleffecten van de weergavekanalen](/help/integrations/assets/a4adc-mc-display-impact-x-channel.png)

U kunt de analyse verder verbeteren door een Stapelgrafiek te gebruiken die aan &quot;100% wordt geplaatst gestapeld&quot;om trended gegevens in tijd te tonen. Dankzij deze visualisatie kunt u gemakkelijker controleren welke laatste aanraakmarketingkanalen zwaarder worden beïnvloed door uw marketingcampagnes voor beeldschermen.

![voorbeeld van de trendale invloed van de kanalen van de Vertoning](/help/integrations/assets/a4adc-mc-display-impact-x-channel-trend.png)

>[!MORELIKETHIS]
>
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Adobe-advertentie-id&#39;s gebruiken om te maken [!DNL Marketing Channels] Verwerkingsregels](mc-ids.md)
>* [Waarom kanaalgegevens kunnen verschillen tussen Adobe-reclame en [!DNL Marketing Channels]](mc-data-variances.md)
>* [Video: Gebruiken [!DNL Marketing Channels] voor Adobe Advertising Reporting](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Overzicht van [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)

