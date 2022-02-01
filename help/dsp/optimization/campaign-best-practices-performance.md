---
title: Beste praktijken voor de Campagnes van Prestaties van de Opstelling
description: Leer beste praktijken voor het opzetten van uw prestaties-gerichte campagnes, die plaatsingen omvatten die voor laagste CPA of hoogste ROAS worden geoptimaliseerd.
feature: DSP Optimization, DSP Best Practices
exl-id: fc64680d-9d1c-4f74-a8b9-2e9b670c00eb
source-git-commit: b40c6f08b94e546e5fc068c46b279292a4d8a14f
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 0%

---

# Beste praktijken voor de Campagnes van Prestaties van de Opstelling

Advertising Cloud kan uw prestatiegerichte campagnes optimaliseren voor plaatsing met de laagste kosten per aankoop (CPA) of het hoogste rendement op advertentie (ROAS).

Raadpleeg de volgende aanbevolen procedures voor prestatiecampagnes:

* Stap 1 - Bepaal uw Doel
* Stap 2 - Definieer uw strategie
* Stap 3 - Pakketten maken
* Stap 4 - Plaatsingsstructuur maken
* Stap 5 - De juiste Creative Assets gebruiken

## Stap 1 - Bepaal uw doel

Het is belangrijk om te begrijpen of het doel van de campagne het hoogst mogelijke ROAS of het laagst mogelijke CPA is te bereiken. Voor elk pakket in de campagne, zult u het objectieve doel dienovereenkomstig als of specificeren *[!UICONTROL Highest ROAS - Custom Goal]* of *[!UICONTROL Lowest CPA - Custom Goal]*.

![optimalisatiedoel](/help/dsp/assets/optimization-goals.png)

U moet ook de succesgebeurtenis(sen) bepalen die tot het algemene doel zullen leiden en dienovereenkomstig douanedoelstellingen creëren. Voor elk pakket, zult u een douanedoel specificeren dat met het algemene optimalisatiedoel voor rapportering en algoritmische optimalisering moet worden gebruikt [!DNL Adobe Sensei]. Voor meer informatie over het creëren van douanedoelstellingen, zie [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md).

![aangepaste doelen](/help/dsp/assets/objective-goals.png)

## Stap 2 - Bepaal uw strategie

### Verkennende strategieën

Pakketten met bovengrondse treinen bevatten plaatsingen met een zeer brede doelgerichtheid om nieuwe consumenten te bereiken.

#### Aanbevolen plaatsingsstrategieën voor prospectie

* Zoek naar nieuwe soorten publiek die met de volgende tactieken kunnen worden omgezet:

   * Modellering van look-alike van een platform van het gegevensbeheer (DMP), zoals Adobe Audience Manager.
   * Gedragingen waarbij gegevens van derden worden gebruikt.
   * Contextafhankelijke doelframes.
   * Doellocatie/categorie.

* Het gebruik van looppas van netwerk (RON) richtend: Het is belangrijk om een looppas van netwerkplaatsing te omvatten zonder doelgericht publiek en met brede inventarisgericht. Hierdoor wordt de [!DNL Adobe Sensei] algoritme om waardevolle gebruikers te vinden die nieuwere cookies kunnen hebben die nog niet in een publiek zijn gecategoriseerd.

### Strategieën opnieuw rangschikken

Lagere treintpakketten bevatten plaatsingen die bedoeld zijn voor gebruikers die al op de webpagina van de adverteerder zijn geweest of voor wie de adverteerder CRM-gegevens heeft.

#### Aanbevolen plaatsingsstrategieën voor opnieuw toewijzen

* Als de adverteerder een Adobe Analytics- of Adobe Audience Manager-klant is, kunt u eerste-partijsegmenten (zoals bezoekers van de homepage, productpagina&#39;s of winkels voor winkelwagens) maken en deze gebruiken als plaatsingsdoelen in Advertising Cloud.

* Vermijd het toewijzen van te veel budget aan een doelgerichte plaatsing. Als algemene regel geldt dat budget $30 per 1.000 gebruikers per maand bedraagt.

## Stap 3 - Pakketten maken

De beste praktijk is het maken van afzonderlijke pakketten voor de prospectie van de bovenste trechter en voor de herbestemming van de ondertrechter. Optimalisatie vindt plaats op pakketniveau, zodat de prestatiegegevens van alle plaatsen binnen een pakket worden samengevoegd. Daarom groepeert plaatsing in pakketten met vergelijkbare verwachte prestaties.

![voorbeeld van afzonderlijke pakketten voor prospectie en heroriëntering](/help/dsp/assets/p-r.png)

Gebruik ook de volgende instellingen.

### Doelstellingen en budget

* **Tussenruimte en uitlijnen:** Als u een doel voor de optimalisatie van CPA of ROAS wilt selecteren, moet het pakket pakketniveau gebruiken. Dit zorgt ervoor dat alle plaatsen binnen het pakket worden geoptimaliseerd om uitgaven op basis van prestaties en schaal aan de geselecteerde doelstellingen te verdelen.

* **Vluchtdatums:** (Pakketten met vooruitzichten) Als uw campagne langer dan 25 dagen wordt uitgevoerd, kunt u de opdracht [!UICONTROL Activate Custom Flighting] gebruiken. Stel eerst een aangepaste vlucht voor de eerste 10 dagen in op ongeveer 75% van de dagelijkse begroting die nodig is om de uitgaven tijdens de *leerfase*. Stel vervolgens een tweede aangepaste vlucht in voor de rest van de begroting.

   Als u bijvoorbeeld $100.000 wilt besteden in 30 dagen, stelt u het budget voor vlucht 1 (dagen 1-10) in op $25.000 (75% x $100.000/30 dagen = $2.500 per dag). Gebruik het resterende budget van $75.000 voor Vlucht 2 (Dagen 11-30).

* **Begroting:** DSP zal altijd proberen om 100% van de pakketbegroting gelijkelijk over alle plaatsen in een pakket te verdelen. Als een baan weinig of geen uitgaven heeft, adviseren wij begroting die de plaatsing begrenzen om meer van het budget toe te wijzen aan stages met schaal. 24-48 uur toestaan voor begrotingswijzigingen.

* **Optimalisatiedoelstellingen:** Gebruik een van de twee optimalisatiedoelen voor prestaties. *[!UICONTROL Highest ROAS]* of *[!UICONTROL Lowest CPA]*, afhankelijk van het pakketdoel. Met deze doelen wordt het pakket automatisch geoptimaliseerd in de richting van respectievelijk de beste ROAS- of laagste CPA-plaatsing.

* **Aangepaste doelen:**
   * Als een nieuw pakket hetzelfde doel heeft als een bestaand pakket, kunt u optioneel het bestaande pakket koppelen, zodat het algoritme de bestaande leergegevens voor computers kan gebruiken.
   * Voer de juiste gegevens in [!UICONTROL Target CPA] of [!UICONTROL Target ROAS].

* **Vulstrategie voor spatiëring:** Selecteren *[!UICONTROL Even]* om uw prestatiedoelstellingen te maximaliseren door uniform door de volledige vluchtdatum te passen.

   Gebruiken *[!UICONTROL FrontLoad]* en *[!UICONTROL Aggressive Front Load]* het plaatsen slechts wanneer u volledig aan levering en besteedt over prestatiesoptimalisering omdat die strategieën negatief uw gewenste prestaties KPIs kunnen beïnvloeden.

## Stap 4 - Plaatsingsstructuur maken

Minder is meer. Als u minder dan zes plaatsen per pakket kunt instellen, dan kan het beschikbare budget dynamisch verschuiven naar de best presterende plaatsen het gemakkelijkst.

Zorg er ook voor dat u elke plaatsing aan een pakket toevoegt met het doeltype van het pakket *[!UICONTROL Prospecting]* of *[!UICONTROL Retargeting]* in voorkomend geval.

Hieronder vindt u de aanbevolen plaatsingsinstellingen voor prestatiecampagnes.

### Doelen

U zult CPA of ROAS optimalisering op het pakketniveau vormen (zie Stap 3 - creeer Pakketten), maar u kunt extra plaatsing-vlakke montages toevoegen.

* **Maximumbod:**
   * Gebruik een laag maximumbod ($5) voor het zoeken naar plaatsen.
   * Gebruik een hoog maximumbod ($12) als u plaatsingen opnieuw wilt toewijzen.

* **Filters vóór bod:** Minimaliseer of vermijd bij voorkeur het instellen van agressieve voorbiedingsfilters, die voorkomen dat de plaatsing schaalbaar wordt. De beste praktijken omvatten het volgende:

   * Gebruik één (1) voorbiedingsfilter per plaatsing. Voor meerdere filters voor vooraf bieden moet aan beide worden voldaan, waardoor de schaal afneemt.

   * U kunt minder strikte voorbiedingsfilters instellen in gevallen waarin extra doelframes (zoals publiek, geo en doellocatie) worden toegepast.

Zie de beschrijvingen van wanneer u elk vooraf biedfilter moet gebruiken op [Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken](/help/dsp/optimization/optimization-pre-bid-filters.md).

### Inventaris

Als u de schaal wilt maximaliseren, gebruikt u [!UICONTROL Public] (Open Exchange) en [!UICONTROL On Demand] voorraad.

### Sitedoelen

* **[!UICONTROL Traffic Type]**: [!UICONTROL Websites] alleen
* **[!UICONTROL Site Tier]**: [!UICONTROL All sites]

### Doelgerichtheid publiek

* **[!UICONTROL Included Audiences]:**
   * Voor prospectieve plaatsingen, groepeer gelijkaardige publiekscategorieën en gelijkaardige publieksgrootte in één plaatsing. Voer vervolgens op basis van prestaties een van de volgende handelingen uit:
      * Verwijder ondermaats presterende soorten publiek uit bestaande plaatsen.
      * Verplaats toppresterende doelgroepen naar een aparte plaatsing voor betere beheerbudgetten.
   * Voor het opnieuw plaatsen, zou u idealiter één publiekssegment per plaatsing moeten omvatten om biedingen en begroting gemakkelijk te controleren.

>[!NOTE]
>
>Uw advertenties presteren het best als een gebruiker slechts door één plaatsing kan worden bereikt. Een aanzienlijke overlapping van gebruikers tussen verschillende plaatsen kan concurrentie veroorzaken, wat een cyclus van voortdurend stijgende biedingen oplevert, waardoor de kosten per gebruiker stijgen. Daarom als u veelvoudige publiek omvat, zorg ervoor zij niet uit overlappende gebruikers/publieksleden bestaan.
>
> U kunt overlappende soorten publiek voorkomen door uw publiek in lagen te maken, zodat u de hogere, meer inclusieve lagen van plaatsingen desgewenst kunt onderdrukken.

* **[!UICONTROL Frequency Capping]:**
   * Gebruik voor prospectie van plaatsingen krappe frequenties (één indruk per dag).
   * Stel voor het opnieuw plaatsen de primaire plaatsingsdop in op 6-10 indrukkingen per dag en de secundaire dop op 1 indruk per uur.

* **[!UICONTROL Device Targeting]**:
   * Inclusief [!UICONTROL Computer], [!UICONTROL Mobile], en [!UICONTROL Tablet].
   * Niet instellen [!UICONTROL Firefox] en [!UICONTROL Safari] vanwege beperkingen inzake doelgerichtheid en meting. Neem contact op met uw [!DNL Adobe] accountteam voor meer informatie over [!DNL Adobe] steun voor [!DNL Safari ITP].
   * Als u mobiel webverkeer als doel instelt, schakelt u alle mobiele browsers uit, behalve [!UICONTROL Chrome] en [!UICONTROL Edge].

### Merk, veiligheid en mediakwaliteit

Contextafhankelijke filtering, blokkering van voorbiedingsfraude en/of [!UICONTROL Ads.txt] het filtreren zal de schaal van uw plaatsen beperken, maar gebruik hen indien nodig.

## Stap 5 - De juiste Creative Assets gebruiken

* De beste manier is om zoveel mogelijk unieke advertentiegrootten op te nemen om het bereik te maximaliseren. Met de universele weergavesjabloon kunt u elke standaardweergave en -grootte uploaden.
* Zorg ervoor dat alle plaatsen bevatten *ten minste* alle primaire schermen en formaten (300x250, 728x90, 160x600, 300x600, 320x50 en 300x50).
* Werk creatieve middelen regelmatig bij om creatieve vermoeidheid te voorkomen.

>[!MORELIKETHIS]
>
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
>* [Plaatsingsinstellingen](/help/dsp/campaign-management/placements/placement-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Filters op plaatsingsniveau vóór het bieden en hoe deze te gebruiken](optimization-pre-bid-filters.md)
>* [Controlelijst voor starten van campagne](/help/dsp/campaign-management/campaign-launch-checklist.md)

