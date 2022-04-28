---
title: 'Adobe Advertising Cloud-steun voor de California Consumer Privacy Act: Consumentenondersteuning voor uitverkoop'
description: Meer informatie over ondersteuning voor het vastleggen van aanvragen voor een opt-out voor consumenten.
feature: CCPA
exl-id: 2c0cd4f5-798f-479a-99cd-f555cd676766
source-git-commit: 2e0395dc1e5aa52adc83c1aaea49793fd5555390
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# Adobe Advertising Cloud Support for the California Consumer Privacy Act: Opt-out verkoopondersteuning voor consumenten

*Voor Adobe Advertising Cloud Demand Side Platform*

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridische adviseur voor advies over de California Consumer Privacy Act.

De California Consumer Privacy Act (CCPA) is de nieuwe privacywet van Californië, die op 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om toegang te krijgen tot hun gegevens en deze te verwijderen, alsook het recht om zich te onthouden van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke informatie aan derden worden aangemerkt.

Als bedrijf, zult u de persoonlijke gegevens bepalen die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, verleent Adobe Advertising Cloud steun voor uw zaken om aan zijn verplichtingen in het kader van CCPA te voldoen die op het gebruik van de producten en de diensten van Advertising Cloud van toepassing zijn, met inbegrip van het beheren van consumentenverzoeken om toegang tot en schrapping van persoonlijke informatie en het beheren van consumentenverzoeken om zich uit de verkoop van persoonlijke informatie te sluiten.

In dit document wordt beschreven hoe het Adobe Advertising Cloud Demand Side Platform (DSP) als dienstverlener het recht van de consument steunt om zich te onthouden van de &quot;verkoop&quot; van &quot;persoonlijke informatie&quot;, zoals elke term door de CCPA wordt gedefinieerd. Het bevat informatie over de manier waarop u aanvragen om te weigeren aan Advertising Cloud kunt doorgeven en over de manier waarop u rapporten kunt ophalen over de verzoeken van uw organisatie om zich af te melden.

Voor informatie over hoe Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform) en Media Optimizer DCO de toegang tot en het verwijderen van persoonlijke informatie van consumenten steunen, zie [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Toegang tot consumentengegevens en ondersteuning voor verwijderen](/help/privacy/ad-cloud-ccpa-access-delete.md).

Voor meer informatie over de diensten van de Privacy van de Adobe voor CCPA, zie [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Communiceren van consumentenverzoeken om niet langer te verkopen aan Advertising Cloud

Je kunt de aanvraag voor een opt-out bij verkoop aan de consument doorgeven met behulp van:

* een in Advertising Cloud DSP tot stand gekomen opt-out-of-sales-segment van de CCPA
* de Adobe Experience Platform Privacy Service API

### Methode 1: Deel CCPA uit-van-verkoop verzoeken gebruikend een [!UICONTROL CCPA Opt-Out-of-Sale] Segment in Advertising Cloud DSP

>[!NOTE]
>
>De gebruikers blijven in opt-out van CCPA-segmenten voor onbepaalde tijd.

1. Meld u aan bij de account van de adverteerder in Advertising Cloud DSP op [https://advertising.adobe.com/](https://advertising.adobe.com/).
1. [Creeer een opt-out van CCPA van verkoop segment, en voer het segmentpixel uit om de opt-out verzoeken te vangen](/help/dsp/audiences/ccpa-opt-out-segment-create.md).

### Methode 2: Deel CCPA uit-van-verkoop verzoeken gebruikend Adobe Experience Platform Privacy Service API

*Adverteerders hebben alleen een Adobe Experience Cloud-organisatie-id toegewezen*

1. Implementeer een JavaScript-bibliotheek om de cookies van uw klant op te halen. Dezelfde bibliotheek, `AdobePrivacy.js`, wordt gebruikt voor alle Adobe Experience Cloud-oplossingen.

   >[!IMPORTANT]
   >
   >Voor aanvragen bij sommige Adobe Experience Cloud-oplossingen is de JavaScript-bibliotheek niet vereist, maar aanvragen bij Advertising Cloud vereisen deze bibliotheek.

   U zou de bibliotheek op de Web-pagina moeten opstellen waarvan uw klanten opt-out-of-verkoop verzoeken, zoals het privacyportaal van uw bedrijf kunnen voorleggen. Met de bibliotheek kunt u Adobe-cookies ophalen (naamruimte-id: `gsurferID`), zodat u deze identiteiten kunt verzenden als onderdeel van een &quot;opt-out&quot;-aanvraag via de Adobe Experience Platform Privacy Service API.

1. Identificeer uw organisatie-id van de Experience Cloud en zorg ervoor dat deze is gekoppeld aan uw Advertising Cloud-accounts.

   Een Experience Cloud-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met &quot;@AdobeOrg&quot;. Aan de meeste klanten van Experience Cloud is een organisatie-id toegewezen. Als uw marketingteam of interne beheerder van het Adobe-systeem uw organisatie-id niet kent of niet zeker weet of deze is ingericht, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de organisatie-id nodig om aanvragen in te dienen bij de privacy-API met behulp van de `imsOrgID` naamruimte.

   >[!IMPORTANT]
   >
   >Neem contact op met de Advertising Cloud-vertegenwoordiger van uw bedrijf om te bevestigen dat alle Advertising Cloud-accounts van uw organisatie — inclusief [!DNL DSP] accounts of adverteerders, [!DNL Search] rekeningen, en [!DNL Creative] of [!DNL DCO] accounts — zijn gekoppeld aan uw Experience Cloud-organisatie-id.

1. De Adobe Experience Platform Privacy Service API gebruiken om [indiening van &quot;opt-out&quot;-verzoeken](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/consent.html) aan Advertising Cloud namens consumenten, en om de status van bestaande verzoeken te controleren.

   Zie de bijlage hieronder voor een voorbeeld van een &quot;opt-out&quot;-verzoek.

   >[!NOTE]
   Als uw bedrijf veelvoudige organisatie IDs van Experience Cloud heeft, dan moet u afzonderlijke API verzoeken voor elk verzenden. U kunt echter één API-aanvraag indienen voor meerdere Advertising Cloud-suboplossingen ([!DNL Search], [!DNL Creative], [!DNL DSP], en [!DNL DCO]), met één rekening per suboplossing.

Al deze stappen zijn nodig om steun van Advertising Cloud te ontvangen. Ga voor meer informatie over deze en andere verwante taken die u moet uitvoeren met de Adobe Experience Platform Privacy Service en waar u de benodigde items kunt vinden naar [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html).

## Rapporten ophalen van consumenten die verzoeken om niet-te verkopen hebben ingediend

Advertising Cloud genereert maandelijkse rapporten met id&#39;s die klanten hebben ingediend voor een aanvraag om te weigeren te verkopen voor de account. Elk rapport is beschikbaar als een tekstbestand met tabs als scheidingsteken en gecomprimeerd in de GZIP-indeling. De gegevens consolideren aanvragen die zijn vastgelegd met CCPA-opt-out-of-sales-segmenten die in Advertising Cloud DSP zijn gemaakt en alle aanvragen die via de Privacy Service-API zijn ingediend. In de CCPA-segmenten vastgelegde gebruikers-id&#39;s worden per segment en per adverteerder geïdentificeerd. Rapporten worden gegenereerd op de eerste van elke maand voor de vorige maand. De maandelijkse gebruikerslijst voor juni is bijvoorbeeld beschikbaar op 1 juli.

U kunt koppelingen ophalen naar de maandelijkse rapporten die in de afgelopen drie maanden zijn gemaakt, vanuit Advertising Cloud DSP of via de Advertising Cloud [!DNL Trafficking API]. Elke koppeling is zeven dagen geldig, maar wordt telkens vernieuwd wanneer een klant probeert een koppeling op te halen.

### Methode 1: Rapporten over verkoopopties voor consumenten in Advertising Cloud DSP ophalen

1. Meld u aan bij de account van de adverteerder in Advertising Cloud DSP op [https://advertising.adobe.com/](https://advertising.adobe.com/).
1. [De rapporten ophalen](/help/dsp/audiences/ccpa-opt-out-segment-report-retrieve.md).

### Methode 2: Rapporten met de verkoopoptie voor consumenten ophalen via de Advertising Cloud [!DNL Trafficking API]

Deze functie is beschikbaar voor organisaties die de [!DNL Trafficking API]. Zie de documentatie voor de [!DNL Trafficking API] voor meer informatie .

Als uw organisatie de opdracht [!DNL Trafficking API] maar is geïnteresseerd in meer informatie, neem contact op met uw [!DNL Adobe] accountteam.

## Aanhangsel: Voorbeeld [!UICONTROL CCPA Opt-Out-of-Sale] Aanvraag voor Privacy Service API-gebruikers

```
curl -X POST \
  https://platform.adobe.io/data/privacy/gdpr/ \
  -H 'Authorization: Bearer {ACCESS_TOKEN}' \
  -H 'Content-Type: application/json' \
  -H 'x-api-key: {API_KEY}' \
  -H 'x-gw-ims-org-id: {IMS_ORG}' \
  -d '{
    "companyContexts": [
      {
        "namespace": "imsOrgID",
        "value": "{IMS_ORG}"
      }
    ],
    "users": [
      {
        "key": "DavidSmith",
        "action": ["opt-out-of-sale"],
        "userIDs": [
          {
            "namespace": "email",
            "value": "dsmith@acme.com",
            "type": "standard"
          },
          {
            "namespace": "AdCloud",
            "type": "standard",
            "value":  "Wqersioejr-wdg",
          }
    ],
    "include": ["AdCloud"],
    "regulation": "ccpa"
}'
```

waarbij:

* `"namespace": "AdCloud"` Hiermee wordt de `AdCloud` koekjesruimte, en de overeenkomstige waarde is de koekjesidentiteitskaart van de klant zoals die van wordt teruggewonnen `AdobePrivacy.js`
* `"include": ["AdCloud"]` geeft aan dat de aanvraag van toepassing is op Advertising Cloud
