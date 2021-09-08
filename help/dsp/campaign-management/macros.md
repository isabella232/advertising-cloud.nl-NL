---
title: Advertising Cloud DSP Macros
description: Verwijs naar de beschikbare macro's voor het algemene volgen en om kliks op derdevertoningsadvertenties te volgen.
feature: Ads
exl-id: e31cc2e5-ad1f-4555-a87b-0e4c3731fe5f
source-git-commit: 185fc7d79798a0a3a9ad5829b701aeb53a4a47c1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Advertising Cloud DSP Macros

Een macro is een korte opdracht of korte opdracht voor een instructie en volgt gewoonlijk de notatie `${MACRO_NAME}`. De Advertising Cloud DSP en de server voeren macro&#39;s uit wanneer de advertentie wordt bediend of geklikt.

Macro&#39;s worden het meest gebruikt tijdens de handel in creatieve code of meta-gegevens van derden en douane (zoals derdepixel).

## Algemene trackingsmacro&#39;s

Gebruik algemene &#39;tracking&#39;-macro&#39;s voor alle advertentietypen en tagtypen om zo nodig specifieke gegevens door te geven.

| Macro | Beschrijving |
| --------------- | ---------------------- |
| `${USER_ID}` | Gebruiker-id voor alle apparaattypen. |
| `${TM_RANDOM}` | Cachebuster: een willekeurig getal tussen 1 en 1000000 |
| `${TM_PLACEMENT_ID_NUM}` | De plaatsings-id |
| `${TM_SITE_URL_URLENC}` | De URL die in de biedaanvraag is doorgegeven; URL-gecodeerd |
| `${TM_SITE_DOMAIN_URLENC}` | Het subdomein van de pagina dat wordt geparseerd vanaf de URL in de biedaanvraag. URL-gecodeerd |

{style=&quot;table-layout:auto&quot;}

## Klik op Macro&#39;s voor externe weergaveadvertenties

Als u kliks voor advertenties op nauwkeurige wijze wilt bijhouden met behulp van externe weergavetags, DSP is een klikmacro voor weergave vereist. Er is slechts één versie van de macro vereist; de desbetreffende macro is afhankelijk van het type tag.

| Macro | Beschrijving |
| --------------- | ---------------------- |
| `${TM_CLICK_URL}` | URL omleiden waarmee advertentieservers het platform kunnen bijhouden en tellen en klikken |
| `${TM_CLICK_URL_URLENC}` | Omleiden URL die toelaat en servers die URL coderen vereisen om te volgen en te tellen en in het platform te klikken |

{style=&quot;table-layout:auto&quot;}

DSP voegt automatisch de weergave toe en klikt op macro&#39;s in een weergavetag wanneer u:

* Advertentietags exporteren van een Advertising Cloud en een serverpartner <!-- [Needs PM confirmation.] -->
* Upload [!DNL Flashtalking] of [!DNL Google DoubleClick for Advertisers] ad tags direct in DSP

Als een klikmacro ontbreekt wanneer u een vertoningsadvertentie bouwt, DSP toont een waarschuwingsbericht, die u ertoe aanzet om de aangewezen vertoning manueel op te nemen klikt macro in het correcte gebied van de markering.

>[!MORELIKETHIS]
>
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-audio.md)
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md)
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-display.md)
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-mobile.md)
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-native.md)
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md)

