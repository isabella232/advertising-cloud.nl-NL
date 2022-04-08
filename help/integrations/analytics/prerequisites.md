---
title: Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]
description: Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 08e54e2b-ed9b-4489-8de5-ab1379b7133c
source-git-commit: 11a13816ccd2ef0c47efa615c54c0f7ce2f83734
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Vereisten en belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]

*Adverteerders met Advertising Cloud DSP en Advertising Cloud Search*

Bekijk de volgende informatie voordat u Advertising Cloud integreert met Adobe Analytics.

## Vereisten voor het rapporteren van Advertising Cloud-gegevens in [!DNL Analytics]

* een van de volgende twee handelingen:
   * Adobe Experience Platform Web SDK: `alloy.js`
   * Experience Cloud-identiteitsdienst: `visitorAPI.js` versie 2.0 of hoger
* Elke versie van Adobe Analytics (inclusief [!DNL Prime], [!DNL Premium], of [!DNL Ultimate])
* Adobe Analytics: `appMeasurement.js` versie 2.1 of hoger

>[!TIP]
>
>Als u de gegevenskwaliteit wilt verbeteren, gebruikt u de meest recente versie van elke bibliotheek.

## Vereisten voor het delen van analysesegmenten met Advertising Cloud

* Experience Cloud-identiteitsdienst: `visitorAPI.js` versie 2.1 of hoger
* Adobe Analytics: `!DNL appMeasurement.js` versie 1.8 of hoger

## Voorschriften voor rapportage [!DNL Analytics] Gegevens in Advertising Cloud

Geef het Advertising Cloud-implementatieteam de volgende informatie:

* De [!DNL Analytics] rapportsuite-id die wordt gebruikt voor rapportage over betaalde mediaconcentraties en voor het doorvoeren van siteactiviteiten voor optimalisatie en rapportage in Advertising Cloud
* De Experience Cloud Organisatie-id van het bedrijf (Org ID).

U kunt beide id&#39;s vinden op het tabblad [Tabblad Overzicht van de Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html).

![Experience Cloud Debugger Samenvattingsscherm](/help/integrations/assets/a4adc-debugger-summary.png)

## [!DNL Analytics] Gegevens in Advertising Cloud {#lookback-a4adc}

Omdat [!DNL Analytics] gegevens voor rapportage en optimalisatie naar Advertising Cloud worden verzonden, zijn de gegevens onderworpen aan de toewijzingsregels, waaronder de indruk en klik op terugzoekvensters, die voor de adverteerder in Advertising Cloud zijn geconfigureerd.

![Instellingen voor terugzoekvensters op adverteerderniveau in Advertising Cloud](/help/integrations/assets/a4adc-lookbacks.png)

* Advertising Cloud-toewijzing klikt op terugzoekvenster: Het aantal dagen na de eerste klik waarin de klik aan een omzetting kan worden toegeschreven. Deze waarde is standaard 60 dagen; het maximum is 90 dagen
* Terugkijkvenster van Advertising Cloud-attribuutindruk: Het aantal dagen na een advertentie waarin de indruk aan een conversie kan worden toegeschreven. Deze waarde is standaard 14 dagen; het maximum is 30 dagen

   >[!NOTE]
   >
   > Het venster voor het terugzoeken van de indruk is specifiek voor Advertising Cloud, niet [!DNL Analytics for Advertising Cloud], rapportage.

De [!DNL Analytics for Advertising Cloud] JavaScript gebruikt deze instellingen om te bepalen hoe ver u een doorkijkitem of doorklikitem naar de site als geldig kunt beschouwen. Voor meer informatie over hoe mening-door en klik-door wordt bepaald, zie &quot;[Advertising Cloud-id&#39;s gebruikt door Analytics](ids.md).&quot;

## Advertising Cloud-gegevens in [!DNL Analytics]

[!DNL Analytics] Hiermee stelt u Advertising Cloud-id&#39;s (AMO-id&#39;s) in in de hit Analytics, afhankelijk van de persistentie-instelling van de eVar van de adverteerder. Deze instelling geldt voor zowel doorklikken als doorzoeken. De persistentie-instelling wordt geconfigureerd op de achterkant van de Advertising Cloud en uw [!DNL Adobe] accountteam kan dit wijzigen.

* [!DNL Analytics for Advertising Cloud] Vervaldatum eVar: Standaard 60 dagen voor AMO-id&#39;s

>[!NOTE]
>
>Als u gegevens voor een ander tijdframe wilt segmenteren, kunt u [aangepaste segmenten instellen](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html) met verschillende terugzoekvensters in Analysis Workspace.

## Ondersteunde advertentie-omgevingen

* Zoeken
* Weergave
* Video
* Online video
* Oorspronkelijk

Neem contact op met uw [!DNL Adobe] -accountteam voor de nieuwste ondersteunde advertentiemogelijkheden in elk kanaal.

## Wat u moet weten voordat u gaat implementeren

* Het Advertising Cloud-implementatieteam zal de integratie opzetten.

* Voor deze integratie worden geen extra kosten in rekening gebracht en serveraanroepen resulteren niet in extra [!DNL Analytics] of Advertising Cloud-kosten.

* [!DNL Analytics for Advertising Cloud] is een advertentie voor serveragnost: kan een mening-door of klik-door van om het even welke advertentieserver voorkomen, en juiste IDs wordt geproduceerd bij plaatsingang.

* De integratie gaat alleen over [!DNL Analytics] standaard- en aangepaste evenementen voor Advertising Cloud voor het optimaliseren van biedingen voor daaropvolgende betaalde media- en reclameactiviteiten. Het gaat niet door [!DNL Analytics] segmenten, berekende maatstaven en Vars naar Advertising Cloud voor Bodoptimalisatie.

* Advertising Cloud maakt permanente id&#39;s binnen [!DNL Analytics] op basis van de laatste advertentie die is aangeklikt of bekeken voordat de gebruiker de site betreedt, op basis van de [klik en mening-door raadplegingsvensters](#lookback-a4adc) geconfigureerd in Advertising Cloud. Als een bezoeker van de site beide typen interactie voor site-invoer binnen zijn profiel zou hebben en de klik zich binnen de terugzoekperiode bevindt, zou de doorklikeid van de bezoeker de doorkijkID voor site-rapportage overschrijven.

* [!DNL Analytics for Advertising Cloud] Voor het bijhouden van conversies in Adobe Analytics wordt een configureerbaar terugzoekvenster (standaard 60 dagen) gebruikt. Advertising Cloud-rapporten weerspiegelen de omzettingen van sites en de betrokkenheid aan het einde van dit terugzoekvenster.

* Alle advertentietypen worden ondersteund. Niet alle advertentieomgevingen worden echter ondersteund.

   Zo worden aangesloten tv-advertenties (CTV-advertenties) niet bijgehouden omdat er geen kliks plaatsvinden in CTV en er geen conversies kunnen plaatsvinden op hetzelfde apparaat. Als de advertentie echter wordt weergegeven in een desktopomgeving, kunnen bepaalde gegevens van de doorkijksite worden bijgehouden.

* [!DNL Analytics] conversies worden momenteel bijgehouden en alleen toegewezen aan een bezoeker op hetzelfde apparaat.

* [!DNL Analytics for Advertising Cloud] ondersteunt geen in-app weergave-through conversies.

* Het volgen van mening-door wordt niet gesteund voor adverteerders die een server-zij door:sturen implementatie van [!DNL Analytics].

### Aanvullende id

Zodra de Dienst van de Identiteit van de Experience Cloud voor een plaats wordt uitgevoerd, klappen die gegevens van bevatten [!DNL Analytics] of Advertising Cloud bevat een aanvullende id.

Voorbeeld: `sdid=2F3C18E511F618CC-45F83E994AEE93A0`

Voor een nauwkeurige gegevensintegratie worden alle Advertising Cloud-aanroepen gebruikt door een [!DNL Analytics for Advertising Cloud] activiteit om inhoud te leveren of het doel te registreren metrisch moet overeenkomstige hebben [!DNL Analytics] hit die dezelfde aanvullende id deelt.

Wanneer u het oplossen van problemen in bent [!DNL Analytics]moet u bevestigen dat de aanvullende id aanwezig is voor [!DNL Analytics] treffers. In de [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html)kunt u deze id op het tabblad Advertising Cloud zien als de `sdid` parameter.

>[!NOTE]
>
> Deze implementatie werkt op dezelfde manier als de [!DNL Analytics for Target] integratie.

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [JavaScript-code voor analyse voor Advertising Cloud](/help/integrations/analytics/javascript.md)

