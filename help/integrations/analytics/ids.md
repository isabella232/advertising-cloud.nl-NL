---
title: Advertising Cloud-id's gebruikt door [!DNL Analytics]
description: Advertising Cloud-id's gebruikt door [!DNL Analytics]
feature: Integration with Adobe Analytics
exl-id: ed1aab7b-9bd0-4d42-9bfb-9c6fa6db76bc
source-git-commit: 7cb39998041d151ece7809adc8a2e872b922e5fc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Van toepassing op Advertising Cloud DSP en Advertising Cloud Search*

Advertising Cloud gebruikt twee id&#39;s voor het on-site bijhouden van prestaties: de *EF-id* en de *AMO-id*.

Wanneer een advertentie-impositie optreedt, maakt Advertising Cloud de waarden voor de AMO-id en EF-id en slaat het deze op. Wanneer een bezoeker die een advertentie heeft gezien, de site betreedt zonder op een advertentie te klikken, [!DNL Analytics] roept deze waarden van Advertising Cloud door [!DNL Analytics for Advertising Cloud] JavaScript-code. Voor doorkijkverkeer, [!DNL Analytics] Hiermee wordt een aanvullende id gegenereerd (`SDID`), dat wordt gebruikt om de EF-id en de AMO-id in te voegen [!DNL Analytics]. Voor doorklikverkeer worden deze id&#39;s opgenomen in de URL van de bestemmingspagina met behulp van de `s_kwcid` en `ef_id` querytekenreeksparameters.

Advertising Cloud maakt een onderscheid tussen een doorklikitem of een doorkijkitem op de website aan de hand van de volgende criteria:

* Een view-through ingang wordt gevangen wanneer een gebruiker de plaats na het bekijken van een advertentie bezoekt maar niet het klikt. [!DNL Analytics] registreert een mening-door als twee voorwaarden worden voldaan:
   * De bezoeker heeft geen doorklikken voor een [!DNL DSP] of [!DNL Search] advertentie tijdens de [klik terugkijkvenster](#lookback-a4adc).
   * De bezoeker heeft minstens één [!DNL DSP] advertentie tijdens de [terugkijkvenster van indruk](#lookback-a4adc). De laatste indruk wordt doorgegeven als de doorkijkhoek.
* Een doorklikitem wordt vastgelegd wanneer een sitebezoeker op een advertentie klikt voordat hij de site betreedt. [!DNL Analytics] vangt een klik-door wanneer één van beiden van de volgende voorwaarden voorkomt:
   * De URL bevat een EF-id en een AMO-id die Advertising Cloud aan de URL van de bestemmingspagina heeft toegevoegd.
   * De URL bevat geen volgcodes, maar de Advertising Cloud JavaScript-code detecteert een klik binnen de laatste twee minuten.

![Op Advertising Cloud gebaseerde weergave [!DNL Analytics] integratie](/help/integrations/assets/a4adc-view-through-process.png)

*Afbeelding 1: Op Advertising Cloud gebaseerde weergave [!DNL Analytics] integratie*

![Advertising Cloud klikken op URL [!DNL Analytics] integratie](/help/integrations/assets/a4adc-click-through-process.png)

*Afbeelding 2: Advertising Cloud klikken op URL [!DNL Analytics] integratie*

## Advertising Cloud EF-id&#39;s

De EF-id is een unieke token die Advertising Cloud gebruikt om activiteit te koppelen aan een online klik of advertentie. De EF-id wordt opgeslagen in een [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) of rVar (gereserveerde eVar) afmeting (Advertising Cloud EF ID) en houdt elke advertentie of blootstelling op het individuele browser of apparatenniveau bij. EF-id&#39;s fungeren voornamelijk als sleutels voor het verzenden [!DNL Analytics] gegevens naar Advertising Cloud voor rapportage en optimalisatie van biedingen in Advertising Cloud.

### EF-id-indeling

>[!NOTE]
>
>EF-id&#39;s zijn hoofdlettergevoelig. Als een [!DNL Analytics] bij de implementatie wordt URL-registratie naar kleine letters gedwongen, zodat Advertising Cloud de EF-id niet herkent. Dit heeft invloed op Advertising Cloud-biedingen en -rapportage, maar heeft geen invloed op Advertising Cloud-rapportage binnen [!DNL Analytics].

#### [!DNL Google Ads] zoekadvertenties

```{gclid}:G:s```

waarbij:

* `gclid` is de [!DNL Google Click ID] (GCLID).
* `s` is het netwerktype (&quot;s&quot; voor onderzoek).

#### Microsoft Adverteren, zoekadvertenties

```{msclkid}:G:s```

waarbij:

* `msclkid` is de [!DNL Microsoft Click ID] (MSCLKID).
* `s` is het netwerktype (&quot;s&quot; voor onderzoek).

#### Advertenties en zoekadvertenties weergeven op andere zoekmachines

```<Advertising Cloud visitor ID>:<timestamp>:<channel type>```

<!-- <*Advertising Cloud visitor ID*>:<*timestamp*>:<*channel type*> -->

waarbij:

* &lt;*Advertising Cloud-bezoeker-id*> is een unieke id per bezoeker (zoals EhKVaAABCkJ0mDt). Wordt ook de *surfer-id*.

* &lt;*tijdstempel*> is de tijd in de notatie YYYYMMDDHHMMSS (zoals 20190821192533 voor 2019, maand 08, dag 21, tijd 19):25:33).

* &lt;*kanaaltype*> is het kanaaltype dat verantwoordelijk is voor de klik of de blootstelling:

   * `d` voor een klik op een DSP (klik-door tonen)
   * `i` voor een indruk van een DSP (display view-through)
   * `s` voor een klik op een zoekadvertentie (doorzoeken door te klikken).

Voorbeeld `EF `ID: WcmibgAAHJK1RyY:1551968087687:d

### De EF ID Dimension in [!DNL Analytics]

In [!DNL Analytics] rapporten, kunt u EF-ID-gegevens vinden door te zoeken naar de [!UICONTROL EF ID] dimensie en het gebruik van de [!UICONTROL EF ID Instance] metrisch.

Voor EF-id&#39;s geldt de limiet van 500 kB voor unieke identificatiekenmerken in Analysis Workspace. Zodra de waarde van 500 k is bereikt, worden alle nieuwe volgcodes gerapporteerd onder de titel van één regel-item &quot;[!UICONTROL Low Traffic].&quot; Omdat het mogelijk is dat de rapportbetrouwbaarheid ontbreekt, worden de EF-id&#39;s niet geclassificeerd en mag u deze niet gebruiken voor segmenten of voor rapportage in [!DNL Analytics].

## Advertising Cloud AMO-id&#39;s

De AMO-id volgt elke unieke advertentiecombinatie op een minder granulair niveau en wordt gebruikt voor [!DNL Analytics] gegevensclassificatie en opname van advertentiemetriek (zoals indrukken, klikken en kosten) van Advertising Cloud. De AMO-id is opgeslagen in een [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) of de rVar-dimensie (AMO-id) en wordt uitsluitend gebruikt voor rapportage in [!DNL Analytics].

De AMO-id wordt ook wel de `s_kwcid`, die soms wordt uitgesproken als &quot;[!DNL the squid].&quot;

### AMO ID-indeling voor [!DNL DSP]

```<Channel ID>!<Ad ID>!<Placement ID>```

waarbij:

* &lt;*Kanaal-id*> kan:

   * `AC` = Advertising Cloud DSP
   * `AL` voor Advertising Cloud Search

* &lt;*ID advertentie*> wordt gebruikt als door Advertising Cloud gegenereerde unieke id voor een advertentie. Het dient als sleutel voor het omzetten van metagegevens van Advertising Cloud-entiteiten in leesbaar [!DNL Analytics] afmetingen.

* &lt;*Plaatsing-id*> is een door Advertising Cloud gegenereerde unieke id voor een plaatsing. Het dient als sleutel voor het omzetten van metagegevens van Advertising Cloud-entiteiten in leesbaar [!DNL Analytics] afmetingen.

<!-- <*Channel ID*>!<*Ad ID*>!<*Placement ID*>

where:

* <*Channel ID*> may be:

    * `AC` = Advertising Cloud DSP
    * `AL` for Advertising Cloud Search

* <*Ad ID*> is used an Advertising Cloud-generated unique identifier for an ad. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.

* <*Placement ID*> is an Advertising Cloud-generated unique identifier for an placement. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.
 -->

Voorbeeld-AMO-id: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

### AMO ID-indeling voor [!DNL Search]

AMO-id&#39;s voor [!DNL Search] voor elk zoekprogramma een aparte indeling gebruiken. De indeling voor alle zoekmachines begint met het volgende:

```AL!{ef_userid}!{ef_sid}```

waarbij:

* `AL` is de kanaal-id voor het zoekkanaal.
* `{ef_userid}` Dit is de unieke numerieke gebruikersnaam die Advertising Cloud aan de adverteerder toewijst.
* `{ef_sid}` is de numerieke id die Advertising Cloud gebruikt voor het opgegeven zoekprogramma, zoals `3` for [!DNL Google Ads] of `10` for [!DNL Microsoft Advertising].

Hieronder ziet u de volledige AMO ID-indelingen voor een aantal zoekprogramma&#39;s. Neem voor AMO ID-indelingen voor andere zoekprogramma&#39;s contact op met uw [!DNL Adobe] accountteam.

AMO ID-indeling voor [!DNL Google Ads]:

```AL!{ef_userid}!{ef_sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}```

waarbij:

* `{creative}` is de [!DNL Google Ads] unieke numerieke id voor creatieve doeleinden.
* `{matchtype}` is het matchype van het sleutelwoord dat de advertentie teweegbracht: `e` voor exact, `p` voor woordgroep, of `b` voor het algemeen.
* `{placement}` Dit is de domeinnaam van de website waarop op de advertentie is geklikt. Er is een waarde beschikbaar voor advertenties in op plaatsing gerichte campagnes en voor advertenties in op trefwoorden gerichte campagnes die op inhoudssites worden weergegeven.
* `{network}` Hiermee wordt het netwerk aangegeven vanwaar de klik heeft plaatsgevonden:  `g` for [!DNL Google] zoeken (alleen voor advertenties die op trefwoorden zijn gericht), `s` voor een zoekpartner (alleen voor advertenties die op trefwoorden zijn gericht), of `d` voor het Netwerk van de Vertoning (voor of sleutelwoord-gericht of plaatsing-gerichte advertenties).
* `{keyword}` is of het specifieke sleutelwoord dat uw advertentie (op onderzoeksplaatsen) of het best-passende sleutelwoord (op inhoudsplaatsen) teweegbracht.

AMO ID-indeling voor [!DNL Microsoft Advertising]:

```AL!{ef_userid}!{ef_sid}!{AdId}!{OrderItemId}```

waarbij:

* `{AdId}` is de [!DNL Microsoft Advertising] unieke numerieke id voor creatieve doeleinden.
* `{OrderItemId}` is de [!DNL Microsoft Advertising] numerieke id voor het trefwoord.

### AMO ID-Dimension in [!DNL Analytics]

In analyserapporten kunt u zoeken naar AMO ID-gegevens [!UICONTROL AMO ID] dimensie en het gebruik van de [!UICONTROL AMO ID Instance] metrisch. De [!UICONTROL AMO ID] dimensie bevat alle vastgelegde AMO-id-waarden, terwijl de [!UICONTROL AMO ID Instance] De metrische waarde geeft aan hoe vaak een AMO-id-waarde door de site is vastgelegd. Als bijvoorbeeld vier keer op dezelfde zoekopdracht is geklikt, maar Analytics zeven sitems heeft bijgehouden, [!UICONTROL AMO ID Instance] zou zeven (7) zijn en [!UICONTROL Clicks] zou vier (4) zijn.

Voor elke rapportage of controle binnen [!DNL Analytics]De beste manier is om de AMO-id samen met het bijbehorende exemplaar te gebruiken. Zie voor meer informatie &quot;[Gegevensvalidatie voor [!DNL Analytics for Advertising Cloud]](data-variances.md#data-validation)&quot; in &quot;Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud.&quot;

## Informatie over analytische classificaties

In [!DNL Analytics], [classificatie](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html) is een stuk van meta-gegevens voor een bepaalde het volgen code, zoals Rekening, Campagne, of Advertentie. Advertising Cloud categoriseert onbewerkte Advertising Cloud-gegevens aan de hand van classificaties, zodat u de gegevens op verschillende manieren kunt weergeven (bijvoorbeeld op Advertentietype of Campagne) wanneer u rapporten genereert. Classificaties vormen de basis voor Advertising Cloud-rapportage in [!DNL Analytics] en kan worden gebruikt met de AMO-metriek, zoals [!UICONTROL AMO Cost], [!UICONTROL AMO Impressions], en [!UICONTROL AMO Clicks]en met aangepaste en standaard onsite gebeurtenissen zoals [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders], en [!UICONTROL Revenue].

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud](data-variances.md)

