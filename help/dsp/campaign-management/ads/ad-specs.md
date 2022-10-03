---
title: Advertentiespecificaties
description: Algemene en uitgeverspecifieke referentiespecificaties.
feature: DSP Ads
exl-id: 905dfd9b-e7a3-4eb6-988f-b49d4b282dd2
source-git-commit: 8bc43253f15859c3b7dd7441fcbb4f34ecc98566
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Specificaties voor ondersteunde advertentietypen

## Video-advertenties (pre-Roll en CTV)

### Ondersteunde schermen

Advertenties worden standaard geleverd op desktopapparaten, mobiele apparaten en aangesloten tv-apparaten. Apparaatgericht is beschikbaar om de levering aan te passen.

### Ondersteunde externe advertentieservers

U kunt tagbladen gebruiken vanuit [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], en [!DNL Sizmek]. Voor een volledige lijst met ondersteunde leveranciers raadpleegt u &quot;[Certified Ad Serving Partners](certified-ad-servers.md).&quot;

### Vereisten voor High Definition Video Assets (vereist)

**Type videolabel:** VPAID 2.0 JavaScript of VAST (CTV). Alle VPAID&#39;s en eenheden moeten zich aan de [VPAID 2.0-specificatie](https://iabtechlab.com/wp-content/uploads/2016/04/VPAID_2_0_Final_04-10-2012.pdf) zoals gedefinieerd door het Interactive Advertising Bureau (IAB).

**Videocodec:** MP4/H.264

**Resolutie:** 1280x720 voor 720p, 1920x1080 voor 1080p

**Bitsnelheid:** 1500-2500 kbps voor 720p, 2500-3500 kbps voor 1080p

**H.264 Profiel/Niveau:** hoog profiel, niveau 3.1 voor 720p; Hoog profiel, niveau 4.0 voor 1080p

**Videoframesnelheid:** 29,970 fps (gewoonlijk aangeduid als 30 fps) voor NTSC-landen, 25 fps voor PAL-landen, 23,976 fps (gewoonlijk aangeduid als 24 fps) voor filmachineachtige inhoud

**Videokleurruimte:** 4:2:0 YUV Chromasubsampling

**Video-interliniëring:** Progressief scannen, d.w.z. niet-geïnterlinieerd. Geen beweging binnen het veld (overvloeiframes) of interliniëring.

**Leiders (leisteen):** Niet toegestaan

**Audiocodec:** AAC-LC of HE-AACv1

**Audiobitsnelheid:** 128-192 kbps voor AAC-LC, 64-128 kbps voor HE-AACv1

**Audiokanaal:** 2-kanaals stereomix

**Samplefrequentie audio:** 44,1 kHz of 48 kHz, volgens het uitgangsmateriaal

**Audioniveaus:** 24 LKFS (+/- 2,0 dB) in de VS volgens ATSC A/85; 23 SBL (+/- 1,0) in de EU volgens EBU R128

#### Aanvullende vereisten voor uitgevers voor aangesloten tv-advertenties

* **A+E-netwerk:** Zie A+E-netwerken [advertentiespecificaties](/help/dsp/assets/a-e-networks-tve-video-ad-specs.pdf)

* **Detectie:** Zie Detectie [advertentiespecificaties](/help/dsp/assets/discovery-networks-ad-specs.pdf).

* **Disney (incl. Hulu):** Zie Disney&#39;s [advertentiespecificaties](https://hulu.disneyadsales.com/ad-products/video-commercial/).

* **Max. HBO:** Zie HBO Max&#39;s [advertentiespecificaties](/help/dsp/assets/hbo-max-ad-specs-2022.xlsx).

* **NBCUniversal:**

   * [Digitale video](https://together.nbcuni.com/nbcu-creative-guidelines/digital-video/)

   * [Livestream](https://together.nbcuni.com/nbcu-creative-guidelines/livestream/)

   * [Peacock](https://together.nbcuni.com/nbcu-creative-guidelines/peacock/)

* **Bovengrens:** Zie Paramount&#39;s [advertentiespecificaties](https://www.paramount.com/digital-ads).

## Advertenties weergeven

### Ondersteunde schermen

Advertenties worden standaard geleverd op desktopapparaten en mobiele apparaten. Apparaatgericht is beschikbaar om de levering aan te passen.

### Ondersteunde bestandstypen

**Afbeelding:** GIF, JPG/JPEG, PNG

**HTML5:** Bestandstypen afbeelding: GIF, JPG/JPEG, PNG, SVG

### Vereisten voor afbeeldingselementen (vereist)

Universal Display wordt ondersteund.

**Aanbevolen advertentiegrootten:** 120x60, 160x600, 180x150, 300x50, 300x100, 300x1050, 300x250, 300x60 0, 320x50, 320x480, 480x60, 640x480, 88x31, 728x90, 970x250, 970x90

**Ondersteunde externe Advertentieservers:** U kunt tagbladen gebruiken vanuit [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], en [!DNL Sizmek]. Voor een volledige lijst met ondersteunde leveranciers raadpleegt u &quot;[Certified Ad Serving Partners](certified-ad-servers.md).&quot;

## Audiobanden

### Ondersteunde schermen

Desktop, mobiel, tablet, slimme luidsprekers en aangesloten tv

### Ondersteunde externe advertentieservers

U kunt tagbladen gebruiken vanuit [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], en [!DNL Sizmek]. Voor een volledige lijst met ondersteunde leveranciers raadpleegt u &quot;[Certified Ad Serving Partners](certified-ad-servers.md).&quot;

### Vereisten voor audio-elementen (vereist)

**Bestandstype:** MP3, OGG, AAC

**Bladeren (leisteen):**  Niet toegestaan

**Maximale bestandsgrootte:** 2 MB

**Bitsnelheid:** 128

**Bestandsafstand:** 0-60 s

#### Aanvullende vereisten voor uitgevers

* **[!DNL iHeartRadio]**
   * Lengte: 5, 15, 30 of 60 seconden
   * Bestandstype: MP3
   * Maximale bestandsgrootte: 320 kbps
   * Volume: 44,1 kHz

* **[!DNL Pandora]**
   * Lengte: 15 of 30 seconden
   * Bestandstype: MP4 (in-app), MP3 (bureaublad)
   * Maximale bestandsgrootte: 2,2 MB

* **[!DNL SoundCloud]**
   * Lengte: 6, 15 of 30 seconden
   * Bestandstype: MP3
   * Maximale bestandsgrootte: 5 MB

* **[!DNL Spotify]**
   * Lengte: Tot 30 seconden
   * Bestandstype: OGG
   * Maximale bestandsgrootte: 500 MB
   * Volume: RMS genormaliseerd tot -14; dBFS-piek genormaliseerd tot -0,2 dBFS

* **[!DNL TargetSpot]**
   * Lengte: 15, 30 of 60 seconden
   * Bestandstype: MP3

* **[!DNL TuneIn]**
   * Lengte: 10, 15 of 30 seconden
   * Bestandstype: MP3, OGG
   * Volume: 44,1 kHz

### Vereisten voor extra hulpmiddelen van de Banner (facultatief)

**Ondersteunde grootten:** 300x250, 500x500, 640x640, 1024x1024

#### Aanvullende vereisten voor uitgevers

* **[!DNL iHeartRadio]:**
   * Bestandstype: JPEG, JPG, PNG, GIF, SWF, HTML
   * Maximale bestandsgrootte: 2,2 MB
   * Dimension: 300 x 250

* **[!DNL Pandora]:**
   * Bestandstype: JPEG, GIF
   * Maximale bestandsgrootte: Grootte: 100 kB
   * Dimension: 300x250 (mobiel of bureaublad) of 500x500 (bureaublad)

* **[!DNL SoundCloud]:**
   * Bestandstype: Statische JPG, PNG
   * Maximale bestandsgrootte: Minder dan 400 kB
   * Dimension: 1024x1024

* **[!DNL Spotify]:**
   * Bestandstype: Statische JPG, PNG
   * Maximale bestandsgrootte: 200 kB
   * Dimension: 300 x 250

* **[!DNL TuneIn]:**
   * Bestandstype: JPEG, JPG, PNG, GIF, HTML
   * Maximale bestandsgrootte: 2 MB
   * Dimension: 300 x 250
 

## Systeemeigen weergaveadvertenties

Elke advertentie kan een stilstaand beeld of een bewegend GIF (cinemagraph) bevatten.

### Ondersteunde schermen

Advertenties worden standaard geleverd op desktopapparaten en mobiele apparaten. Apparaatgericht is beschikbaar om de levering aan te passen.

### Vereiste elementen voor alle native invoerindelingen

#### Afbeeldingselement

**Resolutie:** minimaal 600 x 600 px; Aanbevolen minimum van 1200 x 627 px

**Bestandstype:** JPEG (beeld en/of video en omslagbeeld), GIF (cinemografie)

**Bestandsgrootte:** Minder dan 1 MB (Afbeelding moet vrij van tekst zijn.)

#### Advertiserlogo

**Resolutie:** minimaal 80 x 80 px; Aanbevolen minimum van 300 x 300 px

**Bestandstype:** JPEG of PNG.

**Hoogte-breedteverhouding:**  1x1 verhouding

>[!NOTE]
>
>Afhankelijk van de afbeelding waarop de afbeelding wordt overschreven, kiest u tussen lichte of donkere logo-elementen.

#### Tekst/kopie

**Titel:** maximaal 200 tekens; 25 tekens aanbevolen

**Bijschrift:** maximaal 200 tekens; 100 tekens aanbevolen

**Gesponsord door:** maximaal 200 tekens; 30 tekens aanbevolen

**Oproep tot actie (alleen MoPub):** Maximaal 15 tekens

>[!NOTE]
>
>De uiteindelijke indeling wordt tijdens runtime door de uitgever gedefinieerd. Als een advertentie het geadviseerde karakteraantal overschrijdt, kunnen sommige voorraadleveranciers niet de advertentie leveren, of de uitgever of SSP kunnen de tekst beknotten.

#### URL van bestemmingspagina

De klikthrough URL met facultatieve klikspoor.

Vereisten voor kliktrackers:

* Pixels voor imitatie bij andere bedrijven: Alleen 1x1 afbeeldings-URL-indeling

* JavaScript-trackers voor weergavedoeleinden: Alleen ondersteund voor IAS; 1x1-afbeeldingen alleen in de indeling JS.append

* Klikspatiëringspixels van derden: Moet worden omgeleid naar de bestemmingspagina die is ingesloten in de URL (HTTP 302 omleiding)

* DMP (Data Management Platform)-klik op trackers met 200 of meer reacties worden niet ondersteund.

>[!MORELIKETHIS]
>
>* [Over Advertentiebeheer](ad-about.md)
>* [Eén advertentie maken](ad-create.md)
>* [Meerdere externe advertenties maken](ad-create-multiple.md)
>* [Een advertentie bewerken](ad-edit.md)

