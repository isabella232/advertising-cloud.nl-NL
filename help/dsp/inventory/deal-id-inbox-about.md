---
title: Over het [!UICONTROL Deal ID Inbox]
description: Meer informatie over de [!UICONTROL Deal ID inbox] functie, waarmee u persoonlijke deals kunt accepteren die u al met uitgevers hebt onderhandeld op [!DNL FreeWheel], [!DNL Google Authorized Buyers] (voorheen bekend als [!DNL AdX]), and [!DNL Magnite DV+] (voorheen) [!DNL Rubicon]).
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 959ad1d4-4671-4967-9f73-ec5b0464d0cd
source-git-commit: b40c6f08b94e546e5fc068c46b279292a4d8a14f
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Over het [!UICONTROL Deal ID Inbox]

DSP [!UICONTROL Deal ID inbox] staat u toe om opstellingsovereenkomsten snel te plaatsen die Advertising Cloud DSP van uitgevers door leveringszijplatforms (SSPs) heeft ingevoerd zodat moet u niet elke overeenkomst manueel opstelling. U kunt de gegarandeerde en niet-gegarandeerde privé-voorraadtransacties accepteren die u al met uitgevers hebt onderhandeld op [!DNL FreeWheel], [!DNL Google Authorized Buyers] (voorheen bekend als [!DNL AdX]), en [!DNL Magnite DV+] (voorheen) [!DNL Rubicon]) van de [!UICONTROL Deal ID inbox].

>[!NOTE]
>
>Advertising Cloud DSP is de eerste DSP die met de [!DNL FreeWheel] API.

In de [!UICONTROL Deal ID inbox], kunt u de details van de overeenkomst zien aangezien uw uitgever hen ziet, uw overeenkomstenopstelling versnellen, en handingangsfouten vermijden.

<!-- 
Accepting a deal automatically pre-populates a new Deal ID record with details from the publisher, and you need to enter only the publisher [always? or just in some cases?], the media type, who can access the deal, and any attribute labels to apply to the deal so it's easy to find. [Are labels a dimension you can report on?]

For each available deal, you can review the deal details sent directly from the publisher. Some deals are grouped as proposals (packages), and you can see the individual deal details by reviewing the deal.
   
You can accept any available deal or move an incorrect deal to the Ignored Deals tab. You can also un-ignore deals, which moves them back to the New Deals tab so you can potentially accept them.

For each deal, you can select one publisher and one media type (Desktop Video, Mobile Video, Connected TV, Display, or Audio), and you can share the deal with specific advertisers and with all advertisers for a specific account.
 -->

DSP vernieuwt automatisch alle overeenkomstendetails dagelijks om 4:30 a.m. EST. Het verfrist ook alle [!DNL FreeWheel] deals en updates van bestaande deals van [!DNL Google] en [!DNL Magnite DV+] uur. U kunt de overeenkomstendetails ook manueel verfrissen om nieuwe overeenkomsten op elk ogenblik te bevolken.

<!-- MC: I'm not sure where I got the following. Is this currently true? -->
>[!NOTE]
>
>Voor programmatiegarandeerde deals via [!DNL Google Authorized Buyers], moet u ten minste 90% van uw budget leveren, anders verliest uw account de toegang tot [!DNL Google] in de [!UICONTROL Deal ID inbox].

## De [!UICONTROL Deal ID Inbox]

Als u uw deals wilt ontvangen in de [!UICONTROL Deal ID inbox], moeten uw SSP rekeningen de DSP van uw organisatie aan uw SSP rekening in kaart brengen. DSP zal de de rekeningsnamen van de organisatie met relevante SSPs delen. Neem contact op met uw [!DNL Adobe] accountteam voor instructies.

Geef de uitgever tijdens de onderhandelingen over deals de deal door aan de koper in plaats van aan de bovenliggende DSP. De overeenkomstenherkenningsteken kan een naam of een identiteitskaart, afhankelijk van SSP zijn.

## Handelingen die u kunt uitvoeren

* **Overeenkomsten bekijken** om te verifiëren dat SSP de correcte uitgever, vluchtdata, CPM, en andere overeenkomstendetails heeft verzonden. Als de uitgever een fout heeft gemaakt, contacteer hen buiten DSP zodat kunnen zij de overeenkomst verbeteren en opnieuw verzenden.

* **Overeenkomsten accepteren** na revisie en worden niet meer weergegeven in het dialoogvenster [!UICONTROL Deal ID inbox]. Geaccepteerde deals worden aangeboden in [!UICONTROL Inventory] > [!UICONTROL Deals] en zijn klaar om zich te richten binnen de plaatsen van adverteerders.

* **Overeenkomsten negeren** die niet nodig of ongevraagd zijn. Genegeerde deals worden verplaatst naar de [!UICONTROL Ignored Deals] binnen de [!UICONTROL Deal ID inbox], die als archief fungeert. DSP waarschuwt geen SSPs en uitgevers wanneer u een overeenkomsten negeert.

* **Details wijzigen voor reeds geaccepteerde deals** van [!UICONTROL Inventory] > [!UICONTROL Deals] (niet in de [!UICONTROL Deal ID inbox]). Op dezelfde manier zijn adverteerders verantwoordelijk voor het implementeren van deze wijzigingen in [!UICONTROL Inventory] > [!UICONTROL Deals] omdat de [!UICONTROL Deal ID inbox] synchroniseert geen veranderingen van SSPs nadat de overeenkomsten opstelling zijn.

## Welke types van Overeenkomsten kunnen niet worden goedgekeurd?

Wanneer een lijst van deals geen ![Accepteren](/help/dsp/assets/accept.png) pictogram of een [!UICONTROL Accept] -knop, kunt u deze niet accepteren vanuit de [!UICONTROL Deal ID inbox]. In plaats daarvan kunt u [creeer manueel de details van identiteitskaart van de overeenkomst](/help/dsp/inventory/deal-id-create.md).

U kunt de volgende typen overeenkomsten niet accepteren:

* [!DNL Google] deals die niet in USD staan.

* [!DNL Magnite DV+] deals die niet in USD staan

* [!DNL FreeWheel] aanbiedingen die niet in je accountvaluta staan.

* Overeenkomsten die een einddatum vóór vandaag hebben.

* Oud [!DNL Magnite DV+] deals die werden gelabeld als &quot;meerdere mediatypen&quot;.

De overeenkomstendetails omvatten de reden de overeenkomst niet beschikbaar is te accepteren.

>[!MORELIKETHIS]
>
>* [Accepteer een Overeenkomst in identiteitskaart Inbox van de Overeenkomst](deal-id-inbox-accept.md)
>* [Overzicht van voorraadfuncties](inventory-overview.md)

