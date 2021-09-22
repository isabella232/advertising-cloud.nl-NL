---
title: Het gebruiken van [!DNL Roku] Overzicht
description: 'Leer over DSP partnerschap met [!DNL Roku], including inventory options, approved third-party tracking vendors, and best practices for [!DNL Roku]-specifieke stages. '
feature: DSP On Demand Inventory, DSP Private Inventory
exl-id: 0cd42782-f006-4aa8-b879-322f86cfac4b
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Inventaris [!DNL Roku] gebruiken

Advertising Cloud DSP biedt unieke functies voor advertenties op [!DNL Roku].

## Het partnerschap Advertising Cloud DSP en [!DNL Roku]

Roku en Advertising Cloud DSP hebben een uniek partnerschap dat overeenkomt met uw [!DNL DSP]-publiek tot [!DNL Roku]-id&#39;s voor een-op-een-deterministisch publiek dat zich richt op [!DNL Roku]-voorraad.

Buiten Roku&#39;s eigen DSP (OneView) heeft Advertising Cloud DSP de enige toegang tot deze doelmogelijkheden. Advertising Cloud DSP is ook de enige DSP met toestemming om [!DNL Roku]-voorraad naast alle andere voorraad aangesloten tv&#39;s (CTV) te meten. Omdat [!DNL Roku] niet alle standaard RTB- en pixelsignalen deelt, kan geen andere DSP zich richten of meten over Roku-verkochte CTV-levering.

## [!DNL Roku] Inventarisopties

U kunt of a) opstellings privé deal IDs direct met [!DNL Roku] en dan de gegevens van deal ID in DSP of b) bezoek de [!DNL On Demand] Galerij om aan [!DNL Roku] profielen in te tekenen:

>[!NOTE]
>
>[!DNL Roku] voorraad is niet beschikbaar in open markten en beurzen.

* Voor uw privé overeenkomsten, zult u [opstellingsinformatie over de overeenkomst IDs in DSP](/help/dsp/inventory/deal-id-create.md) en dan richten &quot;[!UICONTROL Roku Network – Audience]&quot;en &quot;[!UICONTROL The Roku Channel – Audience]&quot;binnen [!DNL Roku] plaatsen.<!-- Or do you target the deal ID?? I see those strings for Roku On Demand inventory. Clarify if all Roku private deals will show up as one or the other of these in Roku Private inventory in Roku placement settings. -->

* U kunt [zich op het volgende  [!DNL Roku] inventory within the [!DNL On Demand] Galerij](/help/dsp/inventory/on-demand-inventory-subscribe.md) abonneren, en dan om het even welke goedgekeurde overeenkomsten richten binnen [!DNL Roku] plaatsingen:

   * &quot;[!UICONTROL Roku Network – Audience]&quot; voor inventarisatie over het [!DNL Roku] ecosysteem met partners met premiuminhoud, zoals [!DNL The CW], [!DNL ABC], en [!DNL ESPN].
   * &quot;[!UICONTROL The Roku Channel – Audience]&quot; voor [!DNL Roku]-app-inhoud (O&amp;O) die in eigendom is en wordt gebruikt.

### Voordelen van het Aanpassen van Privémarkten met [!DNL Roku]

De privé overeenkomsten staan u toe om de overeenkomstenparameters aan te passen aan uw behoeften.

* **Onderhandelde tarifering:** Werk met het  [!DNL Roku] verkoopteam om een overeenkomst te bespreken en te structureren die aan uw campagnebehoeften voldoet.

* **Prioriteit schalen:** PMP&#39;s (Private Marketaces) krijgen een hogere prioriteit dan altijd-on deals (zoals  [!DNL On Demand] deals).

* **Frequentiebeheer:** de  [!DNL Roku] standaardfrequentiegrens is 1 (1) en per 30 minuten per gebruiker, maar u kunt de limiet aanpassen per uur, dag, week, maand of volledige vliegperiode.<!-- Within the DSP placement settings? NO - you negotiate this with Roku, but Christine to confirm with Amanda whether you should be able to edit this in placement. -->

* **[!DNL Roku]Data Targeting:** [!DNL Roku] het publiek wordt gebouwd van  [!DNL Roku] apparaat en TV signalen, gegevens die door  [!DNL The Roku Channel] (zoals de genre van TV, het stromen gedrag van TV, en de status van het kabelabonnement) worden gevolgd, en extra gegevens van het systeem van het de relatiebeheer van de  [!DNL Roku] klant (CRM).

* **[!DNL Roku]Inhoudsgericht:** persoonlijke deals kunnen zich richten op apps via genre, toepassing van app lijst van gewezen personen, seizoensgebonden en tentpole gebeurtenissen en  [!DNL The Roku Channel] alleen binnen deze toepassingen worden weergegeven.

## [!DNL Roku] Plaatsen

In DSP campagnes, zult u [creeer [!DNL Roku]-specifieke plaatsen](/help/dsp/campaign-management/placements/placement-create.md) gebruikend het plaatsingstype &quot;[!UICONTROL Connected TV (Roku)].&quot; U zult [!DNL Roku] plaatsingen in [!DNL Roku]-specifieke pakketten met bepaalde doelstellingen omvatten.

Elke [!DNL Roku] plaatsing moet minstens één [!DNL Roku] overeenkomst of bron richten. Als u DSP unieke publiek wilt gebruiken dat overeenkomt met [!DNL Roku], neemt u een of meer publiekssegmenten op die kunnen worden vergeleken met de [!DNL Roku] (opted-in) deterministische dataset.

### [!DNL Roku]-Goedgekeurde leveranciers van tracking van derden

[!DNL Roku] De plaatsing kan derdegebeurtenispixel en omzetingspixels van de volgende verkopers omvatten:   [!DNL Acxiom],  [!DNL comScore],  [!DNL Data Plus Math],  [!DNL Experian],  [!DNL Factual],  [!DNL Kantar],  [!DNL Marketing Evolution],  [!DNL Neustar],  [!DNL Nielsen],  [!DNL Nielsen Catalina Solutions],  [!DNL NinthDecimal]  [!DNL Oracle]  [!DNL Placed]  [!DNL Polk]  [!DNL Research Now], , , en .

### Beste praktijken door Plaatsingsstrategie

Hieronder vindt u de aanbevolen procedures voor [!DNL Roku]-specifieke plaatsingen.

Het incrementele bereik maximaliseren:

* Onderdruk blootgestelde soorten publiek op [!DNL Roku O&O] door publiek uit te sluiten u reeds gebruikend [!DNL The Roku Channel] hebt bereikt.

* Onderdruk blootgestelde soorten publiek op [!DNL All Roku] door publiek uit te sluiten u reeds over het [!DNL Roku] platform hebt bereikt.

Voor de snelste installatie:

* Bestaande, altijd-on deals voor [!DNL The Roku Channel] in [[!DNL On Demand] Inventaris](/help/dsp/inventory/on-demand-inventory-subscribe.md) richten om snel toegang te krijgen tot [!DNL Roku]-voorraad in eigendom en beheer.
* Bestaande, altijd-on deals voor [!DNL Roku Network] in [[!DNL On Demand] Inventaris](/help/dsp/inventory/on-demand-inventory-subscribe.md) richten om snel schalen te bereiken op het [!DNL Roku]-platform.

Op maximale schaal:

* Pas een [!DNL Roku] privé marktplaats voor prioritaire toegang tot [!DNL Roku] levering tegen een onderhandelde prijs aan.

>[!MORELIKETHIS]
>
>* [Handmatig details van deal-id maken](/help/dsp/inventory/deal-id-create.md)
> * [Abonneren en toegang aanvragen  [!DNL On Demand] tot Premium Inventory-aanbiedingen](/help/dsp/inventory/on-demand-inventory-subscribe.md)
>* [Een plaatsing maken](/help/dsp/campaign-management/placements/placement-create.md)

