---
title: Grondbeginselen van [!DNL Marketing Channels]
description: Leer zeer belangrijke informatie over [!DNL Analytics Marketing Channels] that [!DNL Analytics for Advertising Cloud] gebruikers zouden moeten begrijpen.
feature: Integration with Adobe Analytics
exl-id: null
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Grondbeginselen van [!DNL Analytics Marketing Channels]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Deze pagina bevat belangrijke informatie over [!DNL Analytics Marketing Channels] die [!DNL Analytics for Advertising Cloud] gebruikers moeten begrijpen.

Voor volledige documentatie op [!DNL Marketing Channels], zie &quot;[Aan de slag met [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/c-getting-started-mchannel.html).&quot;

## Overzicht van [!DNL Marketing Channels]

[!DNL Marketing Channels] zijn een belangrijke functie van Adobe Analytics. [!DNL Marketing Channels] In rapporten ziet u hoe klanten via het rapportagevenster naar uw website komen en hoe elk kanaal invloed heeft op de inkomsten of het gedrag op de locatie.

Neem bijvoorbeeld het volgende voorbeeld van een reis tijdens een kruisbezoek. Elk bezoek aan uw website wordt aangegeven door het marketingkanaal van waaruit de bezoeker is gekomen. Het eerste bezoek, ook wel First Touch Channel genoemd, is E-mail. Weergeven bij bezoek twee is een deelnemend kanaal en Natuurlijk zoeken wordt beschouwd als het laatste aanraakkanaal. Als u [!UICONTROL Last Touch Attribution] binnen [!UICONTROL Attribution IQ] gebruikt, zou Natuurlijk Onderzoek volledige krediet voor de $250 omzettingsgebeurtenis ontvangen. Met de Experience Cloud ID-service kunt u deze individuele bezoeken aan elkaar koppelen om één reis van één bezoeker te onthullen.

![Voorbeeld van een reis naar conversie tussen bezoeken in marketingkanalen](/help/integrations/assets/a4adc-mc-sample-journey.png)

Door [!UICONTROL Marketing Channels] Regels van de Verwerking te gebruiken, kunt u reeksen logica tot stand brengen om de kanalen te bepalen die verkeer drijven en elk kanaal te volgen aangezien de gebruikers naar uw plaats komen. Het kanaal [!UICONTROL Email] zou bijvoorbeeld worden aangegeven met een unieke trackingcode die wordt gegenereerd wanneer u op dit moment klikt. Als u het kanaal door Adobe Analytics hebt geregistreerd, wordt het bezoek gecategoriseerd als afkomstig van een marketingcampagne voor e-mail.

## De Regels van de verwerking en hoe de Kanalen van de Marketing worden geplaatst

Elke keer dat een gebruiker naar een website komt, doet hij dat via een URL waarop hij of zij heeft geklikt of die hij of zij rechtstreeks in de adresbalk heeft getypt. Wanneer de gebruiker de website ingaat, [!DNL Analytics] houdt informatie bij die kan worden gebruikt om het kanaal te bepalen dat het bezoek leidde.

Vaak voegen marketers code voor het bijhouden van querytekenreeksparameters toe aan kanaal-URL&#39;s om het effect van het kanaal op hun site te volgen. U kunt [!DNL Marketing Channels] verwerkingsregels vormen om naar specifieke volgende parameters en waarden te luisteren om het kanaal zonder enige extra het volgen te bepalen. Bijvoorbeeld, als alle e-mailcampagne URLs het formaat `www.adobe.com?cid=email…` (waar URL de parameter en de waarde `cid=email` van het vraagkoord bevat) volgen, dan kunt u een regel tot stand brengen om naar deze het volgen code te luisteren en het bezoek in [!UICONTROL Email] kanaal te emmeren.

Andere kanalen hebben geen trackable wegen URL en hebben verdere logica voor identificatie nodig. [!UICONTROL Earned Social], bijvoorbeeld, waarin een gebruiker op een verbinding klikt die een andere gebruiker organisch op een sociaal netwerk deelde, is een belangrijk kanaal om te volgen. Nochtans, heeft de teller geen manier om een parameter het volgen code van het vraagkoord aan URL toe te voegen die wordt gedeeld. In dit geval kunt u een verwerkingsregel maken om te luisteren naar het verwijzende domein van sociale netwerken van interesse en naar het ontbreken van betaalcodes om het kanaal te bepalen. De bezoeken die aan deze vereisten voldoen zouden dan als Verdiende Sociale binnen het rapport van de Kanalen van de Marketing worden gevolgd.

Adobe raadt u aan samen te werken met uw analyseteam om een uitgebreide set [!DNL Marketing Channels] verwerkingsregels te maken om alle kanalen te volgen die relevant zijn voor uw bedrijf. Zo kunt u krachtige rapportage van toewijzingen maken.

Als u wilt begrijpen hoe Advertising Cloud kan bijdragen aan de signalen die nodig zijn om aangepaste marketingkanalen te maken, raadpleegt u &quot;[Advertising ID&#39;s gebruiken voor Maken [!DNL Marketing Channels] Rules](mc-ids.md)&quot;.

>[!MORELIKETHIS]
>
>* [Advertising Cloud-id&#39;s gebruiken om  [!DNL Marketing Channels] CreateProcessing-regels te maken](mc-ids.md)
>* [Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]](mc-data-variances.md)
>* [Advertising Cloud-gegevens  [!DNL Analytics Marketing Channels] gebruiken](mc-ac-data.md)
>* [Video: Rapporten met Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](/help/integrations/analytics/overview.md)

