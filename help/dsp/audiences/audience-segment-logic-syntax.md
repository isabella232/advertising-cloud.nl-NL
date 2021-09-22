---
title: Syntaxis voor Audience Segment Logic
description: Verwijs naar de syntaxis u kunt gebruiken om de logica voor publiekssegmenten te bepalen.
feature: DSP Audiences
exl-id: 3a51b1b5-1eef-453b-9be5-0694e27491a8
source-git-commit: d10e1c24ee7c93eaab3fd4fefe853860226cc8e2
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 0%

---

# Syntaxis voor Audience Segment Logic

Wanneer u herbruikbare soorten publiek maakt, kunt u de segmentlogica handmatig definiëren met alfanumerieke segment-id&#39;s en de volgende syntaxis:

* () om een groep aan te geven
* `||` for  [!DNL OR] <!-- || escaped with backticks so Jenkins doesn't think it's a Markdown table -->
* &amp;&amp; voor [!DNL AND]
* ! for [!DNL NOT] (exclude)

>[!NOTE]
>
>* Alle gespecificeerde segmentgroepen zijn inbegrepen tenzij zij door worden voorafgegaan ! (exclusief deze).


De volgende logica:

```
(X5vUk1cNvZxvBJ3jMjTt) || (sfvXrmQkk77PL5OtHpLH) && !(SMWSjTZFiy9hR1bKm1vw || x08UReA0IcP9HAJdcGVe)
```

means (in normale Engelse taal)

```
[!DNL INCLUDE] Segment ID X5vUk1cNvZxvBJ3jMjTt [!DNL OR] INCLUDE Segment ID sfvXrmQkk77PL5OtHpLH [!DNL AND EXCLUDE] (Segment ID SMWSjTZFiy9hR1bKm1vw AND Segment ID x08UReA0IcP9HAJdcGVe)
```

>[!NOTE]
>
>In plaatsingsmontages, kunt u opgeslagen publiek of als publiek gebruiken om uitdrukkelijk te richten of als afzonderlijke publiek om van het richten uit te sluiten. Zorg ervoor uw segmentlogica het doel weerspiegelt waarvoor u het publiek zult gebruiken.

>[!MORELIKETHIS]
>
>* [Over Audience Management](audience-about.md)
>* [Een herbruikbaar publiek maken](reusable-audience-create.md)
>* [Instellingen publiek](audience-settings.md)
>* [Beschikbare gegevensleveranciers van derden](third-party-data-providers.md)

