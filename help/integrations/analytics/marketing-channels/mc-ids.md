---
title: Advertising Cloud-id's gebruiken om [!DNL Marketing Channels] regels te maken
description: Leer hoe te om Advertising Cloud IDs te gebruiken om verwerkingsregels voor  [!DNL Analytics Marketing Channels] tot stand te brengen.
feature: Integration with Adobe Analytics
exl-id: null
source-git-commit: 5224d891d665b901d076ff6a203e9ff3bab80f85
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Advertising Cloud-id&#39;s gebruiken om [!DNL Marketing Channels] verwerkingsregels te maken

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

U kunt Advertising Cloud-id&#39;s ([AMO-id en EF-id](../ids.md)) gebruiken om [!DNL Marketing Channels]-verwerkingsregels te configureren in Adobe Analytics. Gebruik Advertising Cloud-id&#39;s voor specifieke regels voor Advertising Cloud-campagnes.

## De AMO-id in verwerkingsregels

De AMO-id is de primaire trackingcode die wordt gebruikt om Advertising Cloud-gegevens te rapporteren binnen [!DNL Analytics]. De AMO-id is een aaneenschakeling van dynamische waarden die door Adobe worden beheerd voor korrelige rapportage binnen [!DNL Analytics]. Het wordt opgeslagen in een [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) of rVar afmeting (identiteitskaart van AMO). De AMO-id kan op twee manieren worden ingesteld:[!DNL Analytics]

* Doorklikken: Advertising Cloud stelt de parameter van de `s_kwcid` vraagtekenreeks in een verbinding in, en [!DNL Analytics] neemt de parameter van de bestemmingspagina URL op wanneer een klik-door voorkomt.
* Beeld-door het volgen ([!DNL DSP] slechts): De laatste gebeurtenisservice detecteert een doorzicht aan de serverzijde en verzendt de AMO-id naar [!DNL Analytics]. In dit geval bevat de URL geen parameter `s_kwcid`.

De dynamische waarden binnen AMO-id&#39;s geven het marketingkanaal aan dat is bijgehouden:

* Het voorvoegsel in de AMO-id kan worden gebruikt om het kanaal op hoofdniveau binnen [!DNL Marketing Channels] te identificeren.

* Tekenzinnen in de hoofdtekst van de AMO-id geven een specifieker campagneretype aan.

* Het achtervoegsel &quot;vt&quot;is aanwezig voor [!DNL DSP] mening-door verkeer en kan worden gebruikt om afzonderlijke klik-door en mening-door [!DNL DSP] kanalen tot stand te brengen.

De rest van de AMO-id kan worden genegeerd.

| AMO-id | Kanaal | Regellogica |
|--------|---------|--------------------|
| AL! (voorvoegsel) | [!UICONTROL Paid Search] | Begint met |
| AC! (voorvoegsel) | [!UICONTROL DSP] | Begint met |
| !g! (body) | [!UICONTROL Google Search] | Bevat |
| !s! (body) | [!UICONTROL Search Partner] | Bevat |
| !d! (body) | [!UICONTROL Display Network] | Bevat |
| !u! (body) | [!UICONTROL Smart Shopping Campaign] | Bevat |
| !ytv! (body) | [!UICONTROL YouTube Video Ad] | Bevat |
| !yts! (body) | [!UICONTROL YouTube Search Ad] | Bevat |
| !vp! (body) | [!UICONTROL Google Video Partners] | Bevat |
| !vt (achtervoegsel) | [!UICONTROL DSP View-through] | Eindigt met |

### Voorbeelden van verwerkingsregels die de AMO-id gebruiken

De [!DNL Marketing Channels] verwerkingsregel voor het [!UICONTROL Paid Search] kanaal zou als dit kunnen kijken:

![Voorbeeld van een  [!UICONTROL Paid Search] regel](/help/integrations/assets/a4adc-mc-rule-paidsearch.png)

De [!DNL Marketing Channels] verwerkingsregel voor het [!UICONTROL YouTube Video Ads] kanaal zou als dit kunnen kijken:

![Voorbeeld van een  [!UICONTROL YouTube Video Ads] regel](/help/integrations/assets/a4adc-mc-rule-youtube-video.png)

>[!IMPORTANT]
>
> Ben zeker om uw regels in volgorde van specificiteit in werking te stellen. Als de bovenstaande twee regels in orde waren, zouden de [!DNL YouTube] video en het verkeer allen onder het [!UICONTROL Paid Search] kanaal vallen omdat AMO identiteitskaart allebei met &quot;AL zou beginnen!&quot; en bevatten &quot;!ytv!&quot;.

## EF-id in verwerkingsregels

De EF-id (EF-id) van AMO is de tweede trackingcode die wordt gebruikt in de integratie [!DNL Analytics for Advertising Cloud]. Het hoofddoel is het bijhouden en doorgeven van [!DNL Analytics]-gebeurtenisgegevens aan Advertising Cloud. Telkens wanneer een klik-door of een mening-door voorkomt, wordt een unieke EF identiteitskaart geproduceerd, zelfs als het de nauwkeurige zelfde advertentie voor de zelfde bezoeker is. De EF-id wordt niet gebruikt in de [!DNL Analytics] die gebruikersinterface rapporteren omdat deze doorgaans de unieke waarden van 500 kB per variabele in [!DNL Analytics] overschrijdt, waardoor deze onbruikbaar wordt voor rapportage. De Advertising Cloud-meetgegevens en -metagegevens worden niet toegepast op de EF-id. ze worden alleen toegepast op de AMO-id. De toegevoegde granulariteit van het volgen is vereist voor campagtimalisatie in Advertising Cloud, zodat worden beide IDs vereist.

Hoewel de EF-id-dimensie niet rechtstreeks wordt gebruikt in [!DNL Analytics]-rapportage, kan de EF-id nuttig zijn bij het maken van marketingkanalen. Het EF-id-achtervoegsel geeft het kanaal (weergave of zoekopdracht) aan en geeft aan of het bezoek is aangestuurd door een doorklik of een doorzicht. Het scheidingsteken in de EF-id is een dubbele punt in plaats van het uitroepteken in de AMO-id.

| Achtervoegsel EF-ID | Kanaal |
|-------|---------|
| :s | [!UICONTROL Paid Search] |
| :d | [!UICONTROL Display Click-through] |
| :i | [!UICONTROL Display View-through] |

### Voorbeelden van verwerkingsregels die gebruikmaken van de EF-id

#### Doorklikregel weergeven

Maak een marketingkanaal Doorklikken weergeven door alleen doorklikbewerkingen vast te leggen. Omdat AMO ID het zelfde voor zowel klik-door als mening-door is, gebruikt deze regel de EF veranderlijke identiteitskaart en de `ef_id` parameter van het vraagkoord.

Soms worden doorklikkingen gevolgd door URL (het gebrek). In andere gevallen worden doorklikbewerkingen bijgehouden via de laatste gebeurtenisservice aan de serverzijde. De URL bevat daarom niet de parameter `ef_id`. De regel controleert daarom voorwaarden waarin de EF identiteitskaart variabele of `ef_id` de parameter van het vraagkoord met &quot;:d&quot;beëindigt. Gebruik &quot;`Any`&quot;exploitant omdat u deze regel voor één van beide voorwaarde wilt teweegbrengen.

![Voorbeeld van een klikregel voor weergave](/help/integrations/assets/a4adc-mc-rule-display-ct.png)

#### Weergave-through-regel

Maak een regel waarin de EF-id eindigt met &quot;:i&quot; om een weergavedoorvoerkanaal te maken. Omdat de bezoeker niet op de advertentie heeft geklikt, bevat de doorkijkbewerking `ef_id` of `s_kwcid` niet in de URL. Daarom is slechts één voorwaarde nodig.

![Voorbeeld van een weergaveregel](/help/integrations/assets/a4adc-mc-rule-display-vt.png)

>[!MORELIKETHIS]
>
>* [Grondbeginselen van [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Waarom kanaalgegevens kunnen variëren tussen Advertising Cloud en [!DNL Marketing Channels]](mc-data-variances.md)
>* [Advertising Cloud-gegevens  [!DNL Analytics Marketing Channels] gebruiken](mc-ac-data.md)
>* [Video: Rapporten met Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]](/help/integrations/analytics/ids.md)

