---
title: Gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud verwacht
description: Gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud verwacht
feature: Integration with Adobe Analytics
exl-id: 34685e04-d4f9-4e27-b83e-b56164244b2b
source-git-commit: 185fc7d79798a0a3a9ad5829b701aeb53a4a47c1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Verwachte gegevensvariaties tussen [!DNL Analytics] en Advertising Cloud

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Adverteerders met de [!DNL Analytics for Advertising Cloud] <!-- (A4AdC) -->-integratie volgen betaalde reclame via Advertising Cloud en Adobe Analytics. Wanneer u media, campagnes en kanalen bijhoudt via meerdere systemen, komen dezelfde gegevenssets van verschillende systemen zelden volledig overeen. In dit document wordt uitgelegd hoe u gegevens voor media die door Advertising Cloud worden verhandeld, moet vergelijken met gegevens in de verschillende systemen waarin de media worden bijgehouden binnen [!DNL Analytics].

>[!NOTE]
>
>Dit document is gericht op Advertising Cloud en Analytics, maar veel van de belangrijkste punten zijn ook overdraagbaar naar andere volgoplossingen.

## Attribuutverschillen in vergelijkbare rapporten

### Potentieel Verschillende LookbackVensters en Modellen van de Attributie

De integratie [!DNL Analytics for Advertising Cloud] gebruikt twee variabelen (eVars of rVars \[gereserveerde eVars]\) om [EF ID en AMO ID](ids.md) te vangen. Deze variabelen worden gevormd met één enkel raadplegingsvenster (de tijd waarbinnen klik-productie en mening-productie worden toegeschreven) en een attributiemodel. Tenzij anders gespecificeerd, worden de variabelen gevormd om het gebrek, adverteerder-vlakke klik raadplegingsvenster en attributiemodel in Advertising Cloud aan te passen.

Nochtans, zijn de raadplegingsvensters en attributiemodellen configureerbaar in zowel Analytics (via eVars) als in Advertising Cloud. In Advertising Cloud is het toewijzingsmodel bovendien niet alleen op adverteerderniveau (voor optimalisatie van biedingen), maar ook binnen afzonderlijke gegevensweergaven en -rapporten (alleen voor rapportagedoeleinden) configureerbaar. Een organisatie gebruikt bijvoorbeeld liever het toewijzingsmodel voor gelijkmatige verdeling voor optimalisatie, maar gebruikt de laatste aanraakkenmerk voor rapporten in Advertising Cloud DSP of [!DNL Search]. Als u toewijzingsmodellen wijzigt, wordt het aantal toegewezen conversies gewijzigd.

Als een terugkijkvenster of attributenmodel van het rapport in één product en niet in andere wordt gewijzigd, dan zullen de zelfde rapporten van elk systeem verschillende gegevens tonen:

* **Voorbeeld van verschillen die worden veroorzaakt door verschillende terugkijkvensters:**

   Stel dat Advertising Cloud een terugkijkvenster van 60 dagen heeft en [!DNL Analytics] een terugkijkvenster van 30 dagen heeft. En stel dat een gebruiker naar de site komt via een door Advertising Cloud bijgehouden advertentie, bladeren, en vervolgens terugkeert op dag 45 en converteert. Advertising Cloud zal de omzetting aan het aanvankelijke bezoek wegens de omzetting binnen het 60 dagraadplegingsvenster toeschrijven. [!DNL Analytics], nochtans, kan niet de omzetting aan het aanvankelijke bezoek toeschrijven omdat de omzetting voorkwam nadat het terugkijkvenster van 30 dagen was verlopen. In dit voorbeeld rapporteert Advertising Cloud een hoger aantal conversies dan [!DNL Analytics].

   ![Voorbeeld van een conversie die in Advertising Cloud wordt toegewezen, maar niet  [!DNL Analytics]](/help/integrations/assets/a4adc-lookback-example.png)

* **Voorbeeld van discrepanties veroorzaakt door verschillende attributiemodellen:**

   Stel dat een gebruiker drie verschillende Advertising Cloud-advertenties gebruikt voordat deze worden geconverteerd, met inkomsten als het conversietype. Als in een Advertising Cloud-rapport een gelijkmatig distributiemodel wordt gebruikt voor toewijzing, worden de inkomsten gelijkmatig over alle advertenties verdeeld. Als [!DNL Analytics] echter het laatste aanraakattributiemodel gebruikt, worden de opbrengsten aan de laatste advertentie toegewezen. In het volgende voorbeeld kent Advertising Cloud zelfs 10 USD van de 30 USD aan inkomsten toe die aan elk van de drie advertenties worden opgenomen, terwijl [!DNL Analytics] alle 30 USD aan inkomsten toewijst aan de laatste advertentie die de gebruiker heeft gezien. Wanneer u rapporten van Advertising Cloud en [!DNL Analytics] vergelijkt, kunt u het effect van het verschil in attributie verwachten te zien.

   ![Verschillende opbrengsten die aan Advertising Cloud worden toegerekend en  [!DNL Analytics] op verschillende toerekeningsmodellen zijn gebaseerd](/help/integrations/assets/a4adc-attribution-example.png)

>[!IMPORTANT]
>
>De beste praktijken moeten de zelfde raadplegingsvensters en attributiemodel in zowel Advertising Cloud als [!DNL Analytics] gebruiken. Werk zo nodig samen met uw Adobe-accountmanager om de huidige instellingen te identificeren en de configuraties synchroon te houden.

Deze zelfde concepten zijn op een andere gelijkaardige kanalen van toepassing die verschillende raadplegingsvensters of attributiemodellen gebruiken.

#### Verschillende Lookback Vensters voor het Volgen van mening-door {#impression-lookback}

In Advertising Cloud is de toewijzing gebaseerd op klikken en indrukken en kunt u verschillende terugzoekvensters configureren voor klikken en voor indrukken. In [!DNL Analytics], echter, is de attributie gebaseerd op klikproductie en mening-door, en u hebt niet de optie om verschillende attributievensters voor klikproductie en mening-door te plaatsen; het volgen voor elk begint bij het eerste bezoek aan de site. Een indruk kan zich voordoen op dezelfde dag of meerdere dagen voordat een view-through plaatsvindt, en dit kan van invloed zijn op de plaats waar het toewijzingsvenster in elk systeem start.

Doorgaans vindt het merendeel van de doorkijkconversies snel genoeg plaats, zodat beide systemen krediet kunnen toewijzen. Sommige conversies kunnen echter plaatsvinden buiten het Advertising Cloud-imitatievenster, maar binnen het [!DNL Analytics]-terugzoekvenster; dergelijke omzettingen worden toegeschreven aan de doorkijkrichting in [!DNL Analytics], maar niet aan de indruk in Advertising Cloud.

In het volgende voorbeeld, veronderstel een bezoeker een advertentie op Dag 1 werd gediend, een mening-door bezoek uitvoerde (namelijk bezocht de de landende pagina van de advertentie zonder eerder de advertentie) op Dag 2, en op Dag 45 werd omgezet. In dit geval zou Advertising Cloud de gebruiker bijhouden vanaf dagen 1-14 (met een 14-daagse terugzoekactie), [!DNL Analytics] zou de gebruiker bijhouden vanaf dagen 2-61 (met een 60-daagse terugzoekactie) en de conversie op dag 45 zou worden toegeschreven aan de advertentie binnen [!DNL Analytics] maar niet binnen Advertising Cloud.

![Voorbeeld van een doorkijkconversie die in  [!DNL Analytics] maar niet in Advertising Cloud is toegewezen](/help/integrations/assets/a4adc-viewthrough-example.png)

Een andere oorzaak van discrepanties is dat, in Advertising Cloud, u mening-door omzettingen een douane *mening-door gewicht* kunt toewijzen die met betrekking tot het gewicht aan een op klik-gebaseerde omzetting wordt toegeschreven. Het standaardgewicht van de weergave-door is 40%. Dit betekent dat een doorkijkconversie wordt geteld als 40% van de waarde van een klikconversie. [!DNL Analytics] geen dergelijke weging van doorkijkomzettingen biedt. Zo, bijvoorbeeld, zal een 100 USD opbrengstorde die in [!DNL Analytics] wordt gevangen aan 40 USD in Advertising Cloud worden gedisconteerd als u het standaard mening-door gewicht gebruikt - een verschil van 60 USD.

Houd rekening met deze verschillen bij het vergelijken van doorkijkconversies tussen Advertising Cloud- en [!DNL Analytics]-rapporten.

#### Beschikbare kenmerken

| Advertising Cloud Attribution | [!DNL Analytics] Attributie | eVar/Var-toewijzing |
|--- |--- |--- |
| [!UICONTROL Last Event] | [!UICONTROL Last Touch] | [!UICONTROL Most Recent] |
| [!UICONTROL First Event] | [!UICONTROL First Touch] | [!UICONTROL Original Value] |
| [!UICONTROL Weight First Event More] | n.v.t. | n.v.t. |
| [!UICONTROL Even Distribution] | [!UICONTROL Linear] | [!UICONTROL Linear]<br><br>Niet gebruiken* |
| [!UICONTROL Weight Last Event More] | n.v.t. | n.v.t. |
| [!UICONTROL U-Shaped] | [!UICONTROL U-Shaped] | n.v.t. |
| n.v.t. | [!UICONTROL J-Shaped] | n.v.t. |
| n.v.t. | [!UICONTROL Inverse-J] | n.v.t. |
| n.v.t. | [!UICONTROL Custom] | n.v.t. |
| n.v.t. | [!UICONTROL Participation] | n.v.t. |
| n.v.t. | [!UICONTROL Algorithmic] | n.v.t. |

>[!NOTE]
>
>Voor lineaire toewijzing, [!DNL Analytics] attributen succesgebeurtenissen gelijkelijk over alle waarden van eVar binnen één enkel bezoek, zo gebruik lineaire toewijzing met een eVar van &quot;Bezoek.&quot; Voor reclame leidt het gebruik van lineaire toewijzing echter tot een niet echt lineaire toewijzing en tot minder dan ideale rapportage. Als een bezoeker bijvoorbeeld met drie advertenties communiceert voordat hij of zij in drie afzonderlijke bezoeken gaat omwisselen, wordt alleen de advertentie die tijdens het laatste bezoek werd getoond aan de conversie toegeschreven, niet aan alle drie advertenties.
>
>Bovendien voorkomt het schakelen van conversie naar of van &quot;Lineair&quot; dat historische gegevens worden weergegeven, wat kan leiden tot onjuiste gegevens in rapporten. Zo kan lineaire toewijzing inkomsten verdelen over een aantal verschillende eVar. Als u de toewijzing wijzigt in &quot;Recentste&quot;, wordt 100% van die inkomsten gekoppeld aan de meest recente enkele waarde. Deze koppeling kan tot onjuiste conclusies leiden.
>
>Om verwarring te voorkomen maakt [!DNL Analytics] historische gegevens niet beschikbaar in de rapportinterface. U kunt de historische gegevens bekijken als u de eVar terug naar het aanvankelijke plaatsen van de toewijzing verandert, hoewel u geen montages van de eVar toewijzing eenvoudig om tot historische gegevens toegang te hebben zou moeten veranderen. Adobe raadt u aan een nieuwe eVar te gebruiken wanneer u een nieuwe toewijzingsinstelling wilt toepassen voor gegevens die al worden vastgelegd, in plaats van toewijzingsinstellingen te wijzigen voor een eVar die al een aanzienlijke hoeveelheid historische gegevens bevat.

Zie een lijst van [!DNL Analytics] attributiemodellen en hun definities op [https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/models.html](https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/models.html).

Als u bent aangemeld bij Advertising Cloud, kunt u een lijst met toewijzingsmodellen vinden op
[https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm](https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm).

#### Attributie van gebeurtenisdatum in Advertising Cloud

In Advertising Cloud kunt u conversiegegevens rapporteren op basis van de bijbehorende klikdatum/gebeurtenisdatum (de datum van de klik- of impliciete gebeurtenis) of op basis van de transactiedatum (de conversiedatum). Het concept van click/gebeurtenisdatumrapportage bestaat niet in [!DNL Analytics]; alle in [!DNL Analytics] bijgehouden omzettingen worden per transactiedatum gerapporteerd. Dientengevolge, kan de zelfde omzetting met verschillende data in Advertising Cloud en [!DNL Analytics] worden gerapporteerd. Neem bijvoorbeeld een gebruiker die op 1 januari op een advertentie klikt en deze op 5 januari omzet. Als u de conversiegegevens weergeeft op de datum van de gebeurtenis in Advertising Cloud, wordt de conversie gerapporteerd op 1 januari, wanneer de klik plaatsvond. In [!DNL Analytics] zou dezelfde conversie op 5 januari worden gerapporteerd.

![Voorbeeld van een conversie die aan verschillende datums wordt toegeschreven](/help/integrations/assets/a4adc-conversions-based-on.png)

## Attributie in [!DNL Analytics Marketing Channels]

[[!DNL Analytics Marketing Channels] Met ](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/marketing-channels-admin.html) rapportering kunt u regels configureren om verschillende marketingkanalen te identificeren op basis van verschillende aspecten van raakinformatie. U kunt door Advertising Cloud bijgehouden kanalen ([!UICONTROL Display Click Through], [!UICONTROL Display View Through], en [!UICONTROL Paid Search]) als [!DNL Marketing Channels] volgen door de `ef_id` parameter van het vraagkoord te gebruiken om het kanaal te identificeren. <!-- Move most of the above text to "Marketing Channels" chapter once it's created, and add link here. --> Hoewel in de  [!DNL Marketing Channels] rapporten Advertising Cloud-kanalen kunnen worden getraceerd, komen de gegevens om verschillende redenen mogelijk niet overeen met de Advertising Cloud-rapporten. Zie de volgende secties voor meer informatie.

>[!NOTE]
>
> De volgende kernconcepten zijn ook van toepassing op elke multikanaaltracering waarbij campagnes betrokken zijn die niet in Advertising Cloud worden bijgehouden, zoals de variabele [`campaign`](https://experienceleague.adobe.com/docs/analytics/implementation/vars/page-vars/campaign.html) (ook wel de Dimension &quot;Trackingcode&quot; of &quot;eVar 0&quot; genoemd) en aangepaste eVar-tracking.

### Mogelijke verschillen in attributiemodellen in [!DNL Marketing Channels]

De meeste [!DNL Marketing Channels] rapporten worden gevormd met [!UICONTROL Last Touch] attributie, waarvoor het laatste ontdekte marketing kanaal 100% van de omzettingswaarde wordt toegewezen. Het gebruik van verschillende toewijzingsmodellen voor de [!DNL Marketing Channels]-rapporten en Advertising Cloud-rapporten zal leiden tot discrepanties in toegeschreven conversies.

### Een potentieel verschillend Lookback Venster in [!DNL Marketing Channels]

Het terugzoekvenster voor [!DNL Marketing Channels] kan worden aangepast. In Advertising Cloud, is het venster van de klikraadpleging configureerbaar, hoewel een vast venster van 60 dagen gemeenschappelijk is. Als de twee producten verschillende raadplegingsvensters gebruiken, kunt u gegevensdiscrepanties verwachten.

### Verschillende kanaalkenmerken in [!DNL Marketing Channels]

Advertising Cloud rapporteert alleen betaalde media die via Advertising Cloud worden verhandeld (betaalde zoekopdracht naar Advertising Cloud Search-advertenties en weergave voor Advertising Cloud DSP-advertenties), terwijl [!DNL Marketing Channels]-rapporten alle digitale kanalen kunnen traceren. Dit kan tot een discrepantie in het kanaal leiden waarvoor een omzetting wordt toegeschreven.

Betaalde zoekopdrachten en natuurlijke zoekkanalen hebben bijvoorbeeld vaak een symbiotische relatie, waarbij elk kanaal het andere kanaal helpt. Het [!DNL Marketing Channels] rapport zal sommige omzettingen aan natuurlijk onderzoek toeschrijven dat Advertising Cloud niet zal omdat het geen natuurlijk onderzoek volgt.

Neem bijvoorbeeld ook een klant die een advertentie weergeeft, op een betaalde zoekadvertentie klikt, in een e-mailbericht klikt en vervolgens een bestelling van 30 USD plaatst. Zelfs als Advertising Cloud en [!DNL Marketing Channels] beide het laatste aanraakattributiemodel gebruiken, wordt de conversie nog steeds anders toegewezen aan beide. Advertising Cloud heeft geen toegang tot het kanaal [!UICONTROL Email], zodat zou het betaalde onderzoek naar de omzetting crediteren. [!DNL Marketing Channels]De drie kanalen zijn echter toegankelijk, zodat de conversie  [!UICONTROL Email] voor haar rekening komt.

![Voorbeeld van verschillende conversietoewijzing in Advertising Cloud versus  [!DNL Analytics Marketing Channels]](/help/integrations/assets/a4adc-channel-example.png)

Voor meer uitleg over waarom de metriek kan variëren, zie &quot;[Waarom de Gegevens van het Kanaal tussen Advertising Cloud en [!DNL Marketing Channels]](marketing-channels/mc-data-variances.md) kunnen variëren.&quot;

## Gegevensverschillen in Adobe Analytics [!DNL Paid Search Detection]

Met de functie [legacy [!DNL Paid Search Detection]](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/paid-search-detection.html) in [!DNL Analytics] kunnen bedrijven [regels definiëren om betaald en organisch zoekverkeer](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/t-paid-search-detection.html) voor opgegeven zoekmachines te volgen. De [!DNL Paid Search Detection] regels gebruiken zowel een vraagkoord als het verwijzende domein om betaald en natuurlijk onderzoeksverkeer te identificeren. De [!DNL Paid Search Detection] rapporten maken deel uit van de grotere groep van [Het vinden Methoden](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/finding-methods.html) rapporten, die of verlopen wanneer een gespecificeerde gebeurtenis (zoals een Controle van de Kar) voorkomt of het bezoek beëindigt.

Het volgende is de interface voor het creëren van een [!DNL Paid Search Detection] regelreeks:

![Voorbeeld van een regel voor Paid Search-detectie die is ingesteld in  [!DNL Analytics]](/help/integrations/assets/a4adc-paid-search-detection.png)

De resulterende [!DNL Paid Search Detection] rapporten omvatten [!UICONTROL Paid Search Engine], [!UICONTROL Paid Search Keywords], [!UICONTROL Natural Search Engine], en [!UICONTROL Natural Search Keywords] rapporten.

Houd rekening met de volgende twee beperkingen met gegevens in [!DNL Paid Search Detection]-rapporten:

* De [!UICONTROL Paid Search Keywords] en [!UICONTROL Natural Search Keywords] rapporten tonen de onderzoeksvragen zoals die door verwijzende URLs worden geïdentificeerd, niet de sleutelwoorden waarop de gebruikers bieden. In Advertising Cloud- en [!DNL Analytics]-rapporten worden de werkelijke trefwoorden weergegeven. Verwacht dus niet dat deze worden uitgelijnd met de trefwoordrapporten [!DNL Paid Search Detection].

* Toen de functie [!DNL Paid Search Detection] oorspronkelijk werd gemaakt, was de voortkomende zoekquery (de tekenreeks met tekens die de gebruiker in de zoekbalk in het zoekprogramma heeft ingevoerd) gemakkelijker beschikbaar voor adverteerders via de verwijzende URL. Vandaag, verduisteren de onderzoeksmotoren grotendeels de onderzoeksvraag, en de [!DNL Paid Search Detection] sleutelwoordrapporten zijn van beperkte waarde omdat de meeste vraaggegevens onder &quot;unspecified&quot; vallen.

   Met [!DNL Analytics for Advertising Cloud] kunnen adverteerders betaalde trefwoorden nog steeds bijhouden in [!DNL Analytics]. Het verwijzende domein informeert de motorrapporten die de onderzoeksmotor het verkeer drijven. Aangezien de accountgegevens die specifiek zijn voor de adverteerder niet aan het verwijzende domein zijn gekoppeld, wordt al het verkeer weergegeven onder de zoekfunctie. Adverteerders met meerdere accounts in hetzelfde zoekprogramma moeten naar Advertising Cloud of [!DNL Analytics] voor accountspecifieke rapportage verwijzen.

### Waarom [!DNL Paid Search Detection] configureren?

Met de [!DNL Paid Search Detection]-rapporten kunt u natuurlijk zoekverkeer in de [[!DNL Analytics Marketing Channels] rapporten](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/marketing-channels-admin.html) identificeren. Het scheiden van betaald onderzoeksverkeer tegenover natuurlijk onderzoeksverkeer is een grote manier om de waarde te begrijpen die de natuurlijke opsporing aan het volledige marketing ecosysteem brengt.

## Doorklikgegevensvalidatie voor [!DNL Analytics for Advertising Cloud] {#data-validation}

Voor uw integratie moet u uw doorklikgegevens valideren om ervoor te zorgen dat alle pagina&#39;s op uw site de doorklikbewerkingen correct bijhouden.

In [!DNL Analytics], één van de gemakkelijkste manieren om [!DNL Analytics for Advertising Cloud] het volgen te bevestigen is kliks aan instanties te vergelijken gebruikend de &quot;Klikken aan Instanties van AMO ID&quot;berekende metrisch, die als volgt wordt berekend:

```Clicks to AMO ID Instances = (AMO ID Instances / AMO Clicks)```

[!UICONTROL AMO ID Instances] geeft het aantal keren weer dat AMO-id&#39;s (`s_kwcid` parameters) op de site worden bijgehouden. Elke keer dat op een advertentie wordt geklikt, wordt een parameter `s_kwcid` toegevoegd aan de URL van de bestemmingspagina. Het aantal [!UICONTROL AMO ID Instances] is daarom gelijk aan het aantal klikken en kan worden gevalideerd tegen werkelijke en klikbewerkingen. Doorgaans ziet u een 80% overeenkomende frequentie voor [!DNL Search] en een 30% overeenkomende frequentie voor [!DNL DSP]-verkeer (wanneer gefilterd om alleen doorklikken [!UICONTROL AMO ID Instances] op te nemen). Het verschil in verwachtingen tussen onderzoek en vertoning kan door het verwachte verkeersgedrag worden verklaard. Zoekopdracht legt de intentie vast en daarom zijn gebruikers gewoonlijk van plan om op de zoekresultaten van hun zoekopdracht te klikken. Gebruikers die een weergave- of onlinevideo zien, zullen echter vaker onbedoeld op de advertentie klikken en dan van de site naar de site stuiteren of het nieuwe venster dat wordt geladen verlaten voordat de paginageactiviteit wordt bijgehouden.

In Advertising Cloud rapporten, kunt u klikken aan instanties op een vergelijkbare manier vergelijken gebruikend &quot;[!UICONTROL ef_id_instances]&quot;metrisch in plaats van [!UICONTROL AMO ID Instances]:

```Clicks to [!UICONTROL EF ID Instances] = (ef_id_instances / Clicks)```

Zorg dat u een hoge equivalentieverhouding verwacht tussen de AMO-id en de EF-id, maar verwacht geen gelijke waarde van 100%, omdat AMO-id en EF-id fundamenteel verschillende gegevens bijhouden en dit verschil kan leiden tot kleine verschillen in het totaal [!UICONTROL AMO ID Instances] en [!UICONTROL EF ID Instances]. Als het totaal [!UICONTROL AMO ID Instances] in [!DNL Analytics] in Advertising Cloud meer dan 1% verschilt van [!UICONTROL EF ID Instances], neemt u contact op met uw Adobe-accountmanager voor hulp.

Voor meer informatie over AMO ID en EF identiteitskaart, zie [Advertising Cloud IDs die door Analytics](ids.md) wordt gebruikt.

Hieronder ziet u een voorbeeld van een werkruimte waarin u kliks naar instanties kunt bijhouden.

![Voorbeeld van een werkruimte om kliks naar instanties bij te houden](/help/integrations/assets/a4adc-clicks-to-instances-example.png)

## Gegevenssets vergelijken in [!DNL Analytics for Advertising Cloud] versus in Advertising Cloud

De [AMO-id](ids.md) (s_kwcid query string parameter) wordt gebruikt voor rapportage in [!DNL Analytics], en de [EF ID](ids.md) wordt gebruikt voor rapportage in Advertising Cloud. Omdat het verschillende waarden zijn, is het mogelijk dat één waarde is beschadigd of niet aan de landingspagina is toegevoegd.

Stel dat we de volgende bestemmingspagina hebben:

`www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id`

waarbij de EF-id &quot;`test_ef_id`&quot; is en de AMO-id &quot;`test_amo_id`&quot;.

Als een omleiding van de site plaatsvindt, kan de URL er als volgt uitzien:

`www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id#redirectAnchorTag`

waarbij de EF-id &quot;`test_ef_id`&quot; is en de AMO-id &quot;`test_amo_id#redirectAnchorTag`&quot;.

In dit voorbeeld worden door het toevoegen van de ankertag onverwachte tekens aan de AMO-id toegevoegd. Dit leidt tot een waarde die Analytics niet herkent. Deze AMO-id zou niet worden geclassificeerd en conversies die eraan zijn gekoppeld, vallen onder &quot;[!UICONTROL unspecified]&quot; of &quot;[!UICONTROL none]&quot; in [!DNL Analytics]-rapporten.

Gelukkig, terwijl de kwesties als dit gemeenschappelijk zijn, resulteren zij typisch niet in een hoog percentage van discrepantie. Als u echter een grote discrepantie tussen AMO-id&#39;s in [!DNL Analytics] en EF-id&#39;s in Advertising Cloud opmerkt, neemt u contact op met uw Adobe-accountmanager voor hulp.

## Andere metrische overwegingen

### Het verschil tussen klikken en bezoeken {#clicks-vs-visits}

Ze lijken op elkaar, maar klikken en bezoeken geven verschillende gegevens weer:

* **Klik:** [!DNL DSP] of de zoekmachine registreert een klik wanneer een bezoeker op een advertentie op de website van een uitgever klikt.

* **Bezoek:** [!DNL Analytics] definieert een  [](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html) bezoeker als een reeks paginaweergaven door een gebruiker, die eindigt volgens een van de verschillende criteria, zoals 30 minuten inactiviteit.

Een klik kan per definitie leiden tot meerdere bezoeken.

Bekijk het volgende voorbeeld: Gebruikers 1 en 2 openen beide een site door op een Advertising Cloud-advertentie te klikken. Gebruiker 1 geeft vier pagina&#39;s weer en verlaat vervolgens de dag, zodat de eerste klik resulteert in één bezoek. Gebruiker 2 geeft twee pagina&#39;s weer, verlaat voor een lunch van 45 minuten, keert terug, bekijkt nog twee pagina&#39;s, en verlaat dan; in dit geval leidt de eerste klik tot twee bezoeken .

![Voorbeeld van het verschil tussen klikken en bezoeken](/help/integrations/assets/a4adc-visits-example.png)

### Het verschil tussen klikken en klik-door

<!-- Rob to let me know if we should remove this and add more info. to the section on AMO Instances etc. -->

Klik en klik-door zijn twee verschillende metriek:

* **Klik:** [!DNL DSP] of de zoekmachine registreert een klik wanneer een bezoeker op een advertentie op de website van een uitgever klikt.

* **Klik-door:** [!DNL Analytics] registreert een klikdoor wanneer de bezoeker op de bestemmingswebsite, de het landen pagina laadt, en het  [!DNL Analytics] verzoek bij de bodem van de pagina verzendt de gegevens naar  [!DNL Analytics].

Klikken en doorklikken kunnen sterk verschillen als gevolg van een ongeluk en klikken. We hebben gezien dat de meeste klikken op weergaveadvertenties per ongeluk gebeuren. Deze bezoekers raakten op de knop Terug voordat de landingspagina wordt geladen, zodat [!DNL Analytics] geen doorklikken kan opnemen. Dit geldt met name voor advertenties waarin een onbedoelde klik waarschijnlijker is, zoals mobiele advertenties, videobanden en advertenties die het scherm vullen en moeten worden gesloten voordat de gebruiker de pagina kan bekijken.

Sites die op mobiele apparaten worden geladen, zullen ook minder vaak een doorklik tot gevolg hebben vanwege een lagere bandbreedte of een lagere verwerkingscapaciteit, waardoor het langer duurt om bestemmingspagina&#39;s te laden. Het is niet ongebruikelijk voor 50-70% van kliks om niet in klikproductie te resulteren. In mobiele omgevingen kan het verschil oplopen tot 90% vanwege de combinatie van een langzamere browser en de hogere kans dat de gebruiker per ongeluk op de advertentie klikt terwijl de pagina wordt doorgeschoven of de advertentie wordt gesloten.

De klikgegevens kunnen ook worden geregistreerd in milieu&#39;s die klikdoorgangen met de huidige volgende mechanismen (zoals kliks die naar, of van, een mobiele app gaan) niet kunnen registreren of waarvoor de adverteerder slechts één het volgen benadering (bijvoorbeeld, met mening-door JavaScript benadering, browsers die derdecookies blokkeren zal klikken volgen, maar niet kliks-door). Een belangrijke reden dat Adobe aanbeveelt om zowel de aanpak voor het bijhouden van klikken op URL&#39;s als de aanpak voor het bijhouden van JavaScript-weergaven te implementeren, is het maximaliseren van de dekking van doorklikbare doorklikbewerkingen.

### Advertising Cloud Traffic Metrics voor niet-Advertising Cloud-Dimension gebruiken

Advertising Cloud voorziet Analytics van [reclame-specifieke verkeersmetriek en de verwante dimensies van DSP en Onderzoek](advertising-cloud-metrics-in-analytics.md). De door Advertising Cloud verschafte meetgegevens zijn alleen van toepassing op de opgegeven Advertising Cloud-afmetingen en de gegevens zijn niet beschikbaar voor andere dimensies in [!DNL Analytics].

Bijvoorbeeld, als u [!UICONTROL AMO Clicks] en [!UICONTROL AMO Cost] metriek door Rekening bekijkt, die een dimensie van Advertising Cloud is, dan zult u het totaal [!UICONTROL AMO Clicks] en [!UICONTROL AMO Cost] door rekening zien.

![Voorbeeld van Advertising Cloud-meetgegevens in een rapport met een Advertising Cloud-dimensie](/help/integrations/assets/a4adc-traffic-supported-dimension.png)

Als u de [!UICONTROL AMO Clicks]- en [!UICONTROL AMO Cost]-cijfers echter weergeeft met een paginagrootte (zoals Pagina) waarvoor Advertising Cloud geen gegevens levert, zijn [!UICONTROL AMO Clicks] en [!UICONTROL AMO Cost] voor elke pagina nul (0).

![Voorbeeld van Advertising Cloud-meetgegevens in een rapport met een niet-ondersteunde dimensie](/help/integrations/assets/a4adc-traffic-unsupported-dimension.png)

### Het gebruiken van [!UICONTROL AMO ID Instances] als Vervangend voor Klikken met Dimension niet-Advertising Cloud

Aangezien u [!UICONTROL AMO Clicks] niet met onsite afmetingen kunt gebruiken, kunt u een equivalent aan klikken willen vinden. Mogelijk bent u geneigd Visit te gebruiken als een vervanging, maar dit is niet de beste optie, omdat elke bezoeker meerdere bezoeken kan hebben. (Zie &quot;[Het verschil tussen klikken en bezoeken](#clicks-vs-visits).&quot; In plaats daarvan raden we u aan [!UICONTROL AMO ID Instances] te gebruiken. Dit is het aantal keren dat de AMO-id wordt vastgelegd. Hoewel [!UICONTROL AMO ID Instances] [!UICONTROL AMO Clicks] precies niet zal aanpassen, zijn zij de beste optie om klikverkeer op de plaats te meten. Voor meer informatie, zie &quot;[de Bevestiging van Gegevens voor [!DNL Analytics for Advertising Cloud]](#data-validation).&quot;

![Voorbeeld van  [!UICONTROL AMO ID Instances] in plaats van  [!UICONTROL AMO Clicks] voor een niet-ondersteunde dimensie](/help/integrations/assets/a4adc-amo-id-instances.png)

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]](/help/integrations/analytics/ids.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
>* [[!DNL Analytics] Gegevens in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)
>* [Waarom gegevens kunnen verschillen tussen Advertising Cloud en [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-data-variances.md)

