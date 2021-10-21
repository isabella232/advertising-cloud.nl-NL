---
title: Instellingen voor aangepaste rapporten
description: Zie beschrijvingen van de montages van het douanerapport.
feature: DSP Custom Reports
source-git-commit: d2ad7d47d9cf13411fc831526a6fa4ff698b0a15
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---


# Instellingen voor aangepaste rapporten

**[!UICONTROL Name]** De rapportnaam. De maximumlengte is 180 tekens.

**[!UICONTROL Report Type]** Het type rapport: *[!UICONTROL Custom]* (met de meeste beschikbare opties), *[!UICONTROL Billing]*, *[!UICONTROL Conversion]*, *[!UICONTROL Device]*, *[!UICONTROL Frequency (by Impression)]*,  *[!UICONTROL Frequency (by App/Site)]*, *[!UICONTROL Geo]*, *[!UICONTROL Margin]*, *[!UICONTROL Media Performance]*,  *[!UICONTROL Segment]*, of *[!UICONTROL Site]*.

## [!UICONTROL Apply Filters] Sectie

**[!UICONTROL Timezone]:** De tijdzone voor rapportage.

**[!UICONTROL Observe Daylight Savings Time]:** Neemt zomertijd in de gerapporteerde tijden in acht.

**\[Datumbereik\]:** Het datumbereik waarvoor gegevens moeten worden gegenereerd. Het aantal beschikbare dagen varieert per rapport en per geselecteerde afmeting. Kies een optie:

* **[!UICONTROL Previous N days]:** Bevat gegevens voor een specifiek aantal dagen vóór vandaag.

* **[!UICONTROL Custom]:** Bevat gegevens tussen specifieke begin- en einddatums. Selecteer **[!UICONTROL Present]**.

* **[!UICONTROL Last Calendar Month]:** Bevat gegevens voor de vorige kalendermaand.

**[!UICONTROL Add Filters]:** (Optioneel) Aanvullende afmetingen waarmee de gegevens kunnen worden gefilterd, ongeacht of de afmetingen als kolommen in het rapport zijn opgenomen: *[!UICONTROL Account]*,\* *[!UICONTROL Advertiser]*, *[!UICONTROL Campaign]*, *[!UICONTROL Placement]*, *[!UICONTROL Ad]*, *[!UICONTROL Ad Type]*, *[!UICONTROL Video]*, *[!UICONTROL Video Duration]*, *[!UICONTROL Country]*, en *[!UICONTROL Package]*.

\* *[!UICONTROL Account]* is beschikbaar voor de volgende rapporttypes slechts wanneer uw organisatie voor wordt gevormd [cross-account rapportage](report-about.md#cross-account-reporting):  [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo], [!UICONTROL Device], [!UICONTROL Frequency (by Impression)], en [!UICONTROL Conversion]. Neem contact op met uw [!DNL Adobe] accountmanager voor meer informatie over de rapportage van kruisrekeningen.

Ga als volgt te werk om een of meer filters toe te passen:

* Selecteer een dimensie, selecteer de operator (*equals* of *niet gelijk aan*) en selecteert u vervolgens de toepasselijke waarde. Als u bijvoorbeeld alleen gegevens voor preroll-advertenties wilt retourneren, geeft u &quot;[!UICONTROL Ad Type equals Preroll].&quot;
* (Optioneel) Voeg aanvullende criteria toe aan het filter.
* (Optioneel) Voeg aanvullende filters toe, elk met een of meer criteria.

## [!UICONTROL Build Your Report] Sectie

**[!UICONTROL Select To Add As Report Headers]:**  De gegevenskolommen, of kopballen, om in het rapport te omvatten. Als u een kolom wilt toevoegen, vouwt u de categorie uit en schakelt u het selectievakje naast de kolomnaam in. Alle niet-beschikbare meetgegevens zijn uitgeschakeld. De beschikbare gegevenscategorieën zijn:

* [!UICONTROL  Dimensions]
* [!UICONTROL Metrics]
* [!UICONTROL Conversion Metrics] (gesorteerd op adverteerder)
* [!UICONTROL Custom Goals] (gesorteerd op adverteerder)

**[!UICONTROL Drag to Re-Order Report Headers Below]:** De volgorde van de kolomkoppen. U kunt elke kolom slepen en neerzetten om de volgorde aan te passen.

## [!UICONTROL Multi-Touch Conversion Options] Sectie

**[!UICONTROL Format]:** Of een rapport moet worden gegenereerd in *[!UICONTROL CSV]* (door komma&#39;s gescheiden waarden) of *[!UICONTROL Tab]* (door tabs gescheiden waarden).

**[!UICONTROL Report Headers]:** Of *[!UICONTROL Include]* of *[!UICONTROL Do Not Include]* kolomkoppen.

**[!UICONTROL Attribution Rule Settings]:** (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen; adverteerders met alleen het bijhouden van Advertising Cloud-conversies) In het rapport wordt uitgelegd hoe u conversiegegevens kunt toewijzen in een reeks gebeurtenissen die tot conversie leiden. U kunt meer dan één regel kiezen als u de verschillen tussen de regels wilt vergelijken.

>[!NOTE]
>
>Conversiepaden bevatten alle indrukken en klikken binnen de indruk van de adverteerder of klik op terugkijkvensters, die in Advertising Cloud Search zijn geconfigureerd. Klikken krijgen de voorkeur boven indrukken tijdens conversie-toewijzing. Om het even welke kliks in een omzettingsweg ontvangen volledige kredieten die op de attributieregel worden gebaseerd. Impressies krijgen alleen krediet als er geen klikken worden bijgehouden in het conversiepad.

* *[!UICONTROL Last Event]:* Hiermee worden conversies toegewezen aan de laatste klik of indruk in het conversiepad.

* *[!UICONTROL Weight Last More]:* Hiermee worden conversies toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgen de laatste gebeurtenis het meeste gewicht en wordt het gewicht van de voorgaande gebeurtenissen achtereenvolgens minder.

* *[!UICONTROL Even Distribution]:* Hiermee worden conversies gelijkmatig toegewezen aan elke gebeurtenis in het conversiepad.

* *[!UICONTROL Weight First More]:* Hiermee worden conversies toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgen de eerste gebeurtenis het meeste gewicht en wordt het gewicht van de volgende gebeurtenissen achtereenvolgens minder.

* *[!UICONTROL First Event]:* Hiermee worden conversies toegewezen aan de eerste klik of de eerste indruk in het conversiepad.

* *[!UICONTROL U-shaped]:* Hiermee wordt de conversie toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgt het grootste gewicht aan de eerste en laatste gebeurtenis, met achtereenvolgens minder gewicht aan de gebeurtenissen in het midden van het conversiepad.

* *[!UICONTROL Display Only]:*  Hiermee worden conversies toegewezen aan de laatste DSP klik of indruk in het conversiepad. Dit omvat video en aangesloten tv-advertenties en sluit kliks op Advertising Cloud Search-advertenties uit.

* *[!UICONTROL Social Only]:* Achterhaald

<!-- See also [How Attribution Rules Are Calculated for Adobe Advertising Cloud](). -->

**[!UICONTROL Paths as Columns]:**  (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen) Welke soorten omzettingen om te melden wanneer de vroegere gebeurtenissen op het zelfde apparaat voorkwamen. U kunt maximaal drie typen opnemen. Voor elk geselecteerd type wordt een aparte kolom opgenomen voor elke omzettingsmetrische waarde en toegevoegd met het opgegeven achtervoegsel ([!UICONTROL (tl)], [!UICONTROL (ct)], of [!UICONTROL (vt)]):

* *[!UICONTROL Total (TL) = CT + VT \* VT weight]:* Omvat omzettingen die aan kliks (CT voor kliks-door) en aan impressies (VT voor mening-door) worden toegeschreven. Conversies die worden toegewezen aan impressies worden vermenigvuldigd met het opgegeven doorkijkgewicht. Het standaardgezichtsdoorsgewicht is 100%, wat betekent dat omzettingen die aan indrukkingen worden toegeschreven, worden geteld als 100% van de waarde van omzettingen die aan kliks worden toegeschreven.

* *[!UICONTROL With Clicks (CT)]:* Omvat slechts omzettingen die aan kliks worden toegeschreven.

* *[!UICONTROL Impressions Only (VT)]:* Omvat slechts omzettingen die aan impressies werden toegeschreven omdat geen kliks in de omzettingsweg werden gevolgd.

**[!UICONTROL Cross Device Level]:**  (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen; alleen van toepassing op adverteerders met attributie &quot;cross-device&quot;) Het niveau waarop conversies moeten worden bijgehouden: *[!UICONTROL People]* of *[!UICONTROL Household]*.

Meer informatie over [oplossingen voor meerdere apparaten](/help/dsp/introduction/features/cross-device-solutions.md).

**[!UICONTROL Cross-Device Breakout]:** (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen; (alleen van toepassing op adverteerders met apparaatoverschrijdende attributie) Het detailniveau over apparaatoverschrijdende omzettingen dat in het rapport moet worden opgenomen. U kunt tot drie niveaus kiezen, elk waarvan in een afzonderlijke kolom zal worden omvat, als u een gedetailleerde doorbraak wilt.

* *[!UICONTROL Total People (TP)]:* Omvat de totale omzettingen, die zowel de omzettingen van het zelfde apparaat als de overschakeling van het dwars-apparaat omvatten (indien van toepassing). In het verslag[!UICONTROL (tp)]&quot; wordt toegevoegd aan de metrische naam en het regeltype van de omzetting.

* *[!UICONTROL Same Device (SD)]:* Omvat slechts omzettingen waarvoor slechts één enkel apparaat in de omzettingsweg werd gevolgd. In het verslag[!UICONTROL (sd)]&quot; wordt toegevoegd aan de metrische naam en het regeltype van de omzetting.

* *[!UICONTROL Cross Device (XD)]:* Omvat slechts omzettingen waarvoor meer dan één apparaat in de omzettingsweg werd gevolgd. In het verslag[!UICONTROL (xd)]&quot; wordt toegevoegd aan de metrische naam en het regeltype van de omzetting.

**[!UICONTROL Conversion Reporting Based On]:**  Conversiegegevens rapporteren:

* *[!UICONTROL Conversion Timestamp]:* (De standaardwaarde) Conversies worden gekoppeld aan de conversiedatum.

* *[!UICONTROL Event Timestamp]:* Conversies worden gerapporteerd op basis van de datum van de indruk of klik die de conversie heeft veroorzaakt, zoals bepaald door het opgegeven [!UICONTROL Attribution Rule Settings].

## [!UICONTROL Add Email Recipients] Sectie

**[!UICONTROL Email]:** E-mailadres(sen) waarnaar ingevulde rapporten of meldingen moeten worden verzonden als het rapport door fouten is geannuleerd. Als u meerdere adressen wilt opgeven, scheidt u deze met komma&#39;s of spaties.

**[!UICONTROL Frequency]:** Hoe vaak moet het rapport worden verzonden: *[!UICONTROL Once]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, of *[!UICONTROL Monthly]*.

## [!UICONTROL Save Report] Sectie

**[!UICONTROL Send & Save]:** Wanneer het rapport wordt verzonden: *[!UICONTROL On Schedule]* of *[!UICONTROL Run Now]*. Geplande rapporten zullen tegen 9:00 in de tijdzone van de rekening worden geleverd.

>[!NOTE]
>
>U kunt [een aangepast rapport op elk gewenst moment uitvoeren](report-run-now.md) van de [!UICONTROL Reports] weergeven.

>[!MORELIKETHIS]
>
>* [Aangepaste rapporten](/help/dsp/reports/report-about.md)
>* [Een aangepast rapport maken](/help/dsp/reports/report-create.md)
>* [Een aangepast rapport dupliceren](/help/dsp/reports/report-copy.md)
>* [Een aangepast rapport bewerken](/help/dsp/reports/report-edit.md)
>* [Een aangepast rapport uitvoeren](/help/dsp/reports/report-run-now.md)
>* [Instellingen voor aangepaste rapporten](/help/dsp/reports/report-settings.md)

* [Beschikbare rapportkolommen](/help/dsp/reports/report-columns.md)
