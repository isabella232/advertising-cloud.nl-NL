---
title: Toevoegen [!DNL Analytics for Advertising Cloud] Macro's naar [!DNL Flashtalking] Labels toevoegen
description: Ontdek waarom en hoe u kunt toevoegen [!DNL Analytics for Advertising Cloud] macro's voor uw [!DNL Flashtalking] advertentietags
feature: Integration with Adobe Analytics
exl-id: 4b060668-723c-4cd2-b70e-409501ec67de
source-git-commit: 7cb39998041d151ece7809adc8a2e872b922e5fc
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Toevoegen [!DNL Analytics for Advertising Cloud] Macro&#39;s naar [!DNL Flashtalking] Labels toevoegen

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Alleen van toepassing op Advertising Cloud DSP*

Als u tags ad gebruikt van [!DNL Flashtalking] voor Advertising Cloud DSP-advertenties voegt u Analytics voor Advertising Cloud-parameters toe aan de URL&#39;s van de bestemmingspagina. De parameterrecord `s_kwcid` en `ef_id` query-tekenreeksparameters in de URL van de bestemmingspagina, zodat Advertising Cloud klikgegevens voor de advertenties naar Adobe Analytics kan verzenden.

Macro&#39;s gebruiken voor [!DNL Flashtalking] weergave- en videoadvertenties voor de volgende typen [!DNL Analytics for Advertising Cloud] implementaties:

* **Adverteerders met de [!DNL Adobe] [!DNL Analytics for Advertising Cloud] JavaScript-code geïmplementeerd op hun websites**: In de JavaScript-code worden de `s_kwcid` en `ef_id` querytekenreeksparameters. Het gebruik van macro&#39;s breidt het bijhouden van wijzigingen echter uit om op klikken gebaseerde conversies op te nemen wanneer cookies van derden niet worden ondersteund. U kunt het beste de macro&#39;s in de volgende secties aan uw advertentietags toevoegen om aanvullende doorklikgegevens vast te leggen die niet door de JavaScript-code worden vastgelegd.

>[!NOTE]
>
>De JavaScript-code is een oplossing om alleen op bijhouden te klikken als er nog cookies beschikbaar zijn. Wanneer de cookies zijn stopgezet, is het nodig de volgende macro&#39;s te implementeren.

* **Adverteerders van wie de websites de [!DNL Analytics for Advertising Cloud] JavaScript-code en vertrouwen in plaats daarvan op [!DNL Analytics] server-kant het door:sturen voor klik-door gegevens slechts** (zonder doorkijkgegevens): De volgende macro&#39;s zijn vereist om klikactiviteiten ter plaatse te melden die worden aangestuurd door advertenties die u via Advertising Cloud koopt.

## Ad-tags weergeven

Binnen de [!DNL Flashtalking] voeg de volgende macro toe aan het einde van de doorklikURL in het dialoogvenster `Clicktag` veld:

```html
?[ftqs:[AdobeAMO]]
```

Voorbeeld:  `https://www.adobe.com/products/photoshop?[ftqs:[AdobeAMO]]`

![Voorbeeld van [!DNL Flashtalking] instellingen voor advertentietags](/help/integrations/assets/macro-flashtalking-display-ad.png)

## Video-advertentietags

Binnen de [!DNL Flashtalking] voeg de volgende macro toe aan het einde van de doorklikURL in het dialoogvenster `Clicktag` veld:

```html
?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]
```

Voorbeeld:  `https://www.adobe.com/products/photoshop?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]`

![Voorbeeld van [!DNL Flashtalking] instellingen voor advertentietags](/help/integrations/assets/macro-flashtalking-video-ad.png)

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Advertising Cloud-id&#39;s gebruikt door [!DNL Analytics]](/help/integrations/analytics/ids.md)


<!-- >* [Append [!DNL Analytics for Advertising Cloud] Macros to [!DNL Google Campaign Manager 360] Ad Tags](macros-google-campaign-manager.md) -->
