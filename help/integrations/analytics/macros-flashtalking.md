---
title: Toevoegen [!DNL Analytics for Advertising Cloud] Macro's naar [!DNL Flashtalking] Labels toevoegen
description: Ontdek waarom en hoe u kunt toevoegen [!DNL Analytics for Advertising Cloud] macro's voor uw [!DNL Flashtalking] advertentietags
feature: Integration with Adobe Analytics
source-git-commit: 915eea83b2dd246f0f512981efca7ac481cf0c6c
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Toevoegen [!DNL Analytics for Advertising Cloud] Macro&#39;s naar [!DNL Flashtalking] Labels toevoegen

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

*Alleen van toepassing op Advertising Cloud DSP*

Als u tags ad gebruikt van [!DNL Flashtalking] voor Advertising Cloud DSP-advertenties voegt u Analytics voor Advertising Cloud-parameters toe aan de URL&#39;s van de bestemmingspagina. Met de parameters kan Advertising Cloud klikgegevens voor de advertenties naar Adobe Analytics verzenden.

Macro&#39;s gebruiken voor [!DNL Flashtalking] weergave- en videoadvertenties voor de volgende typen [!DNL Analytics for Advertising Cloud] implementaties:

* **Adverteerders met de [!DNL Adobe] [!DNL Analytics for Advertising Cloud] JavaScript-code geïmplementeerd op hun websites**: In Adobe Analytics zijn er klikgegevens beschikbaar van advertenties die je via Advertising Cloud koopt, zonder extra macro&#39;s. Als u doorklikgegevens wilt vastleggen in browsers die geen cookies van derden ondersteunen en daarom niet door de JavaScript-code worden vastgelegd, voegt u de macro&#39;s in de volgende secties toe aan uw [!DNL Flashtalking] advertentietags.

>[!NOTE]
>
>De JavaScript-code is een oplossing om alleen op bijhouden te klikken als er nog cookies beschikbaar zijn. Zodra Advertising Cloud de cookies beëindigt, is het nodig de volgende macro&#39;s te implementeren.

* **Adverteerders van wie de websites de [!DNL Analytics for Advertising Cloud] JavaScript-code en vertrouwen in plaats daarvan op [!DNL Analytics] server-kant het door:sturen voor klik-door gegevens slechts** (zonder doorkijkgegevens): De volgende macro&#39;s zijn vereist voor het rapporteren van onsite klikactiviteiten op advertenties die je via Advertising Cloud koopt.

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


<!-- >* [Append [!DNL Analytics for Advertising Cloud] Macros to [!DNL Google Campaign Manager 360] Ad Tags](macros-google-campaign-manager.md) -->
