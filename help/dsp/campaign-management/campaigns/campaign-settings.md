---
title: Campagne-instellingen
description: Zie beschrijvingen van de beschikbare campagnemontages.
feature: DSP Campaigns
exl-id: ff2e22ff-8073-4532-884b-36e0c1f22641
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Campagne-instellingen

## [!UICONTROL Basic Campaign Details]

**[!UICONTROL Name]:** De naam van de campagne.

**[!UICONTROL Advertiser]:** (Alleen-lezen voor bestaande campagnes) De toepasselijke adverteerder (merk). Selecteer een bestaande adverteerder of maak een nieuwe.

**[!UICONTROL Advertiser URL]:** De officiële pagina van de adverteerder. Dit veld versnelt het goedkeuringsproces voor advertenties met inventarispartners.

**[!UICONTROL Timezone]:** (Alleen-lezen voor bestaande campagnes) De tijdzone voor rapportage en biedingen.

**[!UICONTROL Customer PO]:** (Optioneel) Een inkooporder van een klant voor de invoegorder/inkooporder.

**[Campagnedatums]:** De begin- en einddatum van de campagne.

## [!UICONTROL Campaign Goals]

**[!UICONTROL Margin Management]:** Of marges voor de campagne moeten worden beheerd: *[!UICONTROL Yes]* of *[!UICONTROL No]* (de standaardinstelling).

Wanneer u *[!UICONTROL Yes],* het type en het bedrag van de marge specificeren:

* **[!UICONTROL Margin Type]:** Het type marge. U kunt het margetype niet veranderen zodra u margebeheer toelaat en de campagne bewaart.

   * *[!UICONTROL Fixed]:* (de standaardinstelling) Hiermee wordt DSP toegestaan uitgaven automatisch te berekenen en te beperken op basis van een vast margepercentage van het [!UICONTROL Gross Budget].

   * *[!UICONTROL Dynamic]:* Hiermee kunt u marges tot het plaatsingsniveau beheren door een aparte instelling op te geven [!UICONTROL Budget Reserve %] en [!UICONTROL Gross Budget] voor elk pakket en elke plaatsing in de campagne. DSP optimaliseert op basis van de financiële efficiëntie van elke plaatsing, zonder een specifieke marge te garanderen. Gebruik dit voor toevoegingsorden die uit veelvoudige lijnpunten bestaan waarvoor u bent overeengekomen om een vaste hoeveelheid eenheden of eenheidstypes aan een vaste tarief te leveren.

* **[!UICONTROL Fixed Margin %]:** (Alleen campagnes met vaste marges) De standaardmarkering voor elke invoegvolgorde <!-- impression? -->, als percentage. Dit bedrag wordt in mindering gebracht op het [!UICONTROL Gross Budget] de begroting van de nettocampagne vaststellen.

* **[!UICONTROL Budget Reserve %]:** (Campagnes met alleen vaste marges; (optioneel) Reserveert een bepaald percentage van de [!UICONTROL Gross Budget] als vrijwaringsmaatregel. Dit bedrag wordt in mindering gebracht op het [!UICONTROL Gross Budget] de begroting van de nettocampagne vaststellen.

**[!UICONTROL Gross Budget]:** (Campagnes met uitsluitend margebeheer) De begroting voor het bruto-prijsbeleid, vóór de opgegeven marginale aanpassingen worden toegepast.

U kunt desgewenst een extra bruto-budget per dag, week of maand toevoegen:

1. Klik op **[!UICONTROL Add an additional Gross Budget]**.

1. Voer de **[!UICONTROL Gross Budget]** en selecteert u de budgetinterval: *[!UICONTROL Daily],* *[!UICONTROL Weekly],* of *[!UICONTROL Monthly]*.

De totale nettobegroting, de uitgavenlimiet voor de campagne, wordt automatisch berekend op basis van de marge-instellingen en wordt onder deze waarde aangegeven.

**[!UICONTROL Budget]:** (Campagnes zonder margebeheer) Het totale campagnebudget.

**[!UICONTROL Estimated Tax Withholding]:** Hiermee wordt een percentage van de totale uitgaven bespaard voor advertentiekosten, honoreringskosten en/of gegevenskosten op rekeningniveau voor land- of lokale belastingen. Tarieven zijn ramingen voor budgettering en prijsstelling, zodat de gefactureerde belastingtarieven kunnen variëren.

Belastingen die moeten worden ingehouden ramen:

1. Klik op **[!UICONTROL Update rates here]**.

1. Geef de **[!UICONTROL Estimated tax rate]**, als percentage.

1. Schakel het selectievakje in naast elk type kosten waarvoor belastingen moeten worden ingehouden. De vergoedingstypen omvatten:

   * *[!UICONTROL Include estimated tax - ads fee]:* Is van toepassing op alle uitgaven voor advertenties DSP media, inclusief belastingen op kosten voor campagnebeheer.

   * *[!UICONTROL Include estimated tax - ad serving fee]:* Is van toepassing op alle uitgaven voor DSP, met uitzondering van media en gegevens. Hieronder vallen geen belastingen voor campagnebeheerkosten

   * *[!UICONTROL Include estimated tax - data fee]:* Is van toepassing op alle gegevens die worden besteed aan DSP.

1. Klik op **[!UICONTROL Submit]**.

>[!NOTE]
>
>* In de V.S., kunnen de staten in hun opname van belastingtarieven tussen advertenties, het dienen van, en gegevens variëren. Voor organisaties in andere landen worden alle drie de categorieën belastingtarieven opgenomen om de BTW te vergoeden.
>
>* U kunt deze waarden ook configureren in de instellingen voor accountkosten.<!--[fee settings](/help/dsp/admin/tax-withholdings.md). -->


**[!UICONTROL Cross Device Level]:** (Alleen-lezen voor bestaande campagnes die sinds 22 juni 2020 zijn opgezet; niet beschikbaar voor campagnes die vóór 22 juni 2020 zijn opgezet) Het niveau waarop DSP zich richt op advertenties en frequentieplafonds toepast: *Zelfde apparaat* een apparaat of *Mensen* om een persoon over al hun bekende apparaten te richten.

**[!UICONTROL Device Graph]:** (Alleen-lezen voor bestaande campagnes; campagnes met alleen op personen gebaseerde cross-device gerichte doelgroepen) De apparaatgrafiek die moet worden gebruikt voor apparaatgerichte toepassingen en frequentiebeheer:

* *[!UICONTROL LiveRamp - U.S. only]:* Beschikbaar aan alle adverteerders voor dwars-apparaat richtend bij $0.35 CPM voor beelden die door te gebruiken worden geleverd [!DNL LiveRamp] apparaatgrafiek (dat wil zeggen voor apparaten die niet worden gevonden binnen de doelpubliekssegmenten). U kunt een apparaatmarkering instellen op plaatsingsniveau.

   Deze optie is ook beschikbaar voor alle adverteerders, zonder vergoedingen, voor frequentiebeheer en attributiemeting.

**[!UICONTROL Frequency Cap]:** (Optioneel) Het aantal keren dat een uniek apparaat of een unieke persoon (afhankelijk van het opgegeven apparaat of de opgegeven persoon) [!UICONTROL Cross Device Level]) zal uit de campagne advertenties ontvangen. Opties omvatten *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand.

>[!NOTE]
>
> U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

**[!UICONTROL Packages]:** De [pakketten](/help/dsp/campaign-management/packages/package-about.md) in de campagne op te nemen. Selecteer bestaande pakketten en/of maak pakketten die u wilt opnemen. Als u pakketten maakt, raadpleegt u beschrijvingen over de [pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md) voor meer informatie .

## [!UICONTROL Campaign Measurement]

>[!NOTE]
>
>Met de volgende instellingen worden alleen meet- en rapportagemogelijkheden ingeschakeld. Prestaties worden alleen geoptimaliseerd op pakket- en plaatsingsniveau.

### [!UICONTROL 3rd Party Metrics]

#### [!UICONTROL Viewability, Fraud, & Brand Safety]

**[!UICONTROL IAS]:** (Optioneel) Inschakelen [!DNL IAS] meting en rapportage van gezichtsvermogen, fraude, merkveiligheid en publieksverificatie, met behulp van de opgegeven instellingen. Er zijn extra kosten van toepassing.

* **[!UICONTROL Measure On]:** De inventaris waarop wordt gemeten: *[!UICONTROL Display and VPAID video inventory]* (de standaardwaarde) of *[!UICONTROL Display, VPAID & VAST video inventory]*.

   >[!NOTE]
   >
   >De videoviewability is meetbaar op VPAID slechts inventaris.

* **[!UICONTROL IAS Account ID (AnID)]:** (Adverteerders [!DNL IAS] rekeningen; (facultatief) [!DNL IAS] account-id, die [!DNL IAS] rechtstreeks factureren voor gebruik.

* **[!UICONTROL IAS Team ID]:** (Adverteerders [!DNL IAS] rekeningen; (optioneel) De team-id voor de organisatie [!DNL IAS] account, welke [!DNL IAS] rechtstreeks factureren voor gebruik. <!-- verify -->

**[!UICONTROL MOAT]:** (Optioneel) Inschakelen [!DNL MOAT] meting en rapportage van gezichtsvermogen, fraude, merkveiligheid en verificatie van het publiek. Er zijn extra kosten van toepassing.

#### Verificatie door het publiek

**[!UICONTROL Nielsen]:** (Optioneel) Inschakelen [!DNL Nielsen] meting en rapportage van publieksverificatie, met behulp van de opgegeven instellingen. Er zijn extra kosten van toepassing.

* **[!UICONTROL Target Gender]:** Te bereiken geslacht: *[!UICONTROL Both]* (standaard), *[!UICONTROL Male]*, of *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** Het leeftijdsbereik dat moet worden nagestreefd. Gebruik de linker- en rechterschuifregelaars om het bereik zo nodig te verkleinen.

* **[!UICONTROL Target Country]:** (Optioneel) Een land dat als doel moet dienen. [!DNL Nielsen] zullen alleen de indrukken meten die in de gesteunde landen worden bediend.

**[!UICONTROL comScore vCE]:** (Optioneel) Inschakelen [!DNL Comscore validated Campaign Essentials (vCE)] meting en rapportage van publieksverificatie, met behulp van de opgegeven instellingen. Er zijn extra kosten van toepassing.

* **[!UICONTROL Target Gender]:** Te bereiken geslacht: *[!UICONTROL Both]* (standaard), *[!UICONTROL Male]*, of *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** Het leeftijdsbereik dat moet worden nagestreefd. Gebruik de linker- en rechterschuifregelaars om het bereik zo nodig te verkleinen.

* **[!UICONTROL Target Country]:** (Optioneel) Een land dat als doel moet dienen. [!DNL Comscore] zullen alleen de indrukken meten die in de gesteunde landen worden bediend.

### [!UICONTROL 1st Party Metrics]

**[!UICONTROL Viewability sensitivity]:** Hiermee worden metingen en rapportage van de gezichtsvermogen door de eerste partij mogelijk gemaakt met behulp van de [!DNL IAB Open Video Viewability (OpenVV)] technologie, gebaseerd op het gespecificeerde gevoeligheidsniveau:

* *[!UICONTROL Standard (50% of ad in view for two consecutive seconds)]*

* *[!UICONTROL Strict (100% of ad in view and audio on for 50% duration)]*

>[!MORELIKETHIS]
>
>* [Informatie over Campaign Management](campaign-about.md)
>* [Een campagne maken](campaign-create.md)
>* [Een campagne bewerken](campaign-edit.md)

