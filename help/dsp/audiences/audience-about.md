---
title: Over het beheer van het publiek in DSP
description: Meer informatie over functies voor publieksbeheer.
feature: DSP Audiences, DSP Segments
exl-id: 624d2211-59a2-4791-b8f1-a9a5cecd0b8e
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 0%

---

# Over het beheer van het publiek in DSP

In DSP kunt u publiekssegmenten en publiekssets maken en beheren, die u kunt gebruiken als doelen voor uw plaatsingen:

* U kunt uw eigen gegevens van het eerste publiek verzamelen door segmenten te creëren en uit te voeren. U kunt gebruikers in het segment later opnieuw toewijzen met advertenties of u kunt voorkomen dat gebruikers in het segment advertenties ontvangen. U kunt de volgende typen segmenten maken:

   * [Aangepaste segmenten](/help/dsp/audiences/custom-segment-create.md) om a) gebruikers bij te houden die zijn blootgesteld aan advertenties van desktop-, mobiele- en CTV-apparaten en b) gebruikers die specifieke webpagina&#39;s bezoeken.

   * [CCPA opt-out of-of-sale segmenten](/help/dsp/audiences/ccpa-opt-out-segment-create.md) om de gebruikers-id&#39;s op uw website te traceren van de door de consument ingediende opt-out-of-sale aanvragen, overeenkomstig de California Consumer Privacy Act (CCPA). U kunt maandelijkse rapporten van de gebruikers-id&#39;s ophalen uit aanvragen om niet te verkopen.

      Voor meer informatie over Adobe Advertising support for CCPA opt-out of-of-sales request, raadpleegt u [Adobe Advertising Support for the California Consumer Privacy Act: Support voor consumenten](/help/privacy/ad-cloud-ccpa-opt-out-of-sale.md).

* U kunt een publieksbibliotheek maken van [herbruikbaar publiek](/help/dsp/audiences/reusable-audience-create.md). Opgeslagen doelgroepen bestaan uit een van uw beschikbare doelsegmenten en een van uw andere opgeslagen doelgroepen. Wijzigingen die u aanbrengt in een opgeslagen publiek, worden automatisch toegepast op alle plaatsen die het publiek als doel hebben of uitsluiten en op alle andere soorten publiek die het opgeslagen publiek bevatten.

   Opgeslagen publiek stelt mediaplanners in staat om het publiek zo nodig te groeperen door meerdere segmenten met behulp van complexe Booleaanse logica in te sluiten en uit te sluiten. De grootte van elk individueel segment en de totale publieksgrootte worden vermeld aangezien u een publiek bouwt. De managers van de campagne kunnen één of meerdere bewaarde publiek dan eenvoudig selecteren als plaatsingsdoelstellingen eerder dan manueel publieksdoelstellingen voor elke plaatsing vormen.

Er zijn ook extra publiekstypen beschikbaar voor plaatsing als doel.

## Eerste partij en gegevenssegmenten van derden importeren

DSP kunnen uw eigen gegevenssegmenten van de eerste partij van uw gegevensbeheerplatform (DMP) invoeren en hen verstrekken aan om het even welke reeks adverteerders, zoals nodig.

DSP is een geïntegreerde bestemming voor [de [!DNL Adobe Real-Time Customer Data Profile (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html), zodat u geverifieerde first-party-segmenten kunt delen met goedgekeurde adverteerders en gebruikers voor activering van de campagne. Voor meer informatie over de integratie van Real-Time CDP raadpleegt u de [Bronsectie](/help/dsp/audiences/sources/source-about.md).

DSP kunnen ook aangepaste segmenten van derden importeren, waaronder complexe combinaties van segmenten van derden. U kunt de segmenten desgewenst aan elke set adverteerders aanbieden.

Neem contact op met uw [!DNL Adobe] accountteam voor meer informatie.

## publiek beschikbaar als plaatsingsdoelen

U kunt uw plaatsingen aan alle volgende soorten publiek richten.

* Alle door de gebruiker gemaakte publiekssets die in DSP zijn opgeslagen.

* Alle door de gebruiker gemaakte publiekssegmenten die in DSP zijn gemaakt:

   * Aangepaste segmenten voor gebruikers die specifieke webpagina&#39;s hebben bezocht en gebruikers die zijn blootgesteld aan indrukken van specifieke advertenties.

   * CCPA opt-out-of-sale publiekssegmenten voor gebruikers die opt-out-of-sale verzoeken op uw website, volgens de California Consumer Privacy Act (CCPA) hebben ingediend.

* Alle geïmporteerde gegevenssegmenten van de eerste partij.

* Alle geïmporteerde gegevenssegmenten van derden.

* (Plaatsen die zich richten op de V.S. slechts) [Alle gegevenssegmenten van derden die beschikbaar zijn voor DSP klanten van meer dan 30 providers](/help/dsp/audiences/third-party-data-providers.md), met inbegrip van [!DNL Acxiom], [!DNL Datalogix], [!DNL eXelate] ([!DNL Nielsen]), [!DNL Lotame], [!DNL Oracle], [!DNL Quantcast]en nog veel meer.

   U kunt zich richten op specifieke segmenten, die gebruikers richten die op publieksgegevens (bijvoorbeeld, gebruikers met specifieke demografie, belangen of intents, en/of gedragsprofielen) worden gebaseerd. U kunt bladeren door gegevensleverancier en categorie, naar segmenten door naam of segmentidentiteitskaart zoeken, of de resultaten door gegevensleverancier, totale segmentgrootte, Webbrowser telling, of apparatentelling filtreren.

   Voor segmenten van derden worden extra kosten aangerekend, die naast elke segmentnaam worden vermeld.

* (Adverteerders met Adobe Experience Platform en [!DNL Real-Time CDP], Adobe Audience Manager of Adobe Analytics die alleen conversietags voor advertenties in JavaScript gebruiken) Al uw beschikbare doelsegmenten van het eerste, tweede of derde type die zijn gemaakt in [!DNL Real-Time CDP], gemaakt in Audience Manager of gepubliceerd naar Adobe Experience Cloud vanuit Audience Manager of [!DNL Analytics].

   Prijzen voor het gebruik van de segmenten worden vooraf onderhandeld en zijn niet zichtbaar in DSP.

   Segmenten van [!DNL Analytics] zijn ongeveer een uur beschikbaar nadat u deze als Experience Cloud-publiek hebt gemaakt of gepubliceerd. Segmenten die rechtstreeks afkomstig zijn van Audience Manager of [!DNL Real-Time CDP] zijn beschikbaar binnen 24 uur nadat u deze deelt.

   >[!NOTE]
   >
   >Zie de documentatie voor [Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-home.html), [Analyse](https://experienceleague.adobe.com/docs/analytics.html), en [de [!DNL Real-Time CDP]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/segmentation/segment-builder-guide.html) voor informatie over vestiging en het verzamelen van gegevens voor segmenten in die oplossingen.

## Gegevens over doelgrootte

Binnen de opgeslagen publieksinstellingen en plaatsingsinstellingen kunt u gedetailleerde gegevens over de publieksgrootte zien:

* De totale en actieve gededupliceerde publieksgrootte voor alle geselecteerde segmenten en opgeslagen doelgroepen wordt weergegeven en u kunt details per apparaattype (browser, mobiel of aangesloten tv) weergeven.

   ![de gecombineerde publieksgrootte](/help/dsp/assets/audience-size.png)

* Voor individuele segmenten en bewaard publiek, worden de totale publieksgrootte en CPM (indien van toepassing) getoond naast de segmentnaam. U kunt meer details over het segment weergeven, zoals de grootte per apparaattype (browser, mobiel of aangesloten tv). Voor opgeslagen publiek is de totale grootte het gedupliceerde totaal.

   ![de individuele segmentgrootte](/help/dsp/assets/audience-size-segment.png)

## De weergave Soorten publiek

### De weergave Alle soorten publiek

In de [!UICONTROL All Audiences] In de Audience Library kunt u herbruikbare soorten publiek opslaan en beheren, waaronder groepen publiekssegmenten en zelfs andere opgeslagen soorten publiek. U kunt doelgroepen gebruiken als doelen voor meerdere plaatsen. Het aantal plaatsen waarin elk publiek wordt gebruikt wordt vermeld naast de plaatsingsnaam.

U kunt een publiek bewerken, klonen, verwijderen, exporteren of delen.

### De weergave Segmenten

In de [!UICONTROL Segments] alle gebruikers kunnen extra aangepaste segmenten maken.

De [!UICONTROL Segments] in de weergave worden ook de volgende segmenttypen weergegeven:

* Alle door de gebruiker gemaakte aangepaste segmenten zijn beschikbaar voor de gebruiker.

   U kunt de volgende markeringen voor om het even welke douanesegmenten bekijken u creeerde, en die segmenten met andere gebruikers delen. U kunt ook de aangepaste segmenten die u hebt gemaakt bewerken of verwijderen.

   U kunt geen aangepaste segmenten bewerken of delen die andere gebruikers met u hebben gedeeld.

* Alle geïmporteerde eerste-partijsegmenten zijn beschikbaar voor de gebruiker.

   U kunt geen eerste-partijsegmenten uitgeven of delen die met u werden gedeeld. Neem contact op met uw [!DNL Adobe] -accountteam als u eersteklas segmenten met extra gebruikers moet delen.

* Alle aangepaste segmenten van derden zijn beschikbaar voor de gebruiker.

   U kunt segmenten van derden die met u zijn gedeeld, niet bewerken of delen. Neem contact op met uw [!DNL Adobe] accountteam als u segmenten van derden met extra gebruikers wilt delen.

>[!MORELIKETHIS]
>
>* [Een herbruikbaar publiek maken](reusable-audience-create.md)
>* [Instellingen publiek](audience-settings.md)
>* [Syntaxis voor Audience Segment Logic](audience-segment-logic-syntax.md)
>* [Een aangepast segment maken en implementeren](custom-segment-create.md)
>* [Een [!UICONTROL CCPA Opt-Out-of-Sale] Segment](ccpa-opt-out-segment-create.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

