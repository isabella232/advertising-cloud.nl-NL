---
title: Aangepaste doelen
description: Leer over douanedoelstellingen om uw succesgebeurtenissen te bepalen in pakketten die voor laagste CPA of hoogste ROAS worden geoptimaliseerd.
feature: DSP Optimization
exl-id: 623cb1ef-85ab-4535-aa3a-8e6ec8ae15ee
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Aangepaste doelen

De doelstellingen van de douane bepalen de succesgebeurtenissen die een adverteerder vereist om zijn bedrijfsdoelstellingen te ontmoeten. Elk pakket dat de optimalisatiedoelstellingen gebruikt &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot; of &quot;[!UICONTROL Lowest CPA - Custom Goal]&quot; moet een aangepast doel bevatten dat zal helpen het algemene optimalisatiedoel te bereiken. U kunt aangepaste doelen maken als *doelstellingen* in [!DNL Adobe Advertising Search].

![aangepaste doelen](/help/dsp/assets/objective-goals.png)

Elk douanedoel bestaat uit één of meerdere metriek, of *transactieeigenschappen* en de relatieve gewichten van die transactieeigenschappen. Tot de beschikbare transactieeigenschappen behoren alle meetgegevens die worden bijgehouden met de conversiepixel Adobe Advertising en via Adobe Analytics.

>[!NOTE]
>
>* [!DNL Analytics] De afmetingen en de segmenten zijn niet beschikbaar voor Adobe Advertising optimization.
>* Als u Analytics-gebeurtenissen wilt gebruiken in DSP, werkt u met uw [!DNL Adobe] -accountteam configureren voor integratie op adverteerderniveau.
>* [!DNL Analytics] aangepaste gebeurtenissen volgen deze naamgevingsconventie: `custom_event_[*event #*]_[*Analytics report suite ID*]`. Voorbeeld: `custom_event_16_examplersid`


Stel dat drie metriek (transactieeigenschappen) relevant zijn voor een specifiek pakket in een van uw campagnes: &quot;PDF Download&quot; gewaardeerd op 20 USD, &quot;Email Sign up&quot; gewaardeerd op 30 USD en &quot;Order Confirmation&quot; getaxeerd op 40 USD. Als u gewicht wilt geven volgens de eenmalige monetaire waarde van de actie van de klant, dan zouden de relatieve gewichten van de eigenschappen 1, 2, en 1.5 zijn.

Zie de [aanbevolen procedures voor het maken van aangepaste doelen](custom-goal-best-practices.md) voor uiteinden op hoe te om uw douanedoelstellingen te vormen.

Eenmaal [een aangepast doel maken](custom-goal-create.md), kunt u [toewijzen aan een pakket](/help/dsp/campaign-management/packages/package-settings.md) voor rapportage en algoritmische optimalisatie met Adobe Sensei.

>[!MORELIKETHIS]
>
>* [Een aangepast doel maken](custom-goal-create.md)
>* [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)

