---
title: 'Adobe Advertising support for the California Consumer Privacy Act: Toegang tot consumentengegevens en ondersteuning voor verwijderen'
description: Leer meer over de ondersteunde typen gegevensaanvragen, de vereiste instellingen en veldwaarden en voorbeelden van API-toegangsaanvragen met oude product-id's en geretourneerde gegevensvelden.
feature: CCPA
exl-id: e7808411-7dc3-499c-bda1-1f5882f651b2
source-git-commit: e9d9d51302d32b06af805917db2f46e5f6daee62
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Adobe Advertising Support for the California Consumer Privacy Act: Toegang tot consumentengegevens en ondersteuning voor verwijderen

*Voor [!DNL Adobe Advertising Search]; Adobe-DSP; Creatief reclame voor Adobe; en Adobe Advertising DCO*

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridische adviseur voor advies over de California Consumer Privacy Act.

De California Consumer Privacy Act (CCPA) is de nieuwe privacywet van Californië, die op 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te verwijderen, alsmede het recht om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf, zult u de persoonlijke gegevens bepalen die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, biedt de Reclame van de Adobe steun voor uw zaken om aan zijn verplichtingen uit hoofde van CCPA te voldoen die op het gebruik van de producten en de diensten van de Adobe Reclame van toepassing zijn, met inbegrip van het beheren van verzoeken om toegang tot en schrapping van persoonlijke informatie en het beheren van verzoeken om van de verkoop van persoonlijke informatie te kiezen.

In dit document wordt beschreven hoe [!DNL Advertising Search]; Creatief adverteren; DSP (Demand Side Platform); en [!DNL Advertising DCO] — als dienstverleners — het recht van de consument op toegang tot en verwijdering van persoonsgegevens met behulp van de Adobe ondersteunen [!DNL Experience Platform Privacy Service API] en [!DNL Privacy Service UI].

Voor informatie over de wijze waarop reclame DSP het recht van de consument om te weigeren gebruik te maken van de verkoop van persoonlijke informatie, raadpleegt u [Adobe Advertising Support for the California Consumer Privacy Act: Support voor consumenten](/help/privacy/ccpa/ccpa-opt-out-of-sale.md).

Voor meer informatie over de diensten van de Privacy van de Adobe voor CCPA, zie [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Ondersteunde gegevenstypen voor aanvragen voor Adobe-reclame

Adobe Experience Platform biedt bedrijven de mogelijkheid om de volgende taken uit te voeren:

* Toegang tot gegevens op cookieniveau of gegevens op ID-niveau van een consument (voor advertenties in mobiele apps) binnen [!DNL Search], [!DNL Creative], [!DNL DSP], of [!DNL DCO].
* Gegevens op cookieniveau verwijderen die zijn opgeslagen in [!DNL Search], [!DNL Creative], [!DNL DSP], of [!DNL DCO] voor consumenten die een browser gebruiken; of gegevens op ID-niveau verwijderen die zijn opgeslagen in [!DNL DSP] voor consumenten die apps op mobiele apparaten gebruiken.
* Controleer de status van een of alle bestaande aanvragen.

## Vereiste installatie voor het verzenden van verzoeken om Adobe-reclame

Om verzoeken tot toegang tot en schrapping van de persoonlijke informatie van de consument van Adobe Advertising, zult u moeten:

1. Implementeer een JavaScript-bibliotheek om de cookies van uw klant op te halen en te verwijderen. Dezelfde bibliotheek, `AdobePrivacy.js`, wordt gebruikt voor alle Adobe Experience Cloud-oplossingen.

   >[!IMPORTANT]
   >
   >Voor aanvragen naar bepaalde Experience Cloud-oplossingen is de JavaScript-bibliotheek niet vereist, maar voor aanvragen naar Adobe-advertentie is dit wel vereist.

   U zou de bibliotheek op de Web-pagina moeten opstellen waarvan uw klanten toegang en schrappingsverzoeken, zoals het privacyportaal van uw bedrijf kunnen voorleggen. Met de bibliotheek kunt u Adobe-cookies ophalen (naamruimte-id: `gsurferID`), zodat u deze identiteiten kunt verzenden als deel van toegang en verzoeken kunt schrappen via [!DNL Adobe Experience Platform Privacy Service API].

   Wanneer de klant vraagt om persoonlijke gegevens te verwijderen, verwijdert de bibliotheek ook het cookie van de klant uit de browser van de klant.

   >[!NOTE]
   >
   >Het verwijderen van persoonlijke gegevens is anders dan het uitschakelen van gegevens, waardoor een eindgebruiker niet meer doelgericht met publiekssegmenten werkt. Wanneer een consument echter om verwijdering van persoonsgegevens vraagt [!DNL Creative], [!DNL DSP], of [!DNL DCO], verzendt de bibliotheek ook een verzoek naar Adobe Advertising om de klant te weigeren zich te richten op segmenten. Voor adverteerders met [!DNL Search], adviseren wij u uw klanten een verbinding te verstrekken aan [https://www.adobe.com/privacy/opt-out.html#customeruse](https://www.adobe.com/privacy/opt-out.html#customeruse), die verklaart hoe te om uit doelgesegmenteerd publiekssegment te kiezen.

1. Identificeer uw organisatie-id van de Experience Cloud en zorg ervoor het met uw Adobe Advertising rekeningen wordt verbonden.

   Een Experience Cloud-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met &quot;@AdobeOrg&quot;. Aan de meeste klanten van Experience Cloud is een organisatie-id toegewezen. Als uw marketingteam of interne beheerder van het Adobe-systeem uw organisatie-id niet kent of niet zeker weet of deze is ingericht, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de organisatie-id nodig om aanvragen in te dienen bij de privacy-API met behulp van de `imsOrgID` naamruimte.

   >[!IMPORTANT]
   >
   >Neem contact op met de Adobe Advertising-vertegenwoordiger van uw bedrijf om te bevestigen dat alle accounts van uw organisatie voor Adobe-advertenties — inclusief [!DNL DSP] accounts of adverteerders, [!DNL Search] rekeningen, en [!DNL Creative] of [!DNL DCO] accounts — zijn gekoppeld aan uw Experience Cloud-organisatie-id.

1. Gebruik een van de [Adobe Experience Platform Privacy Service API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html) (voor geautomatiseerde verzoeken) of de [UI Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html) (voor ad-hocverzoeken) verzoeken om toegang tot en verwijdering van persoonsgegevens namens Adobe Advertising voor de consument in te dienen en de status van bestaande verzoeken te controleren.

   Voor adverteerders met een mobiele app om te communiceren met klanten en campagnes te starten met [!DNL DSP], moet u de voor privacy geschikte mobiele SDK&#39;s voor Experience Cloud downloaden. De mobiele SDK&#39;s staan bedrijven toe om statusvlaggen voor weigeren in te stellen, de apparaat-id van de consument op te halen (naamruimte-id: `deviceID`) en dient aanvragen in bij de Privacy Service-API. Voor uw mobiele app is SDK-versie 4.15.0 of hoger vereist.

   Wanneer u een verzoek om toegang voor de consument indient, retourneert de Privacy Service-API de informatie van de consument op basis van de opgegeven cookie of apparaat-id, die u vervolgens aan de consument moet retourneren.

   Wanneer u een verzoek tot verwijdering van een consument indient, worden de cookie-id of apparaat-id en alle kosten, klik en inkomstengegevens die bij het cookie horen, van de server verwijderd.

   >[!NOTE]
   Als uw bedrijf veelvoudige organisatie IDs van Experience Cloud heeft, dan moet u afzonderlijke API verzoeken voor elk verzenden. U kunt echter één API-aanvraag indienen voor meerdere Adobe Advertising-suboplossingen ([!DNL Search], [!DNL Creative], [!DNL DSP], en [!DNL DCO]), met één rekening per suboplossing.

Al deze stappen zijn nodig om steun van Adobe Advertising te ontvangen. Ga voor meer informatie over deze en andere verwante taken die u moet uitvoeren met de Adobe Experience Platform Privacy Service en waar u de benodigde items kunt vinden naar [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html).

## Vereiste veldwaarden in JSON-verzoeken voor Adobe-advertenties

`"company context":`

* `"namespace": **imsOrgID**`
* `"value":` &lt;*uw Experience Cloud-organisatie-id*>

&quot;gebruikers&quot;:

* `"key":` &lt;*gewoonlijk de naam van de klant*>

* `"action":` ofwel `**access**` of `**delete**`

* `"user IDs":`

   * `"namespace": **411**` (dit geeft de adcloud-cookieruimte aan)

   * `"value":` &lt;*de waarde van de cookie-id van de werkelijke klant, zoals opgehaald uit`AdobePrivacy.js`*>

* `"include": **adCloud**` (dit is het product van de Adobe dat op het verzoek van toepassing is)

* `"regulation": **ccpa**` (dit is de privacyverordening die van toepassing is op het verzoek)

## Voorbeeld van een aanvraag die door een consument is ingediend met een Adobe-advertentie-gebruikersnaam die van AdobePrivacy.js is opgehaald

```
{
"companyContexts":[
      {
         "namespace":"imsOrgID",
         "value":"5AB13068374019BC@AdobeOrg"
      }
   ],
   "users": [
{
 "key": "John Doe",
 "action":["access"],
  "userIDs":[
      {
         "namespace":"411",
         "value":"Wqersioejr-wdg",
         "type":"namespaceId",
         "deletedClientSide":false
      }
   ]
}
],
"include":[
      "adCloud"
   ],
    "regulation":"ccpa"
}
}
```

## Gegevensvelden die worden geretourneerd voor toegangsverzoeken

Hieronder ziet u een voorbeeld van een reactie op persoonlijke informatie over toegang tot Adobe-advertenties.

```
{
    "jobId":"12345AD43E",
    "action":"access",
    "product":"adCloud",
    "status":"complete",
    "results":{
        "userIDs":[
            {
                "namespace":"411",
                "userID":" Wqersioejr-wdg "
            }
        ],
        "receiptData":{
            "impressionCount":"100",
            "clickCount":5,
            "geo":[
                "United States of America",
                "San Francisco CA"
            ],
            "profile":[
                {
                    "pixelid":"111",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                },
                {
                    "pixelid":"123",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                }
            ],
            "matchingSegments":[
                {
                    "segmentName":"AP4 - Art/Culture - In-Market",
                    "segmentID":"kV1mPa2aqPNWKSNtf325",
                    "serviceProvider":"Adobe"
                },
                {
                    "segmentName":"EMEA - UK - Health Food Buyers",
                    "segmentID":"eP2oJ2UPsfsDVDhvlGewx",
                    "serviceProvider":"BlueKai"
                }
            ]
        }
    }
}
```
