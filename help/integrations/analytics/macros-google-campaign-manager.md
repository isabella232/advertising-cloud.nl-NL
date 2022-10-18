---
title: Toevoegen [!DNL Analytics for Advertising Cloud] Macro's naar [!DNL Google Campaign Manager 360] Labels toevoegen
description: Ontdek waarom en hoe u kunt toevoegen [!DNL Analytics for Advertising Cloud] macro's voor uw [!DNL Google Campaign Manager 360] advertentietags
feature: Integration with Adobe Analytics
exl-id: 05084a85-5890-4a82-b3eb-4520f44f9d66
source-git-commit: 7cb39998041d151ece7809adc8a2e872b922e5fc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Toevoegen [!DNL Analytics for Advertising Cloud] Macro&#39;s naar [!DNL Google Campaign Manager 360] Labels toevoegen

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Alleen van toepassing op Advertising Cloud DSP*

Als u tags ad gebruikt van [!DNL Google Campaign Manager 360] voor Advertising Cloud DSP-advertenties voegt u Analytics voor Advertising Cloud-parameters toe aan de URL van de bestemmingspagina met behulp van de [`%p` macro](https://support.google.com/campaignmanager/table/6096962). De parameterrecord `s_kwcid` en `ef_id` query-tekenreeksparameters in de URL van de bestemmingspagina, zodat Advertising Cloud klikgegevens voor de advertenties naar Adobe Analytics kan verzenden.

Macro&#39;s gebruiken voor [!DNL Campaign Manager 360] weergave- en videoadvertenties voor de volgende typen [!DNL Analytics for Advertising Cloud] implementaties:

* **Adverteerders met de [!DNL Adobe] [!DNL Analytics for Advertising Cloud] JavaScript-code geïmplementeerd op hun websites**: In de JavaScript-code worden de `s_kwcid` en `ef_id` querytekenreeksparameters. Het gebruik van macro&#39;s breidt het bijhouden van wijzigingen echter uit om op klikken gebaseerde conversies op te nemen wanneer cookies van derden niet worden ondersteund. U kunt het beste de macro&#39;s in de volgende secties aan uw advertentietags toevoegen om aanvullende doorklikgegevens vast te leggen die niet door de JavaScript-code worden vastgelegd.

>[!NOTE]
>
>De JavaScript-code is een oplossing om alleen op bijhouden te klikken als er nog cookies beschikbaar zijn. Wanneer de cookies zijn stopgezet, is het nodig de volgende macro&#39;s te implementeren.

* **Adverteerders van wie de websites de [!DNL Analytics for Advertising Cloud] JavaScript-code en vertrouwen in plaats daarvan op [!DNL Analytics] server-kant het door:sturen voor klik-door gegevens slechts** (zonder doorkijkgegevens): De volgende macro&#39;s zijn vereist om klikactiviteiten ter plaatse te melden die worden aangestuurd door advertenties die u via Advertising Cloud koopt.

## De macro&#39;s toevoegen aan uw [!DNL Google Campaign Manager 360] Adds

Within [!DNL Google Campaign Manager 360]voegt u voor elk van uw weergave- en videoadvertenties de volgende parameter toe aan de URL van de bestemmingspagina: `%pamo=!;`

U kunt de URL van de bestemmingspagina op verschillende manieren opgeven. De volgende subsecties bevatten instructies voor elke optie.

Hieronder ziet u een voorbeeld van de URL van de landingspagina die is opgemaakt met het achtervoegsel.

```
https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;
```

>[!NOTE]
>
>
>* Als de bestemmingspagina-URL een hash-symbool (#) bevat, wat niet gebruikelijk is, plaatst u de URL `amo` vóór het hashsymbool.
>* Als er geen andere parameters zijn opgenomen na de `amo` voegt u vervolgens een parameter toe (bijvoorbeeld &amp;a=b). Voorbeeld:`https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;&a=b#login`


### URL-achtervoegsel van bestemmingspagina op advertentieniveau configureren

1. Klik in het hoofdmenu op de knop [!UICONTROL Advertisers] tab.
1. Klik op de naam van de adverteerder.
1. In de [!UICONTROL Landing page URL suffix] instellingen, inclusief `%pamo!;` in de [!UICONTROL URL suffix] veld.

![instellingen op adverteerderniveau](/help/integrations/assets/macro-ggl360-advertiser.png)

### Het achtervoegsel URL van bestemmingspagina op campagnereniveau configureren

1. Klik in het hoofdmenu op de knop [!UICONTROL Campaigns] tab.
1. Klik op de naam van de campagne.
1. Klik op [!UICONTROL Properties].
1. In de [!UICONTROL Landing page URL suffix] instellingen, inclusief `%pamo!;` in de [!UICONTROL URL suffix] veld.

![instellingen op campagnereniveau](/help/integrations/assets/macro-ggl360-campaign.png)

### URL-achtervoegsel van bestemmingspagina op creatief niveau configureren

1. Klik in het hoofdmenu op de knop [!UICONTROL Campaigns] tab.
1. Klik op de naam van de campagne.
1. In de [!UICONTROL Views] menu, selecteert u [!UICONTROL Creatives].
1. Klik op de creatieve naam.
1. In de [!UICONTROL Click tags] instellen, include `%pamo!;` in de [!UICONTROL Landing page] voor de kliktag.

![instellingen op creatief niveau](/help/integrations/assets/macro-ggl360-creative.png)

## Hoe [!DNL Analytics for Advertising Cloud] Macro&#39;s worden uitgebreid in DSP

Wanneer u in DSP een advertentie maakt die de opdracht [!DNL Analytics for Advertising Cloud] parameter (`amo`), de `ef_id` en `s_kwcid` macro&#39;s worden automatisch toegevoegd aan de klik-URL. De beste manier is om de tag in DSP te controleren om ervoor te zorgen dat de `ef_id` en `s_kwcid` macro&#39;s zijn aanwezig.

Hier volgt een voorbeeld van een [!DNL Google Campaign Manager 360] [De tag ins](https://support.google.com/campaignmanager/answer/6080468) zoals deze in DSP wordt weergegeven.

```
<ins class='dcmads' style='display:inline-block;width:160px;height:600px'
data-dcm-placement='N6482.2155306TUBEMOGUL/B23486129.261313631'
data-dcm-rendering-mode='iframe'
data-dcm-https-only
data-dcm-resettable-device-id=''
data-dcm-app-id='' data-dcm-click-tracker='${TM_CLICK_URL}'
data-dcm-param-amo='ef_id=${TM_USER_ID}:${TM_DATETIME}:d&s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}'>
<script src='https://www.googletagservices.com/dcm/dcmads.js'></script>
</ins>
```

Wanneer een gebruiker op de advertentie klikt, [!DNL Google Campaign Manager 360] ziet `%pamo` in het URL-achtervoegsel en voegt dynamisch de waarde van de `amo` in de URL.


>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]](/help/integrations/analytics/ids.md)
>* [Toevoegen [!DNL Analytics for Advertising Cloud] Macro&#39;s naar [!DNL Flashtalking] Labels toevoegen](macros-flashtalking.md)

