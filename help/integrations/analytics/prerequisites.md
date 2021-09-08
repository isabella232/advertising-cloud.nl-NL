---
title: Vereisten en Belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]
description: Vereisten en Belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 08e54e2b-ed9b-4489-8de5-ab1379b7133c
source-git-commit: e2ee41c7e3e195f062ad1cc67080ed913d6d3d06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Vereisten en Belangrijke Informatie voor het Uitvoeren [!DNL Analytics for Advertising Cloud]

*Adverteerders met Advertising Cloud DSP en Advertising Cloud Search*

Bekijk de volgende informatie voordat u Advertising Cloud integreert met Adobe Analytics.

## Vereisten voor het rapporteren van Advertising Cloud-gegevens in [!DNL Analytics]

* Experience Cloud-identiteitsdienst: `visitorAPI.js` versie 2.0 of hoger
* Elke versie van Adobe Analytics (inclusief [!DNL Prime], [!DNL Premium] of [!DNL Ultimate])
* Adobe Analytics: `appMeasurement.js` versie 2.1 of hoger

>[!TIP]
>
>Voor een betere gegevenskwaliteit gebruikt u de meest recente versie van de Experience Cloud Identity Service met ondersteuning voor CNAME en de meest recente versie van Analytics AppMeasurement voor JavaScript.

## Vereisten voor het delen van analysesegmenten met Advertising Cloud

* Experience Cloud-identiteitsdienst: `visitorAPI.js` versie 2.1 of hoger
* Adobe Analytics: `!DNL appMeasurement.js` versie 1.8 of hoger

## Vereisten voor rapportage [!DNL Analytics] gegevens in Advertising Cloud

Geef het Advertising Cloud-implementatieteam de volgende informatie:

* De [!DNL Analytics]-rapportsuite-id die wordt gebruikt voor rapportage over betaalde mediaconcentraties en voor het doorvoeren van siteactiviteiten voor optimalisatie en rapportage in Advertising Cloud
* De Experience Cloud Organisatie-id van het bedrijf (Org ID).

U kunt beide id&#39;s vinden op het scherm [Samenvatting van de Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/run-debugger.html).

![Experience Cloud Debugger Samenvattingsscherm](/help/integrations/assets/a4adc-debugger-summary.png)

## [!DNL Analytics] Gegevens in Advertising Cloud {#lookback-a4adc}

Aangezien [!DNL Analytics] gegevens naar Advertising Cloud worden verzonden voor rapportage en optimalisatie, zijn de gegevens onderworpen aan de toewijzingsregels, inclusief de indruk en klik op terugzoekvensters, die zijn geconfigureerd voor de adverteerder in Advertising Cloud.

![Instellingen voor terugzoekvensters op adverteerderniveau in Advertising Cloud](/help/integrations/assets/a4adc-lookbacks.png)

* Advertising Cloud-toewijzing klikt op terugzoekvenster: Het aantal dagen na de eerste klik waarin de klik aan een omzetting kan worden toegeschreven. Deze waarde is standaard 60 dagen; het maximum is 90 dagen
* Terugkijkvenster van Advertising Cloud-attribuutindruk: Het aantal dagen na een advertentie waarin de indruk aan een conversie kan worden toegeschreven. Deze waarde is standaard 14 dagen; het maximum is 30 dagen

   >[!NOTE]
   >
   > Het venster voor het terugzoeken van de indruk is specifiek voor Advertising Cloud en niet [!DNL Analytics for Advertising Cloud] voor het rapporteren.

In de JavaScript [!DNL Analytics for Advertising Cloud] worden deze instellingen gebruikt om te bepalen hoe ver u terug kunt gaan om een doorkijkitem of doorklikitem voor de site als geldig te beschouwen. Voor meer informatie over hoe mening-door en klik-door worden bepaald, zie &quot;[Advertising Cloud IDs die door Analytics](ids.md) wordt gebruikt.&quot;

## Advertising Cloud-gegevens in [!DNL Analytics]

[!DNL Analytics] Hiermee stelt u Advertising Cloud-id&#39;s (AMO-id&#39;s) in in de hit Analytics, afhankelijk van de persistentie-instelling van de eVar van de adverteerder. Deze instelling geldt voor zowel doorklikken als doorzoeken. De persistentie-instelling wordt geconfigureerd op de Advertising Cloud back-end en uw Adobe-accountmanager kan deze wijzigen.

* [!DNL Analytics for Advertising Cloud] Vervaldatum eVar: Standaard 60 dagen voor AMO-id&#39;s

>[!NOTE]
>
>Als u gegevens voor een ander tijdframe wilt segmenteren, kunt u [aangepaste segmenten](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html) instellen met verschillende opzoekvensters in Analysis Workspace.

## Ondersteunde advertentie-omgevingen

* Zoeken
* Weergave
* Video
* Online video
* Oorspronkelijk

Neem contact op met uw Adobe-accountmanager voor de meest recente ondersteunde advertentieomgevingen in elk kanaal.

## Wat u moet weten voordat u gaat implementeren

* Voor deze integratie worden geen extra kosten in rekening gebracht en serveraanroepen resulteren niet in extra [!DNL Analytics]- of Advertising Cloud-kosten.

* [!DNL Analytics for Advertising Cloud] is een advertentie voor serveragnost: kan een mening-door of klik-door van om het even welke advertentieserver voorkomen, en juiste IDs wordt geproduceerd bij plaatsingang.

* De integratie geeft Advertising Cloud alleen standaard- en aangepaste gebeurtenissen voor het optimaliseren van biedingen voor daaropvolgende betaalde media en advertentiepogingen door. [!DNL Analytics] Het gaat [!DNL Analytics] geen segmenten, berekende metriek, en eVars aan Advertising Cloud voor biodoptimalisering door.

* Advertising Cloud maakt permanente id&#39;s binnen [!DNL Analytics] op basis van de laatste advertentie die is geklikt of weergegeven voordat de gebruiker de site betreedt, op basis van de [click and view-through lookback windows](#lookback-a4adc) die in Advertising Cloud zijn geconfigureerd. Als een bezoeker van de site beide typen interactie voor site-invoer binnen zijn profiel zou hebben en de klik zich binnen de terugzoekperiode bevindt, zou de doorklikeid van de bezoeker de doorkijkID voor site-rapportage overschrijven.

* [!DNL Analytics for Advertising Cloud] Voor het bijhouden van conversies in Adobe Analytics wordt een configureerbaar terugzoekvenster (standaard 60 dagen) gebruikt. Advertising Cloud-rapporten weerspiegelen de omzettingen van sites en de betrokkenheid aan het einde van dit terugzoekvenster.

* Alle advertentietypen worden ondersteund. Niet alle advertentieomgevingen worden echter ondersteund.

   Zo worden aangesloten tv-advertenties (CTV-advertenties) niet bijgehouden omdat er geen kliks plaatsvinden in CTV en er geen conversies kunnen plaatsvinden op hetzelfde apparaat. Als de advertentie echter wordt weergegeven in een desktopomgeving, kunnen bepaalde gegevens van de doorkijksite worden bijgehouden.

* [!DNL Analytics] conversies worden momenteel bijgehouden en alleen toegewezen aan een bezoeker op hetzelfde apparaat.

* [!DNL Analytics for Advertising Cloud] ondersteunt geen in-app weergave-through conversies.

* Beeld-door volgen wordt niet gesteund voor adverteerders die een server-kant door:sturen implementatie van [!DNL Analytics] gebruiken.

### Aanvullende id

Als de Experience Cloud Identity Service voor een site is geïmplementeerd, bevatten hits die gegevens van [!DNL Analytics] of Advertising Cloud bevatten, een aanvullende id.

Voorbeeld: `sdid=2F3C18E511F618CC-45F83E994AEE93A0`

Voor nauwkeurige gegevensintegratie, moeten alle vraag van Advertising Cloud die door een [!DNL Analytics for Advertising Cloud] activiteit wordt gebruikt om inhoud te leveren of het doel metrisch te registreren overeenkomstige [!DNL Analytics] hebben die zelfde supplementaire identiteitskaart deelt.

Wanneer u het oplossen van problemen in [!DNL Analytics] bent, ben zeker om te bevestigen dat extra identiteitskaart voor [!DNL Analytics] treffers aanwezig is. In [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html), kunt u deze identiteitskaart op het lusje van Advertising Cloud als `sdid` parameter zien.

>[!NOTE]
>
> Deze implementatie werkt net als de integratie [!DNL Analytics for Target].

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [JavaScript-code voor analyse voor Advertising Cloud](/help/integrations/analytics/javascript.md)

