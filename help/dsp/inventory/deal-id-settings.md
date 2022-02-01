---
title: Instellingen voor handmatige deal-id
description: Zie beschrijvingen van de montages voor manueel-binnengegaane overeenkomst IDs.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 0cd5e9e8-2b13-4b1e-a2e0-b8b492f75acf
source-git-commit: cf08c97a6a9fecd637f1776b186a18a5c5cc6435
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Instellingen voor handmatige deal-id

| Sectie | Parameter | Beschrijving | Vereist | Bewerkbaar |
|---------|-----------|-------------|----------|----------|
| [Details van deal] | [!UICONTROL Deal name] | De naam waarmee u uw [!UICONTROL Deal ID] in Advertising Cloud DSP. Geef een naam op of selecteer **[!UICONTROL Auto-name]** om Advertising Cloud een naam te laten produceren die op de overeenkomstendetails wordt gebaseerd.<br><br>Voorbeeld van een automatisch gegenereerde naam: `[!DNL 24159708 - Deal ID - Guaranteed Fixed - USD - 5 - 24Kitchen - Private]` | Ja | Ja |
|  | [!UICONTROL External deal ID] | Identiteitskaart die door uw uitgever en SSP wordt gebruikt om deze overeenkomst te identificeren. | Ja | Nee |
|  | [!UICONTROL Publisher] | De naam van de uitgever die deze voorraad verkoopt. | Ja | Nee |
|  | [!UICONTROL SSP] | Het platform aan de aanbodzijde (SSP) waardoor deze overeenkomst zal lopen. | Ja | Nee |
|  | [!UICONTROL Media type] | Het type media dat door deze overeenkomst zal worden gekocht: *[!UICONTROL Desktop video]*, *[!UICONTROL Mobile video]*, *[!UICONTROL Connected TV]*, *[!UICONTROL Display]*, of *[!UICONTROL Audio]*. De opties variëren door SSP.<br><br> Als de overeenkomst veelvoudige media types toestaat, selecteer het media type voor de standaardplaatsing wanneer u de overeenkomst creeert. Later kunt u de waarde wijzigen of alleen [een nieuwe plaatsing koppelen met het extra mediatype](deal-id-attach-placements.md).<!-- It would be ideal if this field was multi-select rather than a radio button, so you don't have to "change" the value later. --> | Ja | Nee |
|  | [!UICONTROL Deal type] | De deal-verplichting en prijsstructuur:<br><ul><li>*[!UICONTROL Non guaranteed (floor)]*: U en de uitgever hebben zich niet verbonden aan een vast aantal beeldleveringen. De transactie specificeert de minimumprijs voor de inventaris, hoewel het CPM kan fluctueren en stijgen afhankelijk van de marktvoorwaarden.</li><li>*[!UICONTROL Non guaranteed (fixed)]*: U en de uitgever hebben zich niet verbonden aan een vast aantal beeldleveringen. Prijzen worden vastgesteld tegen een door onderhandelingen bepaalde vaste koers.</li><li>*[!UICONTROL Guaranteed (fixed)]*: U en de uitgever zijn het eens geworden over een vooraf gedefinieerd aantal indrukken, doelframes, vliegdatums en vaste prijs.<br><br><b>Opmerking:</b> Gegarandeerde deals vereisen vluchtdatums en een bepaald aantal indrukken in de [!UICONTROL Tracking] sectie. U zult ook een standaard programmatic gegarandeerde plaatsing (PG) voor de overeenkomst moeten creëren, en u kunt naar keuze de overeenkomst voor andere plaatsen in plaats daarvan gebruiken.</li></ul> | Ja | Nee |
|  | [!UICONTROL CPM] | De overeengekomen kosten per duizend impressies (CPM). | Ja | Ja |
|  | [Valuta] | De valuta voor de deal.<br><br>Alle SSPs keurt overeenkomsten in USD goed. Wanneer het SSP de valuta voor uw DSP rekening goedkeurt, is die munt ook beschikbaar. | Ja | Nee |
|  | [!UICONTROL Billing method] | Alle deal-IDs is [!DNL Adobe]-gefinancierd en gefactureerd. Advertising Cloud betaalt alle beschikbare media-leveranciers op basis van gebruik, beheert discrepanties met de leveranciers en stuurt één geconsolideerde factuur naar de account. Voor deze optie worden extra kosten in rekening gebracht zoals aangegeven op de betaalkaart van de account. | Ja | Nee |
| [!UICONTROL Advertisers] | [!UICONTROL Account email] | Het e-mailadres voor de gebruikersrekening die tot de overeenkomst kan toegang hebben. | Nee | Ja |
|  | [!UICONTROL Advertisers that can access this deal] | De specifieke adverteerders in de rekening die tot deze overeenkomst kunnen toegang hebben.<br><br><b>Opmerking:</b> U kunt de overeenkomst met adverteerders delen in extra accounts van de [!UICONTROL Deals] weergeven. In de overeenkomstenrij, klik **[!UICONTROL #]**, klikt u op **[!UICONTROL share]** en deel de deal met een e-mailadres. | Ja | Ja |
| [!UICONTROL Tracking] | [!UICONTROL Flight Dates] | De begin en einddata voor verkeer die deze overeenkomst gebruiken. Deze datum is alleen bedoeld voor traceringsdoeleinden en heeft geen invloed op de levering.<br><br><b>Tip:</b> In de [!UICONTROL Inventory] > [!UICONTROL Deals] de [!UICONTROL Pacing & Budget] de kolom zal tonen hoe de overeenkomst aan het gespecificeerde vliegdatum en imperiatiedoel past. Als de levering onderaan of overpakking is, contacteer uw uitgever om aan te passen hoeveel volume het door de overeenkomst verzendt. | Gegarandeerde deals: Ja<br>Niet-gegarandeerde transacties: Nee | Ja |
|  | [!UICONTROL Impressions] | (Optioneel voor niet-gegarandeerde deals) Het geschatte aantal indrukkingen dat u verwacht te kunnen uitvoeren met deze deal. Deze waarde is alleen voor traceringsdoeleinden; de uitgever controleert en levering. | Gegarandeerde deals: Ja<br>Niet-gegarandeerde transacties: Nee | Ja |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [Handmatig details van deal-id maken](deal-id-create.md)
>* [SSP-partners](ssp-partners.md)
>* [Informatie over privé-voorraad](private-inventory-about.md)

