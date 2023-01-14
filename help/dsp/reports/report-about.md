---
title: Aangepaste rapporten
description: Leer over opties om douanerapporten manueel tot stand te brengen of pre-gevormde rapportmalplaatjes te gebruiken.
feature: DSP Custom Reports
exl-id: 59fc1894-1c9d-451d-b644-5640dd311547
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Aangepaste rapporten

Met aangepaste rapporten kunt u de inhoud en levering van uw rapportgegevens aanpassen aan de hand van de campagneafmetingen (zoals de adverteerder, plaatsing, sites of geos) en de maatstaven die het belangrijkst voor u zijn. U kunt:

* Vorm volledig de rapporten van de campagneprestaties op een korrelig niveau.
* Kies uit vooraf geconfigureerde rapportsjablonen en pas deze desgewenst verder aan.

U kunt rapporten eenmaal genereren, of ze plannen om dagelijks, wekelijks of maandelijks om 3:00 uur te worden gegenereerd in de opgegeven tijdzone. Zodra een rapport wordt geproduceerd, wordt het geleverd aan elke gespecificeerde e-mailontvanger of aan verbonden [rapportbestemmingen](/help/dsp/reports/report-destinations/report-destination-about.md) van de volgende typen:

* [!DNL Amazon Simple Storage Service] ([!DNL S3])
* FTP
* SFTP
* FTP SSL (in bèta)

>[!NOTE]
>
>U kunt ook gegevens op aanvraag weergeven op alle niveaus van een campagne (campagne, pakket, plaatsing of advertentie) [binnen de relevante campagnebeheervisie](/help/dsp/campaign-management/reports/campaign-reports-about.md).

## Beschikbare rapporttypen

* **[!UICONTROL Custom]:** Dit rapport is een leeg malplaatje u kunt gebruiken om uw eigen douanerapport tot stand te brengen gebruikend de meeste dimensies en metriek. [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], en [!UICONTROL Site] rapporten zijn variaties van dit malplaatje met vooraf geselecteerde kolommen en dimensies voor hun respectieve gebruiksgevallen.

* Vooraf geconfigureerde rapportsjablonen

   * **[!UICONTROL Billing]:** Gebruik dit rapport om belangrijke factureringsmetriek zoals uitgavenmetriek voor media het factureren door campagne te begrijpen.

      >[!NOTE]
      >
      >Dit rapport bevat gegevens over het factureringssegment. Als een gebruiker of een apparaat een indruk krijgt die tot veelvoudige segmenten behoort, slechts wordt één factureerbare segment met de indruk gecrediteerd.

   * **[!UICONTROL Conversion]:** Met dit rapport krijgt u inzicht in de manier waarop uw campagnes worden uitgevoerd op basis van conversiemetriek die is vastgelegd met het bijhouden van Adobe-advertenties. Dit rapport bevat multi-touchattributie.

   * **[!UICONTROL Device]:** Gebruik deze vooraf ingevulde sjabloon om belangrijke metriek per apparaat-gerelateerde afmetingen te bekijken.

   * **[!UICONTROL Frequency (by Impression)]:** Met dit rapport krijgt u inzicht in de distributie van afbeeldingen die worden weergegeven aan unieke viewers (bijvoorbeeld hoeveel unieke viewers één indruk, twee afbeeldingen, drie afbeeldingen enzovoort hebben gezien). Gegevens zijn beschikbaar via plaatsing of campagne.

      >[!NOTE]
      >
      >* Gegevens zijn beschikbaar na 1 maart 2019.
      >* De frequentie wordt geschat op basis van een steekproef van gegevens.
      >* Voor sommige inventarisaties geven uitgevers geen apparaat-id door, waardoor het bijhouden van de frequentie wordt verhinderd. Dit rapport bevat alleen afbeeldingen waarvoor een apparaat-id beschikbaar was.


   * **[!UICONTROL Frequency (by App/Site)]:** Gebruik dit rapport om te begrijpen hoeveel unieke gebruikers per app of per site zijn bereikt. U kunt ook zien hoeveel unieke gebruikers alleen via een bepaalde app of site (&quot;verschillende unieke gebruikers&quot;) zijn bereikt.

      >[!NOTE]
      >
      >* Gegevens zijn beschikbaar na 15 november 2018.
      >* Voor sommige privéinventarisaties geven uitgevers geen apparaat-id door, waardoor het bijhouden van de frequentie wordt verhinderd.


   * **[!UICONTROL Geo]**: Gebruik deze vooraf ingevulde sjabloon om de belangrijkste metriek op geografische afmetingen weer te geven.

   * **[!UICONTROL Margin]:** Gebruik dit rapport om belangrijke metriek zoals marge, winst, en andere uitgavenmetriek door campagne of plaatsing te zien.

   * **[!UICONTROL Segment]:** Gebruik dit vooraf ingevulde malplaatje om zeer belangrijke metriek door segment te zien.

      >[!NOTE]
      >
      >* Dit rapport is bedoeld om te tonen hoe de verschillende doelsegmenten presteren. Het gebruikt de gegevens van het segmentlidmaatschap. Wanneer een persoon of een apparaat dat tot twee of meer doelsegmenten behoort, de indruk krijgt, bevat dit rapport één rij voor elk segment. Daarom komen de totalen in dit rapport mogelijk niet overeen met de werkelijke levering.
      >* De metriek van de omzetting en de gegevens van het douanedoel voor segmenten zijn beschikbaar na 2 Augustus 2019. Alle andere gegevens voor segmenten zijn beschikbaar vanaf 1 juni 2018.


   * **[!UICONTROL Site]:** Standaard bevat dit standaard standaardcijfers, totale netto-uitgaven voor media en totale netto-uitgaven voor facturering per site.

## Rapportage tussen accounts {#cross-account-reporting}

Om het even welke organisatie met veelvoudige DSP rekeningen kan naar keuze dwars-rekeningsgegevens in douanerapporten toelaten, volgens de behoeften van de organisatie. U kunt bijvoorbeeld Account A toegang geven tot de gegevens van Account B en Account B toegang geven tot de gegevens van Account C (maar niet van Account A). Om deze eigenschap toe te laten en te vormen, contacteer uw [!DNL Adobe] accountteam.

Als de functie is ingeschakeld voor uw organisatie, kunt u [filter](report-settings.md) om het even welke volgende rapporttypes door rekening:  [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo], [!UICONTROL Device], [!UICONTROL Frequency (by Impression)], en [!UICONTROL Conversion].

Uw accountinstellingen op [!UICONTROL Settings] > [!UICONTROL Account] a) de andere accounts waarvan de gegevens beschikbaar zijn voor uw account en b) de andere accounts die toegang hebben tot de gegevens van uw account.

>[!MORELIKETHIS]
>
>* [Een aangepast rapport maken](/help/dsp/reports/report-create.md)
>* [Instellingen voor aangepaste rapporten](/help/dsp/reports/report-settings.md)
>* [Over rapporten in Platform](/help/dsp/campaign-management/reports/campaign-reports-about.md)
>* [Beschikbare rapportkolommen](/help/dsp/reports/report-columns.md)
>* [Info [!UICONTROL Report Destinations]](/help/dsp/reports/report-destinations/report-destination-about.md)

