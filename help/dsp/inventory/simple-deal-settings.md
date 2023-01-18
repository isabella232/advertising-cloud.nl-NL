---
title: '[!UICONTROL Simple Ad Serving] Deal Settings'
description: Meer informatie over de beschikbare instellingen voor [!UICONTROL Simple Ad Serving] deals.
feature: DSP Simple Ad Serving
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# [!UICONTROL Simple Ad Serving] Dealinstellingen

## Nieuw [!UICONTROL Simple Ad Serving] Overeenkomsten

### [!UICONTROL Select Ad Source]

| Parameter | Beschrijving |
|-----------|-------------|
| **[!UICONTROL Serving Type]** | Het mediatype voor deze deal: *[!UICONTROL Video],* *[!UICONTROL Display],* of *[!UICONTROL Audio].* |
| **[!UICONTROL Publisher Site Served On]** | De naam van de uitgever die deze voorraad verkoopt. Zoek naar een uitgever door minstens de eerste twee karakters in de naam in te gaan. Als u een uitgever wilt toevoegen die niet in de lijst staat, neemt u contact op met uw [!DNL Adobe] accountteam. |
| **[!UICONTROL Advertiser]** | Één enkele adverteerder in de rekening die tot deze overeenkomst kan toegang hebben. Selecteer ook de campagne en (naar keuze) het pakket waarin de overeenkomst beschikbaar is. |
| **[!UICONTROL Media Quality Assessment?]** | (Sommige gebruikers) Laat de advertentie toe om op een andere DSP voor derdecontrole te lopen. <!-- Who can select this? It's disabled for me. Need to see if there are additional fields when this is enabled. --> |
| **[!UICONTROL Ad Source]** | De enige optie is *[!UICONTROL Site Serve (Event Pixels)]*. |
| **[!UICONTROL Ad Creation]** | (Alleen nieuwe deals) Of:<ul><li>*[!UICONTROL Create New]:* Om een advertentie voor deze overeenkomst tot stand te brengen.</li><li>*[!UICONTROL Select Ads]:* Om een bestaande advertentie voor deze overeenkomst te gebruiken.</li></ul> |
| **[!UICONTROL Ad Type]** | Het advertentietype voor deze overeenkomst. Als u advertenties voor de overeenkomst gaat creëren, omvat de advertentiegrootte of de duur, zoals gevraagd. De beschikbare opties variëren per mediatype. |

{style=&quot;table-layout:auto&quot;}

### [!UICONTROL Select Ad(s)]

(Wanneer u bestaande advertenties gebruikt) De advertenties om in de overeenkomst te omvatten. Schakel het selectievakje naast elke advertentie in die u wilt opnemen.

### [!UICONTROL Select & Upload [Media Type]]

(Alleen nieuwe advertenties) Schermen om een nieuwe [advertenties van derden](/help/dsp/campaign-management/ads/ad-create-multiple.md).

### [!UICONTROL Feed Details]

| Parameter | Beschrijving |
|-----------|-------------|
| **[!UICONTROL Media CPM]** | De kosten per 1000 beelden (CPM), zoals die in de tariefkaart voor uw contract worden weerspiegeld. Neem contact op met uw [!DNL Adobe] accountteam voor deze waarde. <br><br>Specificeer ook de munt voor de overeenkomst. Alle gebruikers kunnen USD selecteren, of, als het SSP extra valuta&#39;s steunt, de munt voor de DSP rekening. |
| **[!UICONTROL Third Party Billed Fees]** | (Optioneel) Een statische vergoeding voor derden die moet worden bijgehouden als niet-factureerbare kostprijs, en de valuta voor de transactie.<br><br>Alle gebruikers kunnen USD selecteren, of, als het SSP extra valuta&#39;s steunt, de munt voor de DSP rekening. **OPMERKING:** Facultatieve vergoedingen worden weerspiegeld in de [!UICONTROL Net CPM] metrisch. |
| **[!UICONTROL Third Party Fee Description]** | (Optioneel) Een beschrijving van de vergoedingen van derden. |
| **[!UICONTROL Flight Dates]** | De begin en einddata voor verkeer die deze overeenkomst gebruiken. De vluchtdata moeten worden opgenomen in de vluchtdata voor de campagne. De advertentietags retourneren alleen een reactie tijdens de opgegeven vlucht.<br><br> De beste praktijken om een afzonderlijke eenvoudige ad dienende campagne met een jaar-lange duur te creëren en het volgen pixel binnen het te bouwen. |
| **[!UICONTROL Impressions]** | (Facultatief) het geschatte aantal indrukkingen u verwacht om te lopen gebruikend deze overeenkomst. Deze waarde wordt alleen gebruikt voor traceringsdoeleinden en om te markeren wanneer de leveringsdoelen zijn bereikt; de uitgever controleert de daadwerkelijke levering en levering. De beste manier is om een groot aantal afbeeldingen in te voeren om de tag actief te houden binnen DSP, zodat deze indien nodig kan worden vernieuwd of uitgebreid. |
| **[!UICONTROL Deal Name]** | De naam van de deal. Voer een naam in of selecteer *[!UICONTROL Auto Generate Deal Name]* om DSP een naam te laten produceren die op de overeenkomstendetails wordt gebaseerd.<br><br>Voorbeeld van een automatisch gegenereerde naam: `Campaign-desktop_video_preroll_15-24Kitchen-$10_USD-jdoe-SAS` |
| **[!UICONTROL Attached Ads]** | (Alleen-lezen) De advertenties die deel uitmaken van de deal. Als u een advertentie wilt bewerken, klikt u op de naam van de advertentie. Om een advertentie uit de overeenkomst te verwijderen, klik **[!UICONTROL X]** naast de naam van de advertentie. |

{style=&quot;table-layout:auto&quot;}

<!-- 
## Existing Simple Ad Serving Deals

Changes aren't applied retroactively.
-->

<!-- completely different settings layout, so need a separate section for them -->

<!-- From Abhinav: Editable fields are Name, Start & End date, Impressions & CPM. Changes are not applied retroactively.

But I see:

| Parameter | Description |
|-----------|-------------|

| **[!UICONTROL Are you using Deal ID?] | (Read-only) Whether the deal was set up as a [!UICONTROL Deal ID] (*[!DNL Yes]*)  or a [!UICONTROL Simple Ad Serving] deal (*[!DNL No]*). |
| **[!UICONTROL Inventory Type] | (Read-only) The inventory type for the deal. |
| **[!UICONTROL Feed Name] | The name of the [!UICONTROL Simple Ad Serving] deal. |
| **[!UICONTROL Publisher Ad Server] | (Read-only)  |
| **[!UICONTROL Publisher maximum ad length] | The maximum length of the ad, per the publisher. |
| **[!UICONTROL Publisher minimum ad length] | The minimum length of the ad, per the publisher. |
| **[!UICONTROL Fill Type] | (Read-only)  |
| **[!UICONTROL Contracted CPM] | This field is required if billing through TubeMogul, but enter your CPM in this field to track your actual spend. |
| **[!UICONTROL 3rd party technology CPM] | (Optional)  |
| **[!UICONTROL Planned Flight Dates] | The beginning and end dates for the deal flight. These dates don't control ad delivery but are used to track delivery pacing. **THIS IS CONTRARY TO WHAT THE NEW DEAL SETTINGS ABOVE, FROM ABHINAV, SAY**> |
| **[!UICONTROL Target Impressions] | (Optional) The estimated number of impressions you expect to run using this deal. This value is used for tracking purposes only and to flag when delivery goals are met; the publisher controls actual ad delivery. The best practice is to enter a high number of impressions to keep the tag active within DSP so it can be renewed or extended if needed. |
 -->

>[!MORELIKETHIS]
>
>* [Info [!UICONTROL Simple Ad Serving]](simple-deal-about.md)
>* [Een [!UICONTROL Simple Ad Serving] Deal](simple-deal-create.md)
>* [Bewerken [!UICONTROL Simple Ad Serving] Dealinstellingen](simple-deal-edit.md)
>* [Bekijk een Gedetailleerd Rapport voor een Overeenkomst](/help/dsp/inventory/deal-view-report.md)


<!-- add back when reimplemented:
>* [View Event-Tracking Pixels for a [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)
-->
