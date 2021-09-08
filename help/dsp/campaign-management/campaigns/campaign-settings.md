---
title: Campagne-instellingen
description: Zie beschrijvingen van de beschikbare campagnemontages.
feature: Campaigns
exl-id: ff2e22ff-8073-4532-884b-36e0c1f22641
source-git-commit: e2ee41c7e3e195f062ad1cc67080ed913d6d3d06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Campagne-instellingen

## [!UICONTROL Basic Campaign Details]

**[!UICONTROL Name]:** De naam van de campagne.

**[!UICONTROL Advertiser]:** (Alleen-lezen voor bestaande campagnes) De toepasselijke adverteerder (merk). Selecteer een bestaande adverteerder of maak een nieuwe.

**[!UICONTROL Advertiser URL]:** De officiële pagina van de adverteerder. Dit veld versnelt het goedkeuringsproces voor advertenties met inventarispartners.

**[!UICONTROL Timezone]:** (Alleen-lezen voor bestaande campagnes) De tijdzone voor rapportage en biedingen.

**[!UICONTROL Customer PO]:** (Optioneel) Een inkooporder van een klant voor de order/inkooporder.

**[Campagnedatums]:** de begin- en einddatum van de campagne.

## [!UICONTROL Campaign Goals]

**[!UICONTROL Margin Management]:** Of marges voor de campagne moeten worden beheerd:  *[!UICONTROL Yes]* of  *[!UICONTROL No]* (de standaardinstelling).

Wanneer u *[!UICONTROL Yes]kiest,* specificeer het margetype en de hoeveelheid:

* **[!UICONTROL Margin Type]:** Het type marge. U kunt het margetype niet veranderen zodra u margebeheer toelaat en de campagne bewaart.

   * *[!UICONTROL Fixed]:* (standaard) Hiermee staat u Advertising Cloud DSP toe om uitgaven automatisch te berekenen en te beperken op basis van een vast margepercentage van de  [!UICONTROL Gross Budget]waarde.

   * *[!UICONTROL Dynamic]:* Hiermee kunt u marges tot het plaatsingsniveau beheren door een afzonderlijk  [!UICONTROL Budget Reserve %] en  [!UICONTROL Gross Budget] voor elk pakket en elke plaatsing in de campagne op te geven. Advertising Cloud DSP optimaliseert op basis van de financiële efficiëntie van elke plaatsing, zonder een specifieke marge te garanderen. Gebruik dit voor toevoegingsorden die uit veelvoudige lijnpunten bestaan waarvoor u bent overeengekomen om een vaste hoeveelheid eenheden of eenheidstypes aan een vaste tarief te leveren.

* **[!UICONTROL Fixed Margin %]:** (Campagnes met vaste marges slechts) De standaardprijsverhoging voor elke toevoegingsorde  <!-- impression? -->, als percentage. Dit bedrag wordt in mindering gebracht op de [!UICONTROL Gross Budget] om het netto campagnebudget te bepalen.

* **[!UICONTROL Budget Reserve %]:** (campagnes met alleen vaste marges; (facultatief) reserve een gespecificeerd percentage van het  [!UICONTROL Gross Budget] als veiligheidswaarborg. Dit bedrag wordt in mindering gebracht op de [!UICONTROL Gross Budget] om het netto campagnebudget te bepalen.

**[!UICONTROL Gross Budget]:** (Campagnes met uitsluitend margebeheer) De begroting voor het bruto-campagne vóór de opgegeven marginale aanpassingen worden toegepast.

U kunt desgewenst een extra bruto-budget per dag, week of maand toevoegen:

1. Klik op **[!UICONTROL Add an additional Gross Budget]**.

1. Voer de **[!UICONTROL Gross Budget]** in en selecteer de budgetinterval: *[!UICONTROL Daily],* *[!UICONTROL Weekly],* of *[!UICONTROL Monthly]*.

De totale nettobegroting, de uitgavenlimiet voor de campagne, wordt automatisch berekend op basis van de marge-instellingen en wordt onder deze waarde aangegeven.

**[!UICONTROL Budget]:** (Campagnes zonder margebeheer) Het totale campagnebudget.

**[!UICONTROL Estimated Tax Withholding]:** Hiermee wordt een percentage van de totale uitgaven voor advertenties, honoreringskosten en/of gegevenskosten op rekeningniveau voor land- of lokale belastingen ingehouden. Tarieven zijn ramingen voor budgettering en prijsstelling, zodat de gefactureerde belastingtarieven kunnen variëren.

Belastingen die moeten worden ingehouden ramen:

1. Klik op **[!UICONTROL Update rates here]**.

1. Geef **[!UICONTROL Estimated tax rate]** op als een percentage.

1. Schakel het selectievakje in naast elk type kosten waarvoor belastingen moeten worden ingehouden. De vergoedingstypen omvatten:

   * *[!UICONTROL Include estimated tax - ads fee]:* Is van toepassing op alle media-uitgaven van Advertising Cloud DSP, inclusief belastingen op kosten voor campagnebeheer.

   * *[!UICONTROL Include estimated tax - ad serving fee]:* Is van toepassing op alle uitgaven aan Advertising Cloud DSP behalve media en gegevens. Belastingen voor kosten voor campagnebeheer zijn uitgesloten

   * *[!UICONTROL Include estimated tax - data fee]:* Is van toepassing op alle gegevensuitgaven voor Advertising Cloud DSP.

1. Klik op **[!UICONTROL Submit]**.

>[!NOTE]
>
>* In de V.S., kunnen de staten in hun opname van belastingtarieven tussen advertenties, het dienen van, en gegevens variëren. Voor organisaties in andere landen worden alle drie de categorieën belastingtarieven opgenomen om de BTW te vergoeden.
>
>* U kunt deze waarden ook configureren in de instellingen voor accountkosten.<!--[fee settings](/help/dsp/admin/tax-withholdings.md). -->


**[!UICONTROL Cross Device Level]:** (Alleen-lezen voor bestaande campagnes die sinds 22 juni 2020 zijn gemaakt; niet beschikbaar voor campagnes die vóór 22 juni 2020 zijn gemaakt) Het niveau waarop Advertising Cloud zich richt op advertenties en frequentieplafonds toepast:  *Hetzelfde* apparaat om een apparaat te activeren of  ** Personen om een persoon aan te wijzen voor al hun bekende apparaten.

**[!UICONTROL Device Graph]:** (Alleen-lezen voor bestaande campagnes; campagnes met alleen op personen gebaseerde cross-device gerichte doelgroepen) De apparaatgrafiek die moet worden gebruikt voor apparaatgerichte toepassingen en frequentiebeheer:

* *[!UICONTROL LiveRamp - U.S. only]:* Beschikbaar aan alle adverteerders voor dwars-apparaat richtend bij $0.35 CPM voor beelden die door de  [!DNL LiveRamp] apparatengrafiek (namelijk voor apparaten worden geleverd die niet binnen de gerichte publiekssegmenten worden gevonden) worden geleverd. U kunt een apparaatmarkering instellen op plaatsingsniveau.

   Deze optie is ook beschikbaar voor alle adverteerders, zonder vergoedingen, voor frequentiebeheer en attributiemeting.

* *[!UICONTROL Adobe Co-op U.S. and Canada only]:* Alleen beschikbaar voor Adobe Experience Cloud- [!DNL Device Co-op] deelnemers zonder extra kosten.

>[!TIP]
>
>Als de adverteerder ook apparaatattributie gebruikt, kunt u het beste dezelfde instellingen voor apparaatgrafieken gebruiken voor doelversie en frequentiebeheer als die welke zijn opgegeven in de instellingen voor apparaatattributie van de adverteerder. Als u voor deze campagne een andere apparaatgrafiek selecteert, kunnen er verschillen tussen de apparaten worden gemeld.

**[!UICONTROL Frequency Cap]:** (Optioneel) Het aantal keren dat een uniek apparaat of een unieke persoon (afhankelijk van het opgegeven apparaat of de opgegeven persoon  [!UICONTROL Cross Device Level]) advertenties van de campagne ontvangt. U kunt onder andere *[!UICONTROL Unlimited]* of een specifiek bedrag per dag, week of maand opgeven.

>[!NOTE]
>
> U kunt frequentiecappen instellen op campagne-, pakket- en plaatsingsniveaus. DSP zal de strengste frequentiegrens in de campagnehiërarchie respecteren.

**[!UICONTROL Packages]:** De pakketten  [](/help/dsp/campaign-management/packages/package-about.md) die in de campagne moeten worden opgenomen. Selecteer bestaande pakketten en/of maak pakketten die u wilt opnemen. Als u pakketten maakt, raadpleegt u beschrijvingen over de [pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md) voor meer informatie.

## [!UICONTROL Campaign Measurement]

>[!NOTE]
>
>Met de volgende instellingen worden alleen meet- en rapportagemogelijkheden ingeschakeld. Prestaties worden alleen geoptimaliseerd op pakket- en plaatsingsniveau.

### [!UICONTROL 3rd Party Metrics]

#### [!UICONTROL Viewability, Fraud, & Brand Safety]

**[!UICONTROL IAS]:** (Optioneel) Hiermee kunt u met de opgegeven instellingen de zichtbaarheid, fraude, merkveiligheid en verificatie van het publiek  [!DNL IAS] meten en rapporteren. Er zijn extra kosten van toepassing.

* **[!UICONTROL Measure On]:** De inventaris waarop wordt gemeten:  *[!UICONTROL Display and VPAID video inventory]* (de standaardwaarde) of  *[!UICONTROL Display, VPAID & VAST video inventory]*.

   >[!NOTE]
   >
   >De videoviewability is meetbaar op VPAID slechts inventaris.

* **[!UICONTROL IAS Account ID (AnID)]:** (Adverteerders met eigen  [!DNL IAS] boekhouding; (optioneel) De  [!DNL IAS] account-id van de organisatie, die rechtstreeks  [!DNL IAS] wordt gefactureerd voor gebruik.

* **[!UICONTROL IAS Team ID]:** (Adverteerders met eigen  [!DNL IAS] boekhouding; (optioneel) De team-id voor de  [!DNL IAS] account van de organisatie, die rechtstreeks  [!DNL IAS] wordt gefactureerd voor gebruik.  <!-- verify -->

**[!UICONTROL MOAT]:** (Optioneel) Hiermee kunt u de  [!DNL MOAT] zichtbaarheid, fraude, merkveiligheid en verificatie van het publiek meten en melden. Er zijn extra kosten van toepassing.

#### Verificatie door het publiek

**[!UICONTROL Nielsen]:** (Optioneel) Hiermee schakelt u  [!DNL Nielsen] meting en rapportage van publieksverificatie in met de opgegeven instellingen. Er zijn extra kosten van toepassing.

* **[!UICONTROL Target Gender]:** Het geslacht dat als doel moet worden genomen:  *[!UICONTROL Both]* (de standaardwaarde),  *[!UICONTROL Male]* of  *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** Het leeftijdsbereik dat moet worden gebruikt. Gebruik de linker- en rechterschuifregelaars om het bereik zo nodig te verkleinen.

* **[!UICONTROL Target Country]:** (Optioneel) Een land dat als doel moet worden ingesteld. [!DNL Nielsen] zullen alleen de indrukken meten die in de gesteunde landen worden bediend.

**[!UICONTROL comScore vCE]:** (Optioneel) Hiermee schakelt u  [!DNL Comscore validated Campaign Essentials (vCE)] meting en rapportage van publieksverificatie in met de opgegeven instellingen. Er zijn extra kosten van toepassing.

* **[!UICONTROL Target Gender]:** Het geslacht dat als doel moet worden genomen:  *[!UICONTROL Both]* (de standaardwaarde),  *[!UICONTROL Male]* of  *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** Het leeftijdsbereik dat moet worden gebruikt. Gebruik de linker- en rechterschuifregelaars om het bereik zo nodig te verkleinen.

* **[!UICONTROL Target Country]:** (Optioneel) Een land dat als doel moet worden ingesteld. [!DNL Comscore] zullen alleen de indrukken meten die in de gesteunde landen worden bediend.

### [!UICONTROL 1st Party Metrics]

**[!UICONTROL Viewability sensitivity]:** Laat eerste-partijmeting en rapportering van viewability toe gebruikend de  [!DNL IAB Open Video Viewability (OpenVV)] technologie, die op het gespecificeerde gevoeligheidsniveau wordt gebaseerd:

* *[!UICONTROL Standard (50% of ad in view for two consecutive seconds)]*

* *[!UICONTROL Strict (100% of ad in view and audio on for 50% duration)]*

>[!MORELIKETHIS]
>
>* [Informatie over Campagnebeheer](campaign-about.md)
>* [Een campagne maken](campaign-create.md)
>* [Een campagne bewerken](campaign-edit.md)

