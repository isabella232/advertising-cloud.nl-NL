---
title: Advertising Cloud-id's gebruikt door [!DNL Analytics]
description: Advertising Cloud-id's gebruikt door [!DNL Analytics]
feature: Integration with Adobe Analytics
exl-id: ed1aab7b-9bd0-4d42-9bfb-9c6fa6db76bc
source-git-commit: 185fc7d79798a0a3a9ad5829b701aeb53a4a47c1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Van toepassing op Advertising Cloud DSP en Advertising Cloud Search*

Advertising Cloud gebruikt twee id&#39;s voor het on-site bijhouden van prestaties:  de EF-id en de AMO-id.

Wanneer een advertentie-impositie optreedt, maakt Advertising Cloud de waarden voor de AMO-id en EF-id en slaat het deze op. Wanneer een bezoeker die een advertentie heeft gezien de plaats ingaat zonder een advertentie te klikken, [!DNL Analytics] roept deze waarden van Advertising Cloud door de code [!DNL Analytics for Advertising Cloud] JavaScript aan. Voor mening-door verkeer, [!DNL Analytics] produceert een extra identiteitskaart (`SDID`), die wordt gebruikt om EF identiteitskaart en identiteitskaart van AMO in [!DNL Analytics] te binden. Voor doorklikverkeer, zijn deze IDs inbegrepen in de bestemmingspagina URL gebruikend `s_kwcid` en `ef_id` de parameters van het vraagkoord.

Advertising Cloud maakt een onderscheid tussen een doorklikitem of een doorkijkitem op de website aan de hand van de volgende criteria:

* Een view-through ingang wordt gevangen wanneer een gebruiker de plaats na het bekijken van een advertentie bezoekt maar niet het klikt. [!DNL Analytics] registreert een mening-door als twee voorwaarden worden voldaan:
   * De bezoeker heeft geen klikthrough voor [!DNL DSP] of [!DNL Search] en tijdens [klik raadplegingsvenster](#lookback-a4adc).
   * De bezoeker heeft ten minste één [!DNL DSP] advertentie gezien tijdens het [imitatievenster](#lookback-a4adc). De laatste indruk wordt doorgegeven als de doorkijkhoek.
* Een doorklikitem wordt vastgelegd wanneer een sitebezoeker op een advertentie klikt voordat hij de site betreedt. [!DNL Analytics] vangt een klik-door wanneer één van beiden van de volgende voorwaarden voorkomt:
   * De URL bevat een EF-id en een AMO-id die Advertising Cloud aan de URL van de bestemmingspagina heeft toegevoegd.
   * De URL bevat geen volgcodes, maar de Advertising Cloud JavaScript-code detecteert een klik binnen de laatste twee minuten.

![Advertising Cloud op weergave gebaseerde  [!DNL Analytics] integratie](/help/integrations/assets/a4adc-view-through-process.png)

*Afbeelding 1: Advertising Cloud op weergave gebaseerde  [!DNL Analytics] integratie*

![Advertising Cloud klikken op URL- [!DNL Analytics] integratie](/help/integrations/assets/a4adc-click-through-process.png)

*Afbeelding 2: Advertising Cloud klikken op URL- [!DNL Analytics] integratie*

## Advertising Cloud EF-id&#39;s

De EF-id is een unieke token die Advertising Cloud gebruikt om activiteit te koppelen aan een online klik of advertentie. De EF-id wordt opgeslagen in een [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) of rVar (gereserveerde eVar) dimensie (Advertising Cloud EF-id) en houdt elke advertentie of blootstelling op het individuele browser- of apparaatniveau bij. EF-id&#39;s fungeren in eerste instantie als sleutels voor het verzenden van [!DNL Analytics]-gegevens naar Advertising Cloud voor het melden en optimaliseren van biedingen in Advertising Cloud.

### EF-id-indeling

```<Advertising Cloud visitor ID>:<timestamp>:<channel type>```

<!-- <*Advertising Cloud visitor ID*>:<*timestamp*>:<*channel type*> -->

waarbij:

* &lt;>Advertising Cloud-bezoeker-id *> is een unieke id per bezoeker (zoals EhKVaAABCkJ0mDt).* Wordt ook *surfer-id* genoemd.

* &lt;>timestamp *> is de tijd in formaat YYYYMMDDHHMMSS (zoals 20190821192533 voor Jaar 2019, Maand 08, Dag 21, Tijd 19:25:33).*

* &lt;>kanaaltype *> is het kanaaltype dat verantwoordelijk is voor de klik of de blootstelling:*

   * `d` voor een klik op een DSP (klik-door tonen)
   * `i` voor een indruk van een DSP (display view-through)
   * `s` voor een klik op een zoekadvertentie (doorzoeken door te klikken).

Voorbeeld `EF `ID: WcmibgAAHJK1RyY:1551968087687:d

>[!NOTE]
>
>EF-id&#39;s zijn hoofdlettergevoelig. Als een [!DNL Analytics]-implementatie het bijhouden van URL&#39;s in kleine letters dwingt, zal Advertising Cloud de EF-id niet herkennen. Dit zal gevolgen hebben voor Advertising Cloud-biedingen en -rapportage, maar heeft geen invloed op Advertising Cloud-rapportage binnen [!DNL Analytics].

### De EF ID-Dimension in [!DNL Analytics]

In [!DNL Analytics] rapporten, kunt u EF gegevens van identiteitskaart vinden door naar de [!UICONTROL EF ID] dimensie te zoeken en [!UICONTROL EF ID Instance] metrisch te gebruiken.

`EF IDs` zijn onderworpen aan de limiet van 500 kB voor unieke identificatoren in Analysis Workspace. Zodra de waarde van 500k wordt bereikt, worden alle nieuwe volgcodes gerapporteerd onder de one-line-item titel &quot;[!UICONTROL Low Traffic]&quot;. Vanwege de mogelijkheid dat rapportprecisie ontbreekt, worden `EF IDs` niet geclassificeerd, en u zou hen niet voor segmenten of rapportering in [!DNL Analytics] moeten gebruiken.

## Advertising Cloud AMO-id&#39;s

De AMO-id houdt elke unieke advertentiecombinatie bij op een kleiner korrelig niveau en wordt gebruikt voor [!DNL Analytics] gegevensclassificatie en opname van advertentiemetriek (zoals indrukken, klikken en kosten) van Advertising Cloud. De AMO-id wordt opgeslagen in een [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html)- of rVar-dimensie (AMO-id) en wordt uitsluitend gebruikt voor rapportage in [!DNL Analytics].

De AMO-id wordt ook de `s_kwcid` genoemd. Deze wordt ook wel &#39;de inktvis&#39; genoemd.

### AMO ID-indeling voor [!DNL DSP]

```<Channel ID>!<Ad ID>!<Placement ID>```

waarbij:

* &lt;>Kanaal-id *> kan zijn:*

   * `AC` = Advertising Cloud DSP
   * `AL` voor Advertising Cloud Search

* &lt;>Advertentie-ID *> wordt gebruikt een door Advertising Cloud gegenereerde unieke id voor een advertentie.* Deze functie dient als sleutel voor het omzetten van metagegevens van Advertising Cloud-entiteiten in leesbare [!DNL Analytics]-afmetingen.

* &lt;>Plaatsing-id *> is een unieke id die door Advertising Cloud is gegenereerd voor een plaatsing.* Deze functie dient als sleutel voor het omzetten van metagegevens van Advertising Cloud-entiteiten in leesbare [!DNL Analytics]-afmetingen.

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

AMO-id&#39;s voor [!DNL Search] hebben een aparte indeling voor elk zoekprogramma. De indeling voor alle zoekmachines begint met het volgende:

```AL!{ef_userid}!{ef_sid}```

waarbij:

* `AL` is de kanaal-id voor het zoekkanaal.
* `{ef_userid}` Dit is de unieke numerieke gebruikersnaam die Advertising Cloud aan de adverteerder toewijst.
* `{ef_sid}` is de numerieke id die Advertising Cloud gebruikt voor het opgegeven zoekprogramma, bijvoorbeeld  `3` voor  [!DNL Google Ads] of  `10` voor  [!DNL Microsoft Advertising].

Hieronder ziet u de volledige AMO ID-indelingen voor een aantal zoekprogramma&#39;s. Neem contact op met uw Adobe-accountmanager voor AMO ID-indelingen voor andere zoekprogramma&#39;s.

AMO ID-indeling voor [!DNL Google Ads]:

```AL!{ef_userid}!{ef_sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}```

waarbij:

* `{creative}` Dit is de  [!DNL Google Ads] unieke numerieke id voor creatieve projecten.
* `{matchtype}` is het matchype van het sleutelwoord dat de advertentie teweegbracht:  `e` voor nauwkeurig,  `p` voor uitdrukking, of  `b` voor breed.
* `{placement}` Dit is de domeinnaam van de website waarop op de advertentie is geklikt. Er is een waarde beschikbaar voor advertenties in op plaatsing gerichte campagnes en voor advertenties in op trefwoorden gerichte campagnes die op inhoudssites worden weergegeven.
* `{network}` Hiermee wordt het netwerk aangegeven vanwaar de klik heeft plaatsgevonden:   `g` voor  [!DNL Google] zoekopdrachten (alleen voor advertenties die op trefwoorden zijn gericht),  `s` voor een zoekpartner (alleen voor advertenties die op trefwoorden zijn gericht) of  `d` voor het weergavenetwerk (voor advertenties die op trefwoorden zijn gericht of die op plaatsing zijn gericht).
* `{keyword}` is of het specifieke sleutelwoord dat uw advertentie (op onderzoeksplaatsen) of het best-passende sleutelwoord (op inhoudsplaatsen) teweegbracht.

AMO ID-indeling voor [!DNL Microsoft Advertising]:

```AL!{ef_userid}!{ef_sid}!{AdId}!{OrderItemId}```

waarbij:

* `{AdId}` Dit is de  [!DNL Microsoft Advertising] unieke numerieke id voor creatieve projecten.
* `{OrderItemId}` is de  [!DNL Microsoft Advertising] numerieke id voor het trefwoord.

### AMO ID Dimension in [!DNL Analytics]

In de rapporten van Analytics, kunt u AMO ID- gegevens vinden door naar de [!UICONTROL AMO ID] dimensie te zoeken en [!UICONTROL AMO ID Instance] metrisch te gebruiken. In de [!UICONTROL AMO ID]-dimensie worden alle vastgelegde AMO-id-waarden opgeslagen, terwijl de [!UICONTROL AMO ID Instance]-meting aangeeft hoe vaak een AMO-id-waarde door de site is vastgelegd. Als bijvoorbeeld vier keer op dezelfde zoekadvertentie is geklikt, maar Analytics zeven sittemarkeringen bijhoudt, zou [!UICONTROL AMO ID Instance] zeven (7) zijn en [!UICONTROL Clicks] vier (4).

Voor elke rapportage of controle binnen [!DNL Analytics] kunt u het beste de AMO-id samen met het overeenkomstige exemplaar gebruiken. Zie &quot;[Gegevensvalidatie voor [!DNL Analytics for Advertising Cloud]](data-variances.md#data-validation)&quot; in &quot;Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud.&quot;

## Informatie over analytische classificaties

In [!DNL Analytics] is een [classificatie](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html) een stuk van meta-gegevens voor een bepaalde het volgen code, zoals Rekening, Campagne, of Advertentie. Advertising Cloud categoriseert onbewerkte Advertising Cloud-gegevens aan de hand van classificaties, zodat u de gegevens op verschillende manieren kunt weergeven (bijvoorbeeld op Advertentietype of Campagne) wanneer u rapporten genereert. Classificaties vormen de basis voor Advertising Cloud-rapportage in [!DNL Analytics] en kunnen worden gebruikt met de AMO-metriek, zoals [!UICONTROL AMO Cost], [!UICONTROL AMO Impressions] en [!UICONTROL AMO Clicks], alsmede met aangepaste en standaard onsite gebeurtenissen zoals [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders] en [!UICONTROL Revenue].

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Gegevensvariaties  [!DNL Analytics] tussen en Advertising Cloud verwacht](data-variances.md)

