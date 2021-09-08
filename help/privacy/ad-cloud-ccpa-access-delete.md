---
title: Adobe Advertising Cloud support for the California Consumer Privacy Act &#58; Toegang tot consumentengegevens en ondersteuning voor verwijderen
description: Leer meer over de ondersteunde typen gegevensaanvragen, de vereiste instellingen en veldwaarden en voorbeelden van API-toegangsaanvragen met oude product-id's en geretourneerde gegevensvelden.
feature: CCPA
exl-id: 1330da6c-a944-4bb5-8539-488d97f56175
source-git-commit: 56ac178bf10d8c934297521ca3075783e1bc2c36
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Adobe Advertising Cloud Support for the California Consumer Privacy Act: Toegang tot consumentengegevens en ondersteuning voor verwijderen

*Voor Adobe Advertising Cloud Search, Adobe Advertising Cloud Creative, Adobe Advertising Cloud DSP en Adobe[!DNL Media Optimizer DCO]*

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridische adviseur voor advies over de California Consumer Privacy Act.

De California Consumer Privacy Act (CCPA) is de nieuwe privacywet van Californië, die op 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te verwijderen, alsmede het recht om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf, zult u de persoonlijke gegevens bepalen die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, verleent Adobe Advertising Cloud steun voor uw zaken om aan zijn verplichtingen in het kader van CCPA te voldoen die op het gebruik van de producten en de diensten van Advertising Cloud van toepassing zijn, met inbegrip van het beheren van verzoeken om toegang tot en schrapping van persoonlijke informatie en het beheren van verzoeken om zich uit de verkoop van persoonlijke informatie te sluiten.

In dit document wordt beschreven hoe Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform) en [!DNL Media Optimizer DCO] — als serviceproviders — het recht van consumenten op toegang tot en verwijdering van persoonlijke gegevens ondersteunen met behulp van de Adobe [!DNL Experience Platform Privacy Service API] en [!DNL Privacy Service UI].

Zie [Adobe Advertising Cloud Support for the California Consumer Privacy Act voor meer informatie over hoe Advertising Cloud DSP het recht van de consument om te weigeren om persoonlijke gegevens te verkopen ondersteunt: Support voor de optie-out voor consumenten](/help/privacy/ad-cloud-ccpa-opt-out-of-sale.md).

Voor meer informatie over de diensten van de Privacy van de Adobe voor CCPA, zie [het Centrum van de Privacy van de Adobe](https://www.adobe.com/privacy/ccpa.html).

## Ondersteunde gegevenstypen voor Advertising Cloud

Adobe Experience Platform biedt bedrijven de mogelijkheid om de volgende taken uit te voeren:

* Toegang tot gegevens op cookieniveau of gegevens op ID-niveau van een consument (voor advertenties in mobiele apps) binnen [!DNL Search], [!DNL Creative], [!DNL DSP] of [!DNL DCO].
* Gegevens op cookieniveau die zijn opgeslagen in [!DNL Search], [!DNL Creative], [!DNL DSP] of [!DNL DCO] verwijderen voor consumenten die een browser gebruiken; of gegevens op ID-niveau die zijn opgeslagen in [!DNL DSP] verwijderen voor consumenten die apps gebruiken op mobiele apparaten.
* Controleer de status van een of alle bestaande aanvragen.

## Vereiste installatie voor het verzenden van aanvragen voor Advertising Cloud

Als u verzoeken wilt indienen om persoonlijke gegevens van consumenten te benaderen en te verwijderen uit Advertising Cloud, moet u:

1. Implementeer een JavaScript-bibliotheek om de cookies van uw klant op te halen en te verwijderen. Dezelfde bibliotheek, `AdobePrivacy.js`, wordt gebruikt voor alle Adobe Experience Cloud-oplossingen.

   >[!IMPORTANT]
   >
   >Voor aanvragen bij sommige Adobe Experience Cloud-oplossingen is de JavaScript-bibliotheek niet vereist, maar aanvragen bij Advertising Cloud vereisen deze bibliotheek.

   U zou de bibliotheek op de Web-pagina moeten opstellen waarvan uw klanten toegang en schrappingsverzoeken, zoals het privacyportaal van uw bedrijf kunnen voorleggen. Met de bibliotheek kunt u Adobe-cookies ophalen (naamruimte-id: `gsurferID`) zodat u deze identiteiten als deel van toegang kunt voorleggen en verzoeken via [!DNL  Adobe Experience Platform Privacy Service API] schrappen.

   Wanneer de klant vraagt om persoonlijke gegevens te verwijderen, verwijdert de bibliotheek ook het cookie van de klant uit de browser van de klant.

   >[!NOTE]
   >
   >Het verwijderen van persoonlijke gegevens is anders dan het uitschakelen van gegevens, waardoor een eindgebruiker niet meer doelgericht met publiekssegmenten werkt. Wanneer een consument echter vraagt om persoonsgegevens te verwijderen uit [!DNL Creative], [!DNL DSP] of [!DNL DCO], verzendt de bibliotheek ook een verzoek aan Advertising Cloud om de klant te weigeren om zich te richten op segmenten. Voor adverteerders met [!DNL Search] adviseren wij dat u uw klanten een verbinding aan [https://www.adobe.com/privacy/opt-out.html#customeruse](https://www.adobe.com/privacy/opt-out.html#customeruse) verstrekt, die verklaart hoe te om uit doelgericht van publiekssegment te kiezen.

1. Identificeer uw IMS-organisatie-id en zorg ervoor dat deze is gekoppeld aan uw Advertising Cloud-accounts.

   Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met &quot;@AdobeOrg&quot;. Aan de meeste Adobe Experience Cloud-klanten is een IMS Org-id toegewezen. Als uw marketingteam of interne beheerder van het Adobe-systeem de IMS Org-id van uw organisatie niet kent of niet zeker weet of deze is ingericht, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org-id nodig om aanvragen in te dienen bij de Privacy-API.

   >[!IMPORTANT]
   >
   >Neem contact op met de Advertising Cloud-vertegenwoordiger van uw bedrijf om te bevestigen dat alle Advertising Cloud-accounts van uw organisatie, inclusief [!DNL DSP]-accounts of adverteerders, [!DNL Search]-accounts en [!DNL Creative]- of [!DNL DCO]-accounts, zijn gekoppeld aan uw IMS Org-id.

1. Gebruik [Adobe Experience Platform Privacy Service API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html) (voor geautomatiseerde verzoeken) of [Privacy Service UI](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html) (voor ad-hocverzoeken) om verzoeken om toegang tot en verwijdering van persoonlijke informatie namens consumenten naar Advertising Cloud te verzenden, en om de status van bestaande verzoeken te controleren.

   Voor adverteerders die een mobiele app hebben om met klanten te communiceren en campagnes te starten met [!DNL DSP], moet u de voor privacy geschikte mobiele SDK&#39;s voor Experience Cloud downloaden. De mobiele SDK&#39;s staan bedrijven toe om statusvlaggen voor weigeren in te stellen, de apparaat-id van de consument op te halen (naamruimte-id: `deviceID`) en verzend verzoeken naar de Privacy Service-API. Voor uw mobiele app is SDK-versie 4.15.0 of hoger vereist.

   Wanneer u een verzoek om toegang voor de consument indient, retourneert de Privacy Service-API de informatie van de consument op basis van de opgegeven cookie of apparaat-id, die u vervolgens aan de consument moet retourneren.

   Wanneer u een verzoek tot verwijdering van een consument indient, worden de cookie-id of apparaat-id en alle kosten, klik en inkomstengegevens die bij het cookie horen, van de server verwijderd.

   >[!NOTE]
   Als uw bedrijf meerdere Adobe Experience Cloud Identity Management Service Organization-id&#39;s (IMS Org ID&#39;s) heeft, moet u voor elke organisatie een aparte API-aanvraag verzenden. U kunt echter één API-aanvraag indienen voor meerdere Advertising Cloud-suboplossingen ([!DNL Search], [!DNL Creative], [!DNL DSP] en [!DNL DCO]), met één account per suboplossing.

Al deze stappen zijn nodig om steun van Advertising Cloud te ontvangen. Voor meer informatie over deze en andere verwante taken moet u het gebruiken van Adobe Experience Platform Privacy Service uitvoeren, en waar te om de punten te vinden u zult nodig hebben, zie [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html).

## Vereiste veldwaarden in Advertising Cloud JSON-verzoeken

`"company context":`

* `"namespace": **imsOrgID**`
* `"value":` &lt;>uw IMS Org ID-waarde *>*

&quot;gebruikers&quot;:

* `"key":` &lt;>gewoonlijk de naam van de klant *>*

* `"action":` hetzij  `**access**` hetzij  `**delete**`

* `"user IDs":`

   * `"namespace": **411**` (dit geeft de adcloud-cookieruimte aan)

   * `"value":` &lt;>de werkelijke waarde van de cookie-id van de klant, zoals opgehaald van  `AdobePrivacy.js`*>*

* `"include": **adCloud**` (dit is het product van de Adobe dat op het verzoek van toepassing is)

* `"regulation": **ccpa**` (dit is de privacyverordening die van toepassing is op het verzoek)

## Voorbeeld van een aanvraag die door een consument is ingediend met een Advertising Cloud-gebruikersnaam die is opgehaald van AdobePrivacy.js

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

Hieronder ziet u een voorbeeld van een reactie van Advertising Cloud op de toegang tot persoonlijke gegevens.

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
