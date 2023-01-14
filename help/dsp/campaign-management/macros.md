---
title: Reclame DSP macro's
description: Verwijs naar de beschikbare macro's voor het algemene volgen en om kliks op derdevertoningsadvertenties te volgen.
feature: DSP Ads
exl-id: e31cc2e5-ad1f-4555-a87b-0e4c3731fe5f
source-git-commit: ad978a021c063377e4c91ed41e902d98a03749e4
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Reclame DSP macro&#39;s

Een macro is een korte opdracht of korte opdracht voor een instructie en volgt doorgaans de indeling `${MACRO_NAME}`. Macro&#39;s die zijn opgenomen in creatieve code of doorklikken-URL&#39;s, worden uitgebreid naar een langere codereeks die de advertentieserver kan begrijpen. De DSP en server voeren macro&#39;s uit wanneer de advertentie wordt aangeboden of wanneer op de advertentie wordt geklikt.

Servermacro&#39;s van de advertentie zijn handig om belangrijke informatie door te geven aan DSP of aan externe ad-hocservers. Macro&#39;s worden het meest gebruikt tijdens de handel in creatieve code of meta-gegevens van derden en douane (zoals derdepixel).

U kunt een macro overal, zoals in een markering VAST, in om het even welke URL, of in een DSP of derdegebeurtenispixel manueel opnemen. Elke DSP client en partner heeft echter een andere indeling voor een advertentietag en de macro&#39;s moeten dienovereenkomstig op verschillende plaatsen in de tag worden ingevoegd. Elke keer dat u met een nieuwe client of partner werkt, vraagt u hen om documentatie over de plaats waar de macro&#39;s in hun advertentietags moeten worden ingevoegd die DSP.

## Algemene trackingsmacro&#39;s

Gebruik algemene &#39;tracking&#39;-macro&#39;s voor alle advertentietypen en tagtypen om zo nodig specifieke gegevens door te geven.

| Macro | Beschrijving van vervanging | Type |
| ----- | ----------------------- | ---- |
| `${TM_ACCOUNT_ID}` | De account-id. | integer |
| `${TM_AD_ID}` | De ad-toets (adKey). | string |
| `${TM_AD_ID_NUM}` | De advertentie-id. | integer |
| `${TM_ADVERTISER_ID}` | De adverteerder-id. | integer |
| `${TM_CAMPAIGN_ID}` | De campagnesleutel. | string |
| `${TM_CAMPAIGN_ID_NUM}` | De campagne-id. | integer |
| ` ${TM_CLICK_URL}` | De omleidings-URL, waarmee advertentieservers kunnen bijhouden en tellen en klikken. Wanneer de advertentie wordt aangeboden en de gebruiker erop klikt, wordt de macro geactiveerd en wordt de klik geregistreerd en geteld voor rapportagedoeleinden. | string |
| ` ${TM_CLICK_URL_URLENC}` | De gecodeerde omleidings-URL, waarmee ad-servers kunnen bijhouden en tellen en klikken. Wanneer de advertentie wordt aangeboden en de gebruiker erop klikt, wordt de macro geactiveerd en wordt de klik geregistreerd en geteld voor rapportagedoeleinden. Gebruik deze macro alleen als u advertenties van derden maakt en uw leverancier URL-codering vereist. | string |
| `${TM_FEED_ID}` | De sleutel voor de mediaplaatsing (feedKey). | string |
| `${TM_FEED_ID_NUM}` | De id voor de plaatsing van het medium. | integer |
| ` ${TM_MACRO_PLACEMENT_SITE_KEY` | De sitecode voor de plaatsing. Vereist voor [!DNL AppsFlyer] Klik op trackers voor mobiele apps voor installatiesadvertenties.<!-- should map to placement_site_key column of placement_site table --> | string |
| `${TM_PLACEMENT_ID}` | De plaatsingssleutel (cpKey). | string |
| `${TM_PLACEMENT_ID_NUM}` | De plaatsing-id. | integer |
| `${TM_RANDOM}` | Cachebuster: een willekeurig getal tussen 1 en 1000000. | lang |
| `${TM_SESSION_ID}` | De id van de sessie, die overeenkomt met één ophaalbewerking van de advertentietag. | string |
| `${TM_SITE_DOMAIN_URLENC}` | Het subdomein van de pagina dat wordt geparseerd vanaf de URL in de biedaanvraag. URL-gecodeerd. Niet ondersteund voor in-banner, klik-om-af te spelen advertenties. | string |
| ` ${TM_SITE_NAME}` | De sitenaam voor de plaatsing. | string |
| `${TM_SITE_URL_URLENC}` | De URL die in de biedaanvraag is doorgegeven; URL-gecodeerd. Niet ondersteund voor in-banner, klik-om-af te spelen advertenties. | string |
| `${TM_SITE_ID_NUM}` | De site-id voor de plaatsing. | integer |
| `${TM_TIMESTAMP}` | De Unix-tijdstempel die het aantal seconden aangeeft dat is verstreken sinds middernacht (00:00 UTC) op 1 januari 1970. | lang |
| ` ${TM_VIDEO_DURATION}` | De duur van de advertentievideo in seconden. | integer |

{style=&quot;table-layout:auto&quot;}

<!-- Removed because not found in code base:
|` ${TM_MACRO_PROMOTED_AD_KEY}` | The promoted ad key for the placement. Required for [!DNL AppsFlyer] click trackers for mobile app install ads. | string |
 -->

## Mobiele macro&#39;s

| Macro | Beschrijving van vervanging | Type |
| ----- | ----------------------- | ---- |
| `${CS_PLATFORM_ID}` | ([!DNL ComScore]) De platform-id, die overeenkomt met het besturingssysteem van het apparaat:<ul><li>`ios` = [!DNL Apple iOS]</li><li>`android` = [!DNL Google Android]</li><li>`windows` = [!DNL Windows Mobile]</li><li>`blackberry` = [!DNL Blackberry]</li> <li>`other` als het platform geen van de bovenstaande platformen is</li></ul> | varchar(50) |
| `${CS_DEVICE_MODEL}` | ([!DNL ComScore]) De naam van het apparaatmodel, URL-gecodeerd. | string |
| `${CS_IMPLEMENTATION_TYPE}` | ([!DNL ComScore]) De omgeving waarin de advertentie is bediend:<ul><li>`a` = mobiele toepassing</li><li>`b` = mobiele website</li></ul> | string (`a` of `b`) |
| `${NS_PLATFORM_ID}` | ([!DNL Nielsen]) De platform-id, die overeenkomt met het besturingssysteem van het apparaat:<ul><li>`ios`= [!DNL Apple iOS]</li><li>`android` = [!DNL Google Android]</li><li>`windows` = [!DNL Windows Mobile]</li><li>`blackberry` = [!DNL Blackberry]</li> <li>`other` als het platform geen van de bovenstaande platformen is</li></ul> | string |
| `${NS_DEVICE_GROUPING}` | ([!DNL Nielsen]) Het apparaattype waarop de advertentie viewer was:<ul><li>`TAB` = tablet</li><li>`PHN` = mobiel</li><li>`computer` = computer</li></ul> | string |
| `${UOO}` | ([!DNL Nielsen]) Of de gebruiker al dan niet heeft gekozen voor het volgen van advertenties:<ul><li>`1` (DNT-markering = 1) = de gebruiker heeft de advertentie niet bijgehouden</li><li>`0` (DNT-markering = 0) = de gebruiker heeft zich aangemeld voor het bijhouden van advertenties</li></ul> | integer (`0` of `1`) |
| `${TM_BUNDLE}` | De [!DNL iOS] of [!DNL Android] bundel-id van app store. Voorbeelden: com.zynga.wwf2.free of id804379658 | string |
| `gdpr=${GDPR_ENFORCED}&gdpr_consent=${GDPR_CONSENT}` | `gdpr=${GDPR_ENFORCED}` geeft aan of de bieder bepaalt dat het bod afkomstig is uit de Europese Unie en dat de GDPR-handhaving vereist:<ul><li>`1` = GDPR moet worden afgedwongen</li><li>`0` = GDPR dient niet te worden afgedwongen</li></ul>`gdpr_consent=${GDPR_CONSENT}` is de waarde van de instemming die door de leverancier in het binnenkomende biedverzoek is doorgegeven:<ul><li>In de meeste gevallen is dit een base64url-gecodeerde toestemmingskoord, of madeliefje (voorbeeld: BN5lERiOMYEdiAKAWXEND1HoSBE6CAFAApAMgBkIDIgM0AgOJxAnQA)</li><li>`0` = geen toestemming</li><li>`1` = toestemming</li></ul> | madeliefje of geheel getal |

{style=&quot;table-layout:auto&quot;}

## Klik op Macro&#39;s voor externe weergaveadvertenties

Als u kliks voor advertenties op nauwkeurige wijze wilt bijhouden met behulp van externe weergavetags, DSP is een klikmacro voor weergave vereist. Er is slechts één versie van de macro vereist; de desbetreffende macro is afhankelijk van het type tag.

| Macro | Beschrijving van vervanging | Type |
| ----- | ----------------------- | ---- |
| `${TM_CLICK_URL}` | De omleidings-URL waarmee advertentieservers het platform kunnen bijhouden, tellen en klikken. | string |
| `${TM_CLICK_URL_URLENC}` | De omleidings-URL waarmee advertentieservers die URL-codering nodig hebben, kunnen worden bijgehouden en geteld en op het platform kunnen worden geklikt. | string |

{style=&quot;table-layout:auto&quot;}

DSP voegt automatisch de weergave van klikmacro&#39;s in een externe weergavetag in wanneer u:

* Advertentietags exporteren van een partner van een advertentieserver <!-- [Needs PM confirmation.] -->
* Bulkupload [!DNL Flashtalking] of [!DNL Google DoubleClick for Advertisers] tags rechtstreeks in DSP plaatsen

Als een klikmacro ontbreekt wanneer u een vertoningsadvertentie bouwt, DSP toont een waarschuwingsbericht, die u ertoe aanzet om de aangewezen vertoning manueel op te nemen klikt macro in het correcte gebied van de markering.

## Problemen met macrofouten oplossen

Wanneer u macro&#39;s aan uw code toevoegt, zorg ervoor u de nauwkeurige syntaxis van de macro gebruikt. Wanneer u de macro&#39;s valideert, controleert DSP of de macro exact overeenkomt met een van de geldige macro&#39;s.

Er worden fouten gegenereerd als er tekens ontbreken aan het begin of einde van de macronaam. Er wordt bijvoorbeeld een foutbericht weergegeven als:

* U vergeet een of meer tekens aan het begin van de macronaam, zoals `${`. Als u de volledige syntaxis niet opneemt, wordt het item niet herkend als een geldige macro.
* De macro eindigt niet met een geldige set tekens, zoals `}`.

>[!MORELIKETHIS]
>
>* [Instellingen voor audio toevoegen](/help/dsp/campaign-management/ads/ad-settings-audio.md)
>* [Instellingen voor aangesloten tv-advertentie](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md)
>* [Ad-instellingen weergeven](/help/dsp/campaign-management/ads/ad-settings-display.md)
>* [Instellingen voor mobiele advertentie](/help/dsp/campaign-management/ads/ad-settings-mobile.md)
>* [Instellingen voor eigen advertentie](/help/dsp/campaign-management/ads/ad-settings-native.md)
>* [Instellingen voor pre-roll-advertentie](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md)
>* [Instellingen voor Universal Video Add](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)

