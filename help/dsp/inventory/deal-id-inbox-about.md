---
title: Informatie over [!UICONTROL Deal ID Inbox]
description: Leer over de [!UICONTROL Deal ID inbox] eigenschap, die u toestaat om privé overeenkomsten goed te keuren u reeds met uitgevers op [!DNL FreeWheel], [!DNL Google Authorized Buyers] (formerly known as [!DNL AdX]), and [!DNL Magnite DV+] (vroeger [!DNL Rubicon]) hebt onderhandeld.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 959ad1d4-4671-4967-9f73-ec5b0464d0cd
source-git-commit: 8046ec79ec24f47fe33e49c6097e44dbba450f1f
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Informatie over [!UICONTROL Deal ID Inbox]

DSP [!UICONTROL Deal ID inbox] staat u toe om overeenkomsten snel op te stellen die Advertising Cloud DSP van uitgevers door leveringszijplatforms (SSPs) heeft ingevoerd zodat moet u niet elke overeenkomst manueel opstelling. U kunt de gegarandeerde en niet-gegarandeerde privé inventarisovereenkomsten accepteren die u al met uitgevers hebt onderhandeld op [!DNL FreeWheel], [!DNL Google Authorized Buyers] (voorheen bekend als [!DNL AdX]) en [!DNL Magnite DV+] (voorheen [!DNL Rubicon]) van [!UICONTROL Deal ID inbox].

>[!NOTE]
>
>Advertising Cloud DSP is de eerste DSP die wordt geïntegreerd met de [!DNL FreeWheel]-API.

In [!UICONTROL Deal ID inbox], kunt u de details van de overeenkomst zien aangezien uw uitgever hen ziet, uw overeenkomstenopstelling versnellen, en handingangsfouten vermijden.

DSP vernieuwt automatisch alle overeenkomstendetails dagelijks om 4:30 a.m. EST. Ook worden alle [!DNL FreeWheel] deals vernieuwd en worden bestaande deals van [!DNL Google] en [!DNL Magnite DV+] per uur bijgewerkt. U kunt de overeenkomstendetails ook manueel verfrissen om nieuwe overeenkomsten op elk ogenblik te bevolken.

<!-- MC: I'm not sure where I got the following. Is this currently true? -->
>[!NOTE]
>
>Voor programmatic gegarandeerde deals via [!DNL Google Authorized Buyers] moet u ten minste 90% van uw budget leveren, anders verliest uw account de toegang tot [!DNL Google] deals in [!UICONTROL Deal ID inbox].

## De [!UICONTROL Deal ID Inbox] implementeren

Om uw overeenkomsten in [!UICONTROL Deal ID inbox] te ontvangen, moeten uw SSP rekeningen de DSP van uw organisatie aan uw SSP rekening in kaart brengen. DSP zal de de rekeningsnamen van de organisatie met relevante SSPs delen. Neem voor instructies contact op met uw Adobe-accountmanager.

Geef de uitgever tijdens de onderhandelingen over deals de deal door aan de koper in plaats van aan de bovenliggende DSP. De overeenkomstenherkenningsteken kan een naam of een identiteitskaart, afhankelijk van SSP zijn.

## Handelingen die u kunt uitvoeren

* **De** termijnen van het overzicht om te verifiëren dat SSP de correcte uitgever, vluchtdata, CPM, en andere overeenkomstendetails heeft verzonden. Als de uitgever een fout heeft gemaakt, contacteer hen buiten DSP zodat kunnen zij de overeenkomst verbeteren en opnieuw verzenden.

* **Accepteer** de details na het controleren en deze worden niet meer weergegeven in de  [!UICONTROL Deal ID inbox]lijst. Geaccepteerde deals worden aangeboden in [!UICONTROL Inventory] > [!UICONTROL Deals] en zijn klaar om te worden gebruikt binnen de plaatsen van adverteerders.

* **Negeer** details die niet nodig of ongevraagd zijn. Genegeerde deals worden verplaatst naar het tabblad [!UICONTROL Ignored Deals] in het [!UICONTROL Deal ID inbox], dat als archief fungeert. DSP waarschuwt geen SSPs en uitgevers wanneer u een overeenkomsten negeert.

* **Wijzig details voor reeds-toegelaten** schrapping van  [!UICONTROL Inventory] >  [!UICONTROL Deals] (niet in  [!UICONTROL Deal ID inbox]). Op dezelfde manier wanneer uitgevers veranderingen in overeenkomsten verzenden, zijn de adverteerders verantwoordelijk voor het uitvoeren van die veranderingen in [!UICONTROL Inventory] > [!UICONTROL Deals] omdat [!UICONTROL Deal ID inbox] veranderingen van SSPs na opstelling niet synchroniseert.

## Welke types van Overeenkomsten kunnen niet worden goedgekeurd?

Wanneer een overeenkomstenlijst geen ![Accept](/help/dsp/assets/accept.png) pictogram of [!UICONTROL Accept] knoop omvat, kunt u niet het van [!UICONTROL Deal ID inbox] goedkeuren. In plaats daarvan, kunt u [de details van identiteitskaart van de overeenkomst manueel tot stand brengen](/help/dsp/inventory/deal-id-create.md).

U kunt de volgende typen overeenkomsten niet accepteren:

* [!DNL Google] deals die niet in USD staan.

* [!DNL Magnite DV+] deals die niet in USD staan

* [!DNL FreeWheel] aanbiedingen die niet in je accountvaluta staan.

* Overeenkomsten die een einddatum vóór vandaag hebben.

* Oude overeenkomsten [!DNL Magnite DV+] die als &quot;veelvoudige media types.&quot;werden geëtiketteerd

De overeenkomstendetails omvatten de reden de overeenkomst niet beschikbaar is te accepteren.

>[!MORELIKETHIS]
>
>* [Accepteer een Overeenkomst in identiteitskaart Inbox van de Overeenkomst](deal-id-inbox-accept.md)
>* [Overzicht van voorraadfuncties](inventory-overview.md)

