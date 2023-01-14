---
title: Instellingen voor aangepaste rapporten
description: Zie beschrijvingen van de montages van het douanerapport.
feature: DSP Custom Reports
exl-id: 1d37fc96-0f9b-4eb2-ba8d-9534f627adaf
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '966'
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

\* *[!UICONTROL Account]* is beschikbaar voor de volgende rapporttypes slechts wanneer uw organisatie voor wordt gevormd [cross-account rapportage](report-about.md#cross-account-reporting):  [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo], [!UICONTROL Device], [!UICONTROL Frequency (by Impression)], en [!UICONTROL Conversion]. Neem contact op met uw [!DNL Adobe] -accountteam voor meer informatie over cross-account rapportage.

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

**[!UICONTROL Attribution Rule Settings]:** (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen; adverteerders met alleen Adobe Advertising conversion tracking) In het rapport wordt uitgelegd hoe u conversiegegevens kunt toewijzen in een reeks gebeurtenissen die tot conversie leiden. U kunt meer dan één regel kiezen als u de verschillen tussen de regels wilt vergelijken.

>[!NOTE]
>
>Conversiepaden bevatten alle indrukken en klikken binnen de indruk van de adverteerder of klik op terugkijkvensters die zijn geconfigureerd in [!DNL Adobe Advertising Search]. Klikken krijgen de voorkeur boven indrukken tijdens conversie-toewijzing. Om het even welke kliks in een omzettingsweg ontvangen volledige kredieten die op de attributieregel worden gebaseerd. Impressies krijgen alleen krediet als er geen klikken worden bijgehouden in het conversiepad.

* *[!UICONTROL Last Event]:* Hiermee worden conversies toegewezen aan de laatste klik of indruk in het conversiepad.

* *[!UICONTROL Weight Last More]:* Hiermee worden conversies toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgen de laatste gebeurtenis het meeste gewicht en wordt het gewicht van de voorgaande gebeurtenissen achtereenvolgens minder.

* *[!UICONTROL Even Distribution]:* Hiermee worden conversies gelijkmatig toegewezen aan elke gebeurtenis in het conversiepad.

* *[!UICONTROL Weight First More]:* Hiermee worden conversies toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgen de eerste gebeurtenis het meeste gewicht en wordt het gewicht van de volgende gebeurtenissen achtereenvolgens minder.

* *[!UICONTROL First Event]:* Hiermee worden conversies toegewezen aan de eerste klik of de eerste indruk in het conversiepad.

* *[!UICONTROL U-shaped]:* Hiermee wordt de conversie toegewezen aan alle gebeurtenissen in het conversiepad, maar krijgt het grootste gewicht aan de eerste en laatste gebeurtenis, met achtereenvolgens minder gewicht aan de gebeurtenissen in het midden van het conversiepad.

* *[!UICONTROL Display Only]:*  Hiermee worden conversies toegewezen aan de laatste DSP klik of indruk in het conversiepad. Dit omvat video en aangesloten tv-advertenties en sluit klikken op [!DNL Adobe Advertising Search] advertenties.

* *[!UICONTROL Social Only]:* Achterhaald

<!-- See also [How Attribution Rules Are Calculated for Adobe Advertising](). -->

**[!UICONTROL Paths as Columns]:**  (Alle [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment], en [!UICONTROL Site] rapporten met [!UICONTROL Conversion Metrics] of [!UICONTROL Custom Goals] kolommen) Welke soorten omzettingen om te melden wanneer de vroegere gebeurtenissen op het zelfde apparaat voorkwamen. U kunt maximaal drie typen opnemen. Voor elk geselecteerd type wordt een aparte kolom opgenomen voor elke omzettingsmetrische waarde en toegevoegd met het opgegeven achtervoegsel ([!UICONTROL (tl)], [!UICONTROL (ct)], of [!UICONTROL (vt)]):

* *[!UICONTROL Total (TL) = CT + VT \* VT weight]:* Omvat omzettingen die aan kliks (CT voor kliks-door) en aan impressies (VT voor mening-door) worden toegeschreven. Conversies die worden toegewezen aan impressies worden vermenigvuldigd met het opgegeven doorkijkgewicht. Het standaardgezichtsdoorsgewicht is 100%, wat betekent dat omzettingen die aan indrukkingen worden toegeschreven, worden geteld als 100% van de waarde van omzettingen die aan kliks worden toegeschreven.

* *[!UICONTROL With Clicks (CT)]:* Omvat slechts omzettingen die aan kliks worden toegeschreven.

* *[!UICONTROL Impressions Only (VT)]:* Omvat slechts omzettingen die aan impressies werden toegeschreven omdat geen kliks in de omzettingsweg werden gevolgd.

**[!UICONTROL Conversion Reporting Based On]:**  Conversiegegevens rapporteren:

* *[!UICONTROL Conversion Timestamp]:* (De standaardwaarde) Conversies worden gekoppeld aan de conversiedatum.

* *[!UICONTROL Event Timestamp]:* Conversies worden gerapporteerd op basis van de datum van de indruk of klik die de conversie heeft veroorzaakt, zoals bepaald door het opgegeven [!UICONTROL Attribution Rule Settings].

## [!UICONTROL Add Report Destinations] Sectie

**[!UICONTROL Destination Type]:** Kies een van de volgende doeltypen:

* *[!UICONTROL S3]:* Om het voltooide rapport naar één of meerdere te verzenden [!DNL Amazon Simple Storage Service] ([!DNL Amazon S3]) locaties, die u opgeeft in het dialoogvenster **[!UICONTROL Destination Name]** veld.
* *[!UICONTROL sFTP]:* Om het voltooide rapport naar één of meerdere plaatsen te verzenden SFTP, die u in zult specificeren **[!UICONTROL Destination Name]** veld.
* *[!UICONTROL FTP]:* Om het voltooide rapport naar één of meerdere plaatsen van FTP te verzenden, die u in zult specificeren **[!UICONTROL Destination Name]** veld.
* *[!UICONTROL FTP SSL](Momenteel in bèta):* Om het voltooide rapport naar één of meerdere plaatsen van FTP te verzenden SSL, die u in zult specificeren **[!UICONTROL Destination Name]** veld.
* *[!UICONTROL Email]:* E-mailadres(sen) opgeven waarnaar ingevulde rapporten of meldingen moeten worden verzonden als het rapport door fouten wordt geannuleerd. Als u meerdere adressen wilt opgeven, scheidt u deze met komma&#39;s of spaties.

>[!NOTE]
>
> U kunt niet het bestemmingstype veranderen zodra u het rapport opslaat.

**[!UICONTROL Destination Name]:** (S3, FTP, sFTP, en de bestemmingstypes van FTP SSL slechts) De namen van de rapportbestemmingen waarnaar het douanerapport zal worden verzonden.

* Als u een bestaand doel wilt opgeven, selecteert u een doelnaam in de lijst. U kunt meerdere doelnamen afzonderlijk selecteren.

* Een nieuw doel maken:

   1. Klikken **Nieuw doel toevoegen**.

   1. Voer de [doelinstellingen rapport](/help/dsp/reports/report-destinations/report-destination-settings.md)en klik op **Opslaan**.

   1. Klik weer in de rapportinstellingen op **Doelnamen vernieuwen.**

      De nieuwe bestemming is nu beschikbaar van de lijst van bestaande bestemmingen, en u kunt naar keuze het aan het rapport toevoegen.

**[!UICONTROL Frequency]:** (Voor elke [!UICONTROL Destination Name] Hoe vaak om het rapport naar de bestemming te verzenden: *[!UICONTROL Once]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, of *[!UICONTROL Monthly]*.

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
>* [Info over Rapportdoelen](/help/dsp/reports/report-destinations/report-destination-about.md)

* [Beschikbare rapportkolommen](/help/dsp/reports/report-columns.md)
