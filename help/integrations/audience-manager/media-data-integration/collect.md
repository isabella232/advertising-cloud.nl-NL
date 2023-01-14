---
title: Klik- en indrukgegevens verzamelen uit DSP advertenties
description: Leer hoe u op cookies gebaseerde beelden vastlegt en op gebeurtenissen klikt in advertenties DSP advertenties met Audience Managers pixels
feature: Integration with Adobe Audience Manager
exl-id: eb717148-00ab-428a-97b9-e8396a5c47b0
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---

# Blootstellingsgegevens van media verzamelen van reclame DSP campagnes

*Adverteerders DSP alleen reclame*

*Adverteerders met een Adobe Advertising-Adobe Audience Manager Integration Only*

In dit document wordt uitgelegd hoe u advertenties DSP advertenties kunt voorzien van labels om op cookies gebaseerde beelden vast te leggen en op gebeurtenissen kunt klikken met pixels van Audience Managers en extra taken om de gegevens te kunnen gebruiken.

De gebeurtenispixels leggen geen gebeurtenissen vast die plaatsvinden in omgevingen zonder cookie, zoals mobiele apps en aangesloten tv (CTV).

## Stap 1: Een gegevensbron instellen in Audience Manager {#set-up-data-source}

Maak in de Audience Manager een [gegevensbron](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/datasources-list-and-settings.html) voor de DSP en klik op gegevens. De gegevensbron-id opnemen [in elke gebeurtenistag](#implement-dsp-pixels) zodat alle bijgehouden gebeurtenissen worden toegewezen aan de gegevensbron.

>[!NOTE]
> Het is mogelijk om alle beelden te verzamelen en gegevens voor reclamecampagnes te klikken die op veelvoudige DSP binnen één enkele gegevensbron lopen.

## Stap 2: Impressie implementeren en op webpagina&#39;s op gebeurtenispixels klikken {#implement-dsp-pixels}

Adverteerders kunnen gebeurtenislabels voor hun eigen merken maken en implementeren. Neem indien nodig contact op met uw Adobe Audience Manager-consultant of uw [!DNL Adobe] accountmanager voor ondersteuning.

>[!NOTE]
>
>Als uw organisatie [!DNL Analytics] gevolgd, dan hebt u misschien geen Audience Manager het klikken volgen nodig. Adobe Analytics legt kliksignalen vast en kan ze naar de Audience Manager verzenden [server-kant door:sturen](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

### Pixelsyntaxis

Gebeurtenispixels moeten de volgende parameters bevatten.

**Pixels voor het bijhouden van indrukking:**

`[Audience Manager customer domain].demdex.net/event?d_event=imp&d_src=[source id]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

with [optionele aanvullende parameters](#parameters) voorgefixeerd met `&`

**Klikken-volgende pixels:**

`[Audience Manager customer domain].demdex.net/event?d_event=click&d_src=[source id]&d_rd=[redirect URL]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

with [optionele aanvullende parameters](#parameters) voorgefixeerd met `&`

Waar:

* `[Audience Manager customer domain]` is de domeinnaam waarnaar de indruk wordt gewekt of waarop klikgebeurtenissen worden verzonden [!DNL Adobe].

* `[source id]` is de id voor de [gegevensbron](#set-up-data-source) waarin u DSP indruk zult volgen en gegevens zult klikken.

* `[redirect URL]` is de dubbele gecodeerde omleidings-URL. Als u een online coderingsprogramma gebruikt, zoals www.urlencoder.org, voert u de tekenreeks uit via de codeermodule en codeert u het resultaat opnieuw.

* `${TM_CAMPAIGN_ID_NUM}` is de numerieke campagne-id in DSP. Als u een afzonderlijke campagne-id wilt coderen in plaats van de DSP macro te gebruiken, zoekt u de id in de campagne-instellingen.

* Elk [parameter](#key-value-pairs) is vooraf ingesteld met `&` en heeft de notatie `d_parameter=parameter_id`, waarbij `parameter` wordt vervangen door het sleutelwaardepaar voor het nieuwe veld. Voorbeeld: `&d_placement=${TM_PLACEMENT_ID_NUM}`

### Parameters als sleutelwaardeparen {#parameters}

**Indeling:**  `d_parameter=parameter_id`

    waarbij:
    
    * de parameter wordt voorafgegaan door `&amp;&#39;
    
    * &quot;parameter&quot; wordt vervangen door het sleutelwaardepaar voor het nieuwe veld
    
    Voorbeeld: `&amp;d_placement=${TM_PLACEMENT_ID_NUM}`

Beide typen pixels kunnen aanvullende parameters bevatten als *sleutelwaardeparen* om eigenschappen te verzamelen of campagnemetagegevens (zoals een plaatsingsnaam of een campagnenaam) voor andere rapporten te verstrekken. Een sleutelwaardepaar bestaat uit twee gerelateerde elementen: a *key*, dat een constante is die de gegevensset definieert, en een *value*, een variabele die tot de set behoort.

In het sleutelwaardepaar, kan de waardevariabele of hard - gecodeerde identiteitskaart of zijn *macro* Dit is een kleine eenheid op zichzelf staande code die dynamisch wordt vervangen door de bijbehorende waarden wanneer de tag ad wordt geladen voor het bijhouden van campagnes en gebruikers. Voor campagneparameters kunt u [DSP macro&#39;s](/help/dsp/campaign-management/macros.md) in plaats van Audience Manager macros om campagnerekenmerken samen met de overeenkomstige indruk te verzenden of gegevens aan Audience Manager te klikken, gebruikend één enkele pixel over alle advertenties. De DSP macro&#39;s die u in uw gebeurtenispixels invoegt, moeten de juiste waarden zijn voor de sleutelwaardeparen die u in de pixels opneemt. Bijvoorbeeld voor `d_placement` sleutel, zou u de DSP macro gebruiken `${TM_PLACEMENT_ID_NUM}` als de waarde voor het vastleggen van plaatsings-id&#39;s die zijn gegenereerd door de Adobe-advertentiemacro.

Raadpleeg &quot;[Vastleggen van Campagne-indrukgegevens via pixelaanroepen](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/impression-data-pixels.html#supported-key-value-pairs).&quot;

Voor een lijst met macro&#39;s die Audience Manager ondersteunt voor click-gebeurtenispixels, raadpleegt u &quot;[Het vangen van Campagne klikt Gegevens via de Vraag van het Pixel](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/click-data-pixels.html).&quot;

>[!TIP]
>
>* De beste manier is om de campagne, plaatsing, creatieve (advertentie) en site-id&#39;s op te nemen, zodat u de campagnerekenmerken kunt gebruiken om Audience Manager-eigenschappen te maken.
>* Voor het maken van Audience Optimization-rapporten zijn aanvullende parameters vereist.
>* Vervang de waarden in de sleutelwaardeparen door de relevante [DSP macro&#39;s](/help/dsp/campaign-management/macros.md) zodat u in alle campagnes één pixel kunt gebruiken voor alle advertenties. Bijvoorbeeld, wijzigen `d_campaign=[%campaignID%]`tot `d_campaign=${TM_CAMPAIGN_ID_NUM}` om campagne-id&#39;s vast te leggen die zijn gegenereerd door de Adobe Advertising macro.
>* Indien nodig kunt u uw eigen parameters met gecodeerde waarden maken. Voorbeeld: `d_DSP=AdCloud`


Voorbeeld van een pixel van een impressiegebeurtenis:

`http://acme.demdex.net/event?d_event=imp&d_src=1052880&d_site=${TM_SITE_ID_NUM}&d_creative=${TM_AD_ID_NUM}&d_placement=${TM_FEED_ID_NUM}&d_campaign=${TM_CAMPAIGN_ID_NUM}&d_DSP=AdCloud&d_bust=${TM_RANDOM}`

### Waar moet u de pixels toevoegen?

#### Pixel voor het bijhouden van indrukken

Koppel een pixel voor het bijhouden van een impressie aan alle advertenties in uw [!DNL DSP] campagnes. U kunt dit op de volgende plaatsen doen:

* Op plaatsingsniveau, dat de pixel door gebrek op alle advertenties in de plaatsing toepast. Voeg in het gedeelte Tekstspatiëring van de plaatsingsinstellingen de pixel toe in het gedeelte [[!UICONTROL Event pixels] field](/help/dsp/campaign-management/placements/placement-settings.md).

* Op advertentieniveau, dat om het even welke plaatsing-vlakke gebeurtenispixel met voeten treedt. In de advertentie-instellingen [een gebeurtenispixel maken op het tabblad [!UICONTROL Pixel] tab](/help/dsp/campaign-management/ads/ad-edit.md).

* (Voor advertenties op een externe advertentieserver) Op advertentieniveau in de advertentieserver.

#### Klikken en pixels bijhouden

Voeg in de advertentieserver de pixel van de klikgebeurtenis in (met de gecodeerde URL toegevoegd) waar u normaal de klikdoorklikURL van de advertentie invoegt.

## Stap 3: Taken na de implementatie

Zodra de gebeurtenismarkeringen worden uitgevoerd, zullen de gegevens in de servers van de de gegevensinzameling van de Audience Manager stromen. Voer de volgende taken uit voordat u de gegevens in rapporten kunt gebruiken.

### Een [!DNL Amazon S3] Emmertje en gegevensbron

Als uw gegevens zich op de servers van de Audience Manager bevinden, moet u een [!DNL Amazon Simple Storage Service] ([!DNL Amazon S3]) emmertje en vervolgens een gegevensbron, waarnaar alle pixelgegevens worden verzonden. Neem contact op met uw Audience Manager consultant of [Klantenservice](https://experienceleague.adobe.com/docs/audience-manager/user-guide/help-and-legal/help-legal-contact.html) als u ondersteuning nodig hebt.

### Audience Managers en segmenten maken

Uw gebeurtenisgegevens stromen in Audience Manager als [ongebruikte signalen](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/interactive-and-overlap-reports/unused-signals.html). Handmatig maken [op regels gebaseerde kenmerken](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html) van de opgenomen gegevens, en creeer dan [segmenten](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/segments-purpose.html) gebruik deze kenmerken voordat u de gegevens in rapporten kunt gebruiken.

Voorbeeld dat gegevens op gebruikersniveau vult voor gebruikers die worden blootgesteld aan een bepaalde creatieve functie in DSP:

1. De gebeurtenis identificeren als `d_event = imp`.
1. Identificeer creatieve identiteitskaart binnen de DSP campagne, en wijs het dan aan het bezit toe zoals `d_creative=[Creative ID]`.

![Trait creation screen](/help/dsp/assets/aa-trait.png)

>[!MORELIKETHIS]
>
>* [DSP Macros](/help/dsp/campaign-management/macros.md)
>* [Overzicht van het verzenden van gegevens over DSP mediablootstelling naar Adobe Audience Manager](overview.md)
>* [Gevallen gebruiken](use-cases.md)

