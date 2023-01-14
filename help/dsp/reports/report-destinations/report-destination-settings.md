---
title: Doelinstellingen rapporteren
description: Zie de details die voor uw rapportbestemmingen, door bestemmingstype worden vereist.
feature: DSP Custom Reports
exl-id: 584c9c69-7b94-4e5c-bcc1-277ac2689d8e
source-git-commit: 17482b831c5db7ef6c211f87b2e408443180746e
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Doelinstellingen rapporteren

De details die voor niet-e-mailrapportbestemmingen worden vereist variëren door bestemmingstype.

>[!NOTE]
>
> U kunt uw douanerapporten aan e-mailontvangers ook leveren, die geen opgeslagen rapportbestemming vereisen. U kunt e-mailontvangers, in plaats van opgeslagen doelen, binnen de rapportinstellingen opgeven.

## [!UICONTROL S3]

**[!UICONTROL Name]:** Een naam waarmee u het doel kunt identificeren.

**[!UICONTROL S3 Bucket URL]:** Het volledige pad naar de map op het tabblad [!DNL Amazon Simple Storage Service] (S3) emmertje waarnaar het rapport wordt geüpload. Voorbeeld: `s3://dsp_account/reports`

**[!UICONTROL Access Key ID]:** De toegangstoets-id voor de ([!DNL Amazon S3]) emmer (verstrekt door [!DNL Amazon]).

**[!UICONTROL Secret Access Key]:** De geheime sleutel van de Toegang tot ([!DNL Amazon S3]) emmer (verstrekt door [!DNL Amazon]).

## [!UICONTROL FTP]

**[!UICONTROL Name]:** Een naam waarmee u het doel kunt identificeren.

**[!UICONTROL Server]:** De hostnaam voor de server.

**[!UICONTROL Port]:** Het poortnummer dat op de server moet worden gebruikt. De standaardwaarde is *[!UICONTROL 21]*.

**[!UICONTROL Username]:** De gebruikersnaam die moet worden gebruikt om zich aan te melden bij de server.

**[!UICONTROL Password]:** Het wachtwoord voor aanmelding bij de server.

**[!UICONTROL Path (Optional)]:** Het serverpad waarnaar de bestanden worden geüpload.

## [!UICONTROL SFTP]

**[!UICONTROL Name]:** Een naam waarmee u het doel kunt identificeren.

**[!UICONTROL Server]:** De hostnaam voor de server.

**[!UICONTROL Port]:** Het poortnummer dat op de server moet worden gebruikt. De standaardwaarde is *[!UICONTROL 21]*.

**[!UICONTROL Username]:** De gebruikersnaam die moet worden gebruikt om zich aan te melden bij de server.

**[!UICONTROL Password]:** Het wachtwoord voor aanmelding bij de server.

**[!UICONTROL Path (Optional)]:** Het serverpad waarnaar de bestanden worden geüpload.

## [!UICONTROL FTP SSL]

**[!UICONTROL Name]:** Een naam waarmee u het doel kunt identificeren.

**[!UICONTROL Server]:** De hostnaam voor de server.

**[!UICONTROL Port]:** Het poortnummer dat op de server moet worden gebruikt. De standaardwaarde is *[!UICONTROL 21]*.

**[!UICONTROL Username]:** De gebruikersnaam die moet worden gebruikt om zich aan te melden bij de server.

**[!UICONTROL Password]:** Het wachtwoord voor aanmelding bij de server.

**[!UICONTROL Path (Optional)]:** Het serverpad waarnaar de bestanden worden geüpload.

>[!MORELIKETHIS]
>
>* [Info [!UICONTROL Report Destinations]](/help/dsp/reports/report-destinations/report-destination-about.md)
>* [Een [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-create.md)
>* [Een [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-edit.md)
>* [Een [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-delete.md)

