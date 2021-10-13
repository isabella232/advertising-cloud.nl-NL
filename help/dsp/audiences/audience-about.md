---
title: Over Audience Management in Advertising Cloud DSP
description: Meer informatie over functies voor publieksbeheer.
feature: DSP Audiences, DSP Segments
exl-id: 624d2211-59a2-4791-b8f1-a9a5cecd0b8e
source-git-commit: 578651a458ffd505573df0e9a61e26bd2176ad17
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Over Audience Management in Advertising Cloud DSP

In Advertising Cloud DSP kunt u publiekssegmenten en publiekssets maken en beheren, die u kunt gebruiken als doelen voor uw plaatsingen:

* U kunt uw eigen gegevens van het eerste publiek verzamelen door segmenten te creëren en uit te voeren. U kunt gebruikers in het segment later opnieuw toewijzen met advertenties of u kunt voorkomen dat gebruikers in het segment advertenties ontvangen. U kunt de volgende typen segmenten maken:

   * [Aangepaste ](/help/dsp/audiences/custom-segment-create.md) segmenten om a) gebruikers bij te houden die worden blootgesteld aan advertenties van desktop-, mobiele- en CTV-apparaten en b) gebruikers die specifieke webpagina&#39;s bezoeken.

   * [CCPA-opt-out-of-sales-](/help/dsp/audiences/ccpa-opt-out-segment-create.md) segmentering om de gebruikers-id&#39;s te volgen van de consument-opt-out-of-sales-verzoeken op uw website, volgens de California Consumer Privacy Act (CCPA). U kunt maandelijkse rapporten van de gebruikers-id&#39;s ophalen uit aanvragen om niet te verkopen.

      Voor meer informatie over de steun van Advertising Cloud voor de opt-out van CCPA verzoeken, zie [Steun van Adobe Advertising Cloud voor de Wet van de Privacy van de consument van Californië: Support voor de optie-out voor consumenten](https://experienceleague.adobe.com/docs/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html).

* U kunt een publieksbibliotheek van [herbruikbaar publiek](/help/dsp/audiences/reusable-audience-create.md) tot stand brengen. Opgeslagen doelgroepen bestaan uit een van uw beschikbare doelsegmenten en een van uw andere opgeslagen doelgroepen. Wijzigingen die u aanbrengt in een opgeslagen publiek, worden automatisch toegepast op alle plaatsen die het publiek als doel hebben of uitsluiten en op alle andere soorten publiek die het opgeslagen publiek bevatten.

   Opgeslagen publiek stelt mediaplanners in staat om het publiek zo nodig te groeperen door meerdere segmenten met behulp van complexe Booleaanse logica in te sluiten en uit te sluiten. De grootte van elk individueel segment en de totale publieksgrootte worden vermeld aangezien u een publiek bouwt. De managers van de campagne kunnen één of meerdere bewaarde publiek dan eenvoudig selecteren als plaatsingsdoelstellingen eerder dan manueel publieksdoelstellingen voor elke plaatsing vormen.

Er zijn ook extra publiekstypen beschikbaar voor plaatsing als doel.

## Eerste partij en gegevenssegmenten van derden importeren

Advertising Cloud DSP kan uw eigen gegevenssegmenten van de eerste partij van uw gegevensbeheerplatform (DMP) invoeren en hen verstrekken aan om het even welke reeks adverteerders, zoals nodig.

Advertising Cloud DSP kan ook aangepaste segmenten van derden importeren, waaronder complexe combinaties van segmenten van derden. U kunt de segmenten desgewenst aan elke set adverteerders aanbieden.

Neem contact op met uw accountmanager voor meer informatie.

## publiek beschikbaar als plaatsingsdoelen

U kunt uw plaatsingen aan alle volgende soorten publiek richten.

* Alle door de gebruiker gemaakte publiekssets die in Advertising Cloud DSP zijn opgeslagen.

* Alle door de gebruiker gemaakte publiekssegmenten die in Advertising Cloud DSP zijn gemaakt:

   * Aangepaste segmenten voor gebruikers die specifieke webpagina&#39;s hebben bezocht en gebruikers die zijn blootgesteld aan indrukken van specifieke advertenties.

   * CCPA opt-out-of-sale publiekssegmenten voor gebruikers die opt-out-of-sale verzoeken op uw website, volgens de California Consumer Privacy Act (CCPA) hebben ingediend.

* Alle geïmporteerde gegevenssegmenten van de eerste partij.

* Alle geïmporteerde gegevenssegmenten van derden.

* (Plaatsen die alleen op de VS gericht zijn) [Alle gegevenssegmenten van derden die beschikbaar zijn voor Advertising Cloud DSP-klanten van meer dan 30 providers](/help/dsp/audiences/third-party-data-providers.md), inclusief [!DNL Acxiom], [!DNL Datalogix], [!DNL eXelate] ([!DNL Nielsen]), [!DNL Lotame], [!DNL Oracle], [!DNL Quantcast] en nog veel meer.

   U kunt zich richten op specifieke segmenten, die gebruikers richten die op publieksgegevens (bijvoorbeeld, gebruikers met specifieke demografie, belangen of intents, en/of gedragsprofielen) worden gebaseerd. U kunt bladeren door gegevensleverancier en categorie, naar segmenten door naam of segmentidentiteitskaart zoeken, of de resultaten door gegevensleverancier, totale segmentgrootte, Webbrowser telling, of apparatentelling filtreren.

   Voor segmenten van derden worden extra kosten aangerekend, die naast elke segmentnaam worden vermeld.

* (Adverteerders met Adobe Experience Cloud, Adobe Audience Manager of Adobe Analytics die alleen Advertising Cloud JavaScript-conversietags gebruiken) Al uw beschikbare eerste-, tweede- of andere publiekssegmenten die in Adobe Experience Cloud zijn gemaakt, in Audience Manager zijn gemaakt of vanuit Audience Manager of [!DNL Analytics] naar Adobe Experience Cloud zijn gepubliceerd.

   Prijzen voor het gebruik van de segmenten worden vooraf bepaald en zijn niet zichtbaar in Advertising Cloud.  <!-- Verify -->

   Segmenten uit Adobe Experience Cloud zijn ongeveer een uur beschikbaar nadat u deze hebt gemaakt of gepubliceerd in Adobe Experience Cloud. Segmenten die rechtstreeks afkomstig zijn uit de Audience Manager zijn ongeveer 24 uur beschikbaar nadat u ze hebt gemaakt. <!-- Verify all -->

   >[!NOTE]
   >
   >Zie de documentatie voor [Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-home.html), [Analytics](https://experienceleague.adobe.com/docs/analytics.html), en [Adobe Experience Cloud](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html) voor informatie over vestiging en het verzamelen van gegevens voor segmenten in die oplossingen.

## Gegevens over doelgrootte

Binnen de opgeslagen publieksinstellingen en plaatsingsinstellingen kunt u gedetailleerde gegevens over de publieksgrootte zien:

* De totale en actieve gededupliceerde publieksgrootte voor alle geselecteerde segmenten en opgeslagen doelgroepen wordt weergegeven en u kunt details per apparaattype (browser, mobiel of aangesloten tv) weergeven.

   ![de gecombineerde publieksgrootte](/help/dsp/assets/audience-size.png)

* Voor individuele segmenten en bewaard publiek, worden de totale publieksgrootte en CPM (indien van toepassing) getoond naast de segmentnaam. U kunt meer details over het segment weergeven, zoals de grootte per apparaattype (browser, mobiel of aangesloten tv). Voor opgeslagen publiek is de totale grootte het gedupliceerde totaal.

   ![de individuele segmentgrootte](/help/dsp/assets/audience-size-segment.png)

## De weergave Soorten publiek

### De weergave Alle soorten publiek

In de [!UICONTROL All Audiences] mening, of de Bibliotheek van het Publiek, kunt u herbruikbare publiek opslaan en beheren, die groepen publiekssegmenten en zelfs andere bewaarde publiek omvatten. U kunt doelgroepen gebruiken als doelen voor meerdere plaatsen. Het aantal plaatsen waarin elk publiek wordt gebruikt wordt vermeld naast de plaatsingsnaam.

U kunt een publiek bewerken, klonen, verwijderen, exporteren of delen.

### De weergave Segmenten

In de weergave [!UICONTROL Segments] kunnen alle gebruikers extra aangepaste segmenten maken.

In de weergave [!UICONTROL Segments] worden ook de volgende segmenttypen weergegeven:

* Alle door de gebruiker gemaakte aangepaste segmenten zijn beschikbaar voor de gebruiker.

   U kunt de volgende markeringen voor om het even welke douanesegmenten bekijken u creeerde, en die segmenten met andere gebruikers delen. U kunt ook de aangepaste segmenten die u hebt gemaakt bewerken of verwijderen.

   U kunt geen aangepaste segmenten bewerken of delen die andere gebruikers met u hebben gedeeld.

* Alle geïmporteerde eerste-partijsegmenten zijn beschikbaar voor de gebruiker.

   U kunt geen eerste-partijsegmenten uitgeven of delen die met u werden gedeeld. Neem contact op met uw accountmanager als u segmenten van de eerste partij met extra gebruikers wilt delen.

* Alle aangepaste segmenten van derden zijn beschikbaar voor de gebruiker.

   U kunt segmenten van derden die met u zijn gedeeld, niet bewerken of delen. Neem contact op met uw accountmanager als u segmenten van derden met extra gebruikers wilt delen.

>[!MORELIKETHIS]
>
>* [Een herbruikbaar publiek maken](reusable-audience-create.md)
>* [Instellingen publiek](audience-settings.md)
>* [Syntaxis voor Audience Segment Logic](audience-segment-logic-syntax.md)
>* [Een aangepast segment maken en implementeren](custom-segment-create.md)
>* [Een  [!UICONTROL CCPA Opt-Out-of-Sale] segment maken en implementeren](ccpa-opt-out-segment-create.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)

