---
title: Activeer Erkende Segmenten van de Duurzame partners van identiteitskaart
description: Meer informatie over het activeren van geverifieerde doelgroepen via een duurzame ID-oplossing.
feature: DSP Audiences
source-git-commit: 3059a5b211a8a219b02930f7f5763d5ec1467b8e
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Activeer Erkende Segmenten van de Duurzame partners van identiteitskaart

*Beta, functie*

Als u geverifieerde doelgroepen wilt activeren via een duurzame ID-oplossing in DSP voor advertenties, moeten uw segmenten worden vertaald in [!DNL RampIDs], die herkenbaar zijn in een biedbare omgeving. U kunt dit bereiken door:

* De DSP integratie met de [!DNL Adobe Real-Time Customer Data Profile (CDP)] en de [!DNL Adobe-LiveRamp Retrieval API].

* Handmatig geverifieerde segmenten verzenden naar DSP vanuit de [!DNL LiveRamp] [!DNL Connect] dashboard.

## Taken

1. Voor beide opties neemt u contact op met `adcloud-support@adobe.com` om de volgende montages in DSP toe te laten, die u zal toestaan om voor authentiek verklaarde segmenten in DSP campagnes te richten [alle stappen in de activeringsworkflow zijn voltooid](source-about.md#workflow-sources):

   1. [!DNL LiveRamp] [!DNL RampID] campagneconfiguratie voorafgaand aan segment delen van [!DNL Real-Time CDP].

   1. Het rekeningniveau &quot;[!UICONTROL LiveRamp segments]&quot;.

1. (Gebruikers delen geverifieerde segmenten handmatig via [!DNL LiveRamp]) Voer de volgende stappen uit in het dialoogvenster [!DNL LiveRamp] [!DNL Connect] dashboard:

   1. De doeltegel activeren **[!DNL AAC API 1P Onboarding]**.

   1. Set [!DNL Identifier Settings] tot **[!DNL Ramp ID]** alleen.

      ![Instellingen voor id](/help/dsp/assets/liveramp-tile-settings.png)

   1. (Optioneel) Als u nog steeds op cookies gebaseerde id&#39;s wilt ontvangen, maakt u een tweede id [!DNL AAC API 1P Onboarding] doeltegel met &quot;[!DNL Cookies],&quot; &quot;[!DNL IDFA],&quot; en &quot;[!DNL AAID]&quot; geselecteerd.

## Aanbevolen procedures voor het testen en valideren van gegevens

* **Doel [!DNL RampID]Op cookies gebaseerde segmenten en op cookie gebaseerde segmenten in afzonderlijke campagnes.**

   * Met de campagneinstellingen kan aan slechts één id de prioriteit worden toegekend.

   * Momenteel [!DNL RampIDs] kunnen niet worden opgehaald tijdens onsite gebeurtenissen. Dit betekent dat bepaalde douanedoelstellingen, zoals Laagste CPA en ROAS, niet beschikbaar met het gebruik van voor authentiek verklaarde segmenten zijn. Gebruik op cookies gebaseerde segmenten alleen als u een beperkende prestatie-KPI hebt.

* **Eén plaatsing maken in beide [!DNL RampID] en op cookies gebaseerde campagnes.**

   * De segmenten bepalen waarvan wordt gedeeld [!DNL LiveRamp] met behulp van het standaardsegmentactiveringsproces.

   * Werk met het ondersteuningsteam voor reclame van Adobe om de juiste gegevensdistributie te valideren.

Meer informatie over de DSP integratie met [!DNL LiveRamp], contact `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [Ongeveer het Activeren van Authenticated Segmenten van de Bronnen van het Publiek](source-about.md)
>* [Creeer een Bron van het Publiek om Eerste Publiek te activeren](source-create.md)
>* [Broninstellingen voor publiek](source-settings.md)
>* [Adobe Adverteren DSP Verbinding](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [Over Audience Management](/help/dsp/audiences/audience-about.md)

