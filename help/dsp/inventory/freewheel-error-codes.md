---
title: Foutcodes voor [!DNL FreeWheel] Advertentie verzenden
description: Verwijs de foutencodes die voor ad voorlegging zijn teruggekeerd aan [!DNL FreeWheel].
feature: DSP Private Inventory, DSP Deal IDs
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# Foutcodes voor [!DNL FreeWheel] Advertentie verzenden

De foutberichten voor mislukte advertenties kunnen afkomstig zijn uit DSP of uit [!DNL FreeWheel]. Foutberichten worden weergegeven in het dialoogvenster [!UICONTROL API Response] in de [[!UICONTROL Freewheel Status] dialoogvenster](freewheel-check-status.md).

## Reclame DSP interne fouten

| Foutbericht | Beschrijving | Volgende stappen |
|--- |--- |--- |
| [!DNL Awaiting status response from [!DNL FreeWheel]] | [!DNL FreeWheel] heeft nog niet gereageerd dat de verzending is gelukt of mislukt. | Controleer de status over 10 minuten opnieuw. |
| [!DNL The submitted ad does not have a clock number assigned.] | [!DNL FreeWheel] Accepteert geen Britse advertenties zonder toegewezen kloknummers. | Wijs een kloknummer toe aan de advertentie en verzend de advertentie opnieuw. |
| [!DNL The ad you are attempting to submit has not yet finished transcoding. Please wait ten minutes then try again.] | De transcoder had het transcoderen van de advertentie niet gebeëindigd toen u probeerde om de advertentie voor te leggen. | Wacht tien minuten en verzend de advertentie opnieuw. |
| [!DNL The deal id you input is not setup as a guaranteed feed. Please submit guaranteed deals only.] | De voorgelegde overeenkomst wordt niet opgezet als programmatic gewaarborgde overeenkomst. [!DNL FreeWheel] accepteert alleen gegarandeerde deals. | Opstelling overeenkomstenidentiteitskaart als programmatic gewaarborgde overeenkomst. De advertentie wordt automatisch verzonden naar [!DNL FreeWheel] wanneer u sparen programmatic gewaarborgde standaardplaatsing aan het eind van het werkschema van identiteitskaart van de overeenkomst. |
| [!DNL Invalid external_deal_id:] \&lt;deal_id> | Voorgelegde overeenkomstenidentiteitskaart of bestaat niet of is niet actief op het eind van de Adobe. | Zorg ervoor dat de overeenkomst actief is, en verzend dan de advertentie opnieuw. |
| [!DNL \[public_id=]\&lt;deal>] bestaat niet | De voorgelegde overeenkomstenidentiteitskaart bestaat niet op [!DNL FreeWheel] einde. | Neem contact op met uw [!DNL FreeWheel] vertegenwoordiger om deal ID te bevestigen. |
| [!DNL Ad with identifier] \&lt;*advertentienaam*\> [!DNL was not found.] | De verzonden ad-toets bestaat niet of is niet actief aan de Adobe-zijde. | Zoek de juiste advertentiecode en verzend de advertentie opnieuw. |
| [!DNL Pending Submission] | De indiening is nog in behandeling. | Vernieuw de pagina. |

{style=&quot;table-layout:auto&quot;}

## [!DNL Freewheel] API-fouten

| Code | Betekenis | Beschrijving | Volgende stappen |
|--- |--- |--- |--- |
| 401 | Onbevoegd | Onjuiste, ontbrekende of ongeldige toegangsreferenties. | Neem contact op met uw [!DNL Adobe] accountteam. |
| 403 | Verboden | De server begreep het verzoek maar weigert het te autoriseren. | Neem contact op met uw [!DNL Adobe] accountteam. |
| 404 | Niet gevonden | De bron die u hebt aangevraagd, is niet beschikbaar. Als Creative ID niet wordt gevonden in de PUT bewerking, wordt een 404 geretourneerd. | Neem contact op met uw [!DNL Adobe] accountteam. |
| 405 | Methode niet toegestaan | Er is een verzoek ingediend van een bron die een aanvraagmethode gebruikt die niet door die bron wordt ondersteund (bijvoorbeeld door GET te gebruiken voor een methode die vereist dat gegevens door POST worden verzonden of door PUT te gebruiken voor een alleen-lezen bron). | Neem contact op met uw [!DNL Adobe] accountteam. |
| 408 | Tijdslimiet aanvraag | Er is een time-out opgetreden tijdens de verwerking van dit verzoek. De onderbrekingen worden gewoonlijk veroorzaakt door gezamenlijke verzoeken van exclusieve toegang tot bepaalde middelen. | Verzend het verzoek opnieuw wanneer u deze status ontvangt. Neem contact op met uw [!DNL Adobe] accountteam. |
| 422 | Onbewerkbare entiteit | Ongeldige bron. Deze fout gebeurt wanneer het verzoeklichaam ongeldig is of het gecreeerde/bijgewerkte middel ongeldig is (bijvoorbeeld, als identiteitskaart van de Overeenkomst niet werd gevonden). Zie [FreeWheel API 422-fouten](#freewheel-422-errors) voor meer informatie . | Neem contact op met uw [!DNL Adobe] accountteam. |
| 500 | Interne serverfout | API-systeemfout. | Neem contact op met uw [!DNL Adobe] accountteam. |

{style=&quot;table-layout:auto&quot;}

## [!DNL Freewheel] API 422-fouten {#freewheel-422-errors}

| Code | HTTP-code | Beschrijving |
|--- |--- |--- |
| DATA_UNMARSHALL_FAILURE | 422 | De aanvraaggegevens hebben een ongeldige JSON-indeling. Controleer het foutbericht voor meer informatie. |
| DATA_VALIDATION_FAILURE | 422 | De aanvraaggegevens ontbreken in de vereiste velden of hebben een ongeldig gegevenstype. Controleer het foutbericht voor meer informatie. |
| DATA_DEAL_INVALID | 422 | De overeenkomst wordt gevormd verkeerd of bestaat niet. Controleer het foutbericht voor meer informatie. |
| DATA_DEAL_GET_FAILURE | 422 | De overeenkomst werd niet gevonden of zijn configuratie heeft een kwestie. Controleer het foutbericht voor meer informatie. |
| DATA_CREATIVE_INGEST_FAILURE | 422 | De creatieve URL is ongeldig. Controleer het foutbericht voor meer informatie. |
| DATA_CREATIVE_LINK_FAILURE | 422 | De creatieve was niet verbonden met de knooppunten van de advertentie-eenheid van de deal. Controleer het foutbericht voor meer informatie. |
| DATA_CREATIVE_UPDATE_FAILURE | 422 | De creatieve functie is niet bijgewerkt. Controleer het foutbericht voor meer informatie. |
| DATA_DSP_GET_FAILURE | 422 | De DSP bestaat niet binnen het systeem. |
| DATA_CREATIVE_UNLINK_FAILURE | 422 | De creatieve objecten zijn niet losgekoppeld van advertentiefaciliteiten. |
| DATA_CREATIVE_DELETE_FAILURE | 422 | De creatieve functie is niet verwijderd. |
| DATA_CREATIVE_DETECTION_FAILURE | 422 | De URL is niet gedetecteerd. |
| DATA_ENTITY_NOT_FOUND | 422 | De creatieve bestaat niet. |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [Overzicht van de Opstelling Programma Gegarandeerde Overeenkomsten in [!DNL Freewheel]](/help/dsp/inventory/freewheel-overview.md)
>* [Accepteer een Overeenkomst in identiteitskaart Inbox van de Overeenkomst](deal-id-inbox-accept.md)
>* [Verzend Ad voor een Programma Gegarandeerde Overeenkomst aan [!DNL Freewheel]](/help/dsp/inventory/freewheel-submit.md)
>* [Controleer de status van advertenties voor [!DNL FreeWheel] Door programmacode gegarandeerde deals](/help/dsp/inventory/freewheel-check-status.md)

