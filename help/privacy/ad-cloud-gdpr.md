---
title: Adobe Advertising Cloud-steun voor de algemene gegevensbeschermingsverordening
description: Meer informatie over de ondersteunde gegevenstypen voor aanvragen, de vereiste instellingen en veldwaarden en voorbeelden van API-toegangsaanvragen met oude product-id's en geretourneerde gegevensvelden
feature: GDPR
exl-id: 304d88d0-d63d-4b32-8d4d-c61ba2409adc
source-git-commit: 2e0395dc1e5aa52adc83c1aaea49793fd5555390
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Adobe Advertising Cloud-steun voor de algemene gegevensbeschermingsverordening

*Voor Adobe Advertising Cloud Search, Adobe Advertising Cloud Creative, Adobe Advertising Cloud DSP en Adobe Media Optimizer DCO*

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de algemene verordening inzake gegevensbescherming.

De algemene gegevensbeschermingsverordening (GDPR), een wet die op 25 mei 2018 van kracht is, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens en vereenvoudigt het regelgevingskader voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud treedt op als een gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform) en Media Optimizer DCO de toegang tot en het verwijderen van GDPR-gegevens van de betrokkenen ondersteunen met behulp van de Adobe Experience Platform Privacy Service API en de interface van de Privacy Service.

Voor meer informatie over wat GDPR voor uw zaken betekent, zie [GDPR en uw bedrijf](https://www.adobe.com/privacy/general-data-protection-regulation.html).

## Ondersteunde gegevenstypen voor Advertising Cloud

Adobe Experience Platform biedt bedrijven de mogelijkheid om de volgende taken uit te voeren:

* Toegang tot gegevens op cookieniveau of gegevens op id-niveau van een apparaat (voor advertenties in mobiele apps) op [!DNL Search], [!DNL Creative], [!DNL DSP], of [!DNL DCO].
* Gegevens op cookieniveau verwijderen die zijn opgeslagen in [!DNL Search], [!DNL Creative], [!DNL DSP], of [!DNL DCO] voor betrokkenen die een browser gebruiken; of gegevens op ID-niveau verwijderen die zijn opgeslagen in [!DNL DSP] voor betrokkenen die apps gebruiken op mobiele apparaten.
* Controleer de status van een of alle bestaande aanvragen.

## Vereiste installatie voor het verzenden van aanvragen voor Advertising Cloud

Als u toegang wilt vragen tot gegevens voor Advertising Cloud en deze wilt verwijderen, moet u:

1. Implementeer een JavaScript-bibliotheek om de cookies van het gegevenssubject op te halen en te verwijderen. Dezelfde bibliotheek, `AdobePrivacy.js`, wordt gebruikt voor alle Adobe Experience Cloud-oplossingen.

   >[!IMPORTANT]
   >
   >Voor aanvragen bij sommige Adobe Experience Cloud-oplossingen is de JavaScript-bibliotheek niet vereist, maar aanvragen bij Advertising Cloud vereisen deze bibliotheek.

   U moet de bibliotheek implementeren op de webpagina waarvan de betrokkene toegang kan verzenden en aanvragen kan verwijderen, zoals het privacyportaal van uw bedrijf. Met de bibliotheek kunt u Adobe-cookies ophalen (naamruimte-id: `gsurferID`), zodat u deze id&#39;s kunt verzenden als onderdeel van toegangs- en verwijderaanvragen via de Adobe Experience Platform Privacy Service API.

   Wanneer de betrokkene om verwijdering van persoonsgegevens vraagt, verwijdert de bibliotheek ook het cookie van de betrokkene uit de browser van de betrokkene.

   >[!NOTE]
   >
   >Het schrappen van persoonlijke gegevens is verschillend dan uit Opt, die het richten van een eindgebruiker met publiekssegmenten tegenhoudt. Wanneer een betrokkene echter om verwijdering van persoonsgegevens verzoekt [!DNL Creative], [!DNL DSP], of [!DNL DCO], stuurt de bibliotheek ook een verzoek aan Advertising Cloud om de betrokkene uit te sluiten van segmentgerichtheid. Voor adverteerders met [!DNL Search], adviseren wij u een verbinding te verstrekken aan de betrokkenen [https://www.adobe.com/privacy/opt-out.html](https://www.adobe.com/privacy/opt-out.html), die verklaart hoe te om uit doelgesegmenteerd publiekssegment te kiezen.

1. Identificeer uw organisatie-id van de Experience Cloud en zorg ervoor het met uw rekeningen van Advertising Cloud verbonden is.

   Een Experience Cloud-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met &quot;@AdobeOrg&quot;. Aan de meeste klanten van Experience Cloud is een organisatie-id toegewezen. Als uw marketingteam of interne beheerder van het Adobe-systeem uw organisatie-id niet kent of niet zeker weet of deze is ingericht, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de organisatie-id nodig om aanvragen in te dienen bij de privacy-API met behulp van de `imsOrgID` naamruimte.

   >[!IMPORTANT]
   >
   >Neem contact op met de Advertising Cloud-vertegenwoordiger van uw bedrijf om te bevestigen dat alle Advertising Cloud-accounts van uw organisatie — inclusief [!DNL DSP] accounts of adverteerders, [!DNL Search] rekeningen, en [!DNL Creative] of [!DNL DCO] accounts — zijn gekoppeld aan uw Experience Cloud-organisatie-id.

1. Gebruik een van de [Adobe Experience Platform Privacy Service API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html) (voor geautomatiseerde verzoeken) of de [UI Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html) (voor ad-hocverzoeken) om namens de betrokkenen verzoeken om toegang en om verwijdering naar Advertising Cloud in te dienen, en om de status van bestaande verzoeken te controleren.

   Voor adverteerders die een mobiele app hebben om te communiceren met de betrokkenen en campagnes te starten met de DSP, moet u de voor privacy geschikte mobiele SDK&#39;s voor Experience Cloud downloaden. De mobiele SDK&#39;s staan gegevenscontrollers toe om statusmarkeringen voor weigeren in te stellen, de apparaat-id van de betrokkene op te halen (naamruimte-id: deviceID), en verzoeken indienen bij de Privacy Service-API. Voor uw mobiele app is SDK-versie 4.15.0 of hoger vereist.

   Wanneer u het toegangsverzoek van een betrokkene verzendt, retourneert de Privacy Service-API de informatie van de betrokkene op basis van de opgegeven cookie of apparaat-id, die u vervolgens moet terugsturen naar de betrokkene.

   Wanneer u het verwijderingsverzoek van een betrokkene verzendt, worden de cookie-id of apparaat-id en alle kosten, klik en inkomstengegevens die bij het cookie horen, van de server verwijderd.

   >[!NOTE]
   Als uw bedrijf veelvoudige Experience Cloud organisatie IDs heeft, dan moet u afzonderlijke API verzoeken voor elk verzenden. U kunt echter één API-aanvraag indienen voor meerdere Advertising Cloud-suboplossingen ([!DNL Search], [!DNL Creative], [!DNL DSP], en [!DNL DCO]), met één rekening per suboplossing.

Al deze stappen zijn nodig voor Advertising Cloud. Ga voor meer informatie over deze en andere verwante taken die u moet uitvoeren met de Adobe Experience Platform Privacy Service en waar u de benodigde items kunt vinden naar [www.adobe.io/apis/cloudplatform/gdpr.html](https://www.adobe.io/apis/experienceplatform/gdpr.html).

## Vereiste veldwaarden in Advertising Cloud JSON-verzoeken

&quot;&quot;bedrijfcontext&quot;:

* `"namespace": **imsOrgID**`
* `"value":` &lt;*uw IMS Org ID-waarde*>

`"users":`

* `"key":` &lt;*gewoonlijk de naam van de betrokkene*>

* `"action":` ofwel `**access**` of `**delete**`

* `"user IDs":`

   * `"namespace": **411**` (die de [!DNL adcloud] cookie spatie)

   * `"value":` &lt;*de eigenlijke waarde van de cookie-id van de betrokkene, zoals opgehaald uit`AdobePrivacy.js`*>

* `"include": **adCloud**` (dit is het product van de Adobe dat op het verzoek van toepassing is)

* `"regulation": **gdpr**` (dit is de privacyverordening die van toepassing is op het verzoek)

## Voorbeeld van een aanvraag die is ingediend door de betrokkene met een Advertising Cloud-gebruikersnaam die is opgehaald van `AdobePrivacy.js`

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
    "regulation":"gdpr"
}
}
```

## Gegevensvelden die worden geretourneerd voor toegangsverzoeken

Hieronder ziet u een voorbeeld van een toegangsreactie voor Advertising Cloud.

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
