---
title: Aangepaste doelen
description: Leer over douanedoelstellingen om uw succesgebeurtenissen te bepalen in pakketten die voor laagste CPA of hoogste ROAS worden geoptimaliseerd.
feature: DSP Optimization
exl-id: 623cb1ef-85ab-4535-aa3a-8e6ec8ae15ee
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Aangepaste doelen

De doelstellingen van de douane bepalen de succesgebeurtenissen die een adverteerder vereist om zijn bedrijfsdoelstellingen te ontmoeten. Elk pakket dat de optimalisatiedoelstellingen &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot;of &quot;[!UICONTROL Lowest CPA - Custom Goal]&quot;gebruikt moet een douanedoel omvatten dat de algemene optimalisatiedoelstelling zal helpen bereiken. U kunt aangepaste doelen maken als *doelstellingen* in Advertising Cloud Search.

![aangepaste doelen](/help/dsp/assets/objective-goals.png)

Elk douanedoel bestaat uit één of meerdere metriek, of *transactieeigenschappen*, en de relatieve gewichten van die transactieeigenschappen. Tot de beschikbare transactieeigenschappen behoren alle meetgegevens die worden bijgehouden met de Advertising Cloud-conversiepixel en via Adobe Analytics.

>[!NOTE]
>
>* [!DNL Analytics] afmetingen en segmenten zijn niet beschikbaar voor Advertising Cloud-optimalisatie.
>* Om de gebeurtenissen van de Analyse in DSP te gebruiken, werk met uw de rekeningsmanager van Adobe om een adverteerder-vlakke integratie te vormen.
>* [!DNL Analytics] aangepaste gebeurtenissen volgen deze naamgevingsconventie:  `custom_event_[*event #*]_[*Analytics report suite ID*]`. Voorbeeld: `custom_event_16_examplersid`


Stel dat drie metriek (transactieeigenschappen) relevant zijn voor een specifiek pakket in een van uw campagnes: &quot;PDF-download&quot; gewaardeerd op 20 USD, &quot;E-mailaanmelding&quot; gewaardeerd op 30 USD en &quot;Bestelbevestiging&quot; gewaardeerd op 40 USD. Als u gewicht wilt geven volgens de eenmalige monetaire waarde van de actie van de klant, dan zouden de relatieve gewichten van de eigenschappen 1, 2, en 1.5 zijn.

Zie [beste praktijken voor het creëren van douanedoelstellingen](custom-goal-best-practices.md) voor uiteinden op hoe te om uw douanedoelstellingen te vormen.

Als u [een aangepast doel ](custom-goal-create.md) hebt gemaakt, kunt u [dit toewijzen aan een pakket](/help/dsp/campaign-management/packages/package-settings.md) voor rapportage en algoritmische optimalisatie met Adobe Sensei.

>[!MORELIKETHIS]
>
>* [Een aangepast doel maken](custom-goal-create.md)
>* [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)

