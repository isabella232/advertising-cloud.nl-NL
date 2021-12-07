---
title: Met de [!DNL Last Event Service] JavaScript-bibliotheek met [!DNL Web SDK]
description: Leer de stappen om over te schakelen van het gebruiken van [!DNL Analytics] [!DNL visitorAPI] library to the [!DNL Experience Platform] [!DNL Web SDK] library for your [!DNL Analytics for Advertising Cloud] uitvoering.
feature: Integration with Adobe Analytics
source-git-commit: 1ae45d0ceee2efc4fc52b86fd6737d4c7467a6ca
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Met de [!DNL Last Event Service] JavaScript-bibliotheek met Adobe Experience Platform [!DNL Web SDK]

*Adverteerders met alleen Advertising Cloud-Adobe Analytics-integratie*

Als uw organisatie de oudere Adobe Analytics gebruikt `visitorAPI.js` bibliotheek voor gegevensinzameling, kunt u naar keuze schakelen aan het gebruiken van [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html) bibliotheek (`alloy.js`), waardoor u via de [!DNL Edge Network].

De [!DNL Analytics for Advertising Cloud] [!DNL Last Event Service] JavaScript-bibliotheek, ongewijzigd, registreert gebeurtenissen view-through en click-through en koppelt deze aan de bijbehorende conversies met een aanvullende id (`SDID`). De [!DNL Web SDK] bibliotheek, echter, levert geen [!DNL stitch ID]. Als u de opdracht [!DNL Web SDK] for [!DNL Analytics for Advertising Cloud], moet u 1) wijzigen [!DNL Last Event Service] -tags die u op uw webpagina&#39;s gebruikt en 2) uw [!DNL Web SDK] `sendEvent` opdrachten dienovereenkomstig.

## Stap 1: Bewerk uw [!DNL Last Event Service] Label om een `[!DNL StitchID]`

In de [!DNL Analytics for Advertising Cloud] [!DNL Last Event Service] -tag die u gebruikt op uw webpagina&#39;s, voegt u code toe om de `[!DNL StitchID]` met behulp van de willekeurige id-generator die in de bibliotheek is gebundeld.

**Oudere tag:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          AdCloudEvent('IMS ORG Id');
</script>
```

**Nieuwe tag:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          stitchId = AdCloudEvent('IMS ORG Id').generateRandomId();
</script>
```

## Stap 2: Gebruiken [!DNL Web SDK] om de [!DNL StitchID] als XDM-gegevens voor [!DNL Analytics]

Voeg de volgende eigenschap in uw [!DNL Web SDK] `sendEvent` opdracht om de [!DNL StitchID] tot [!DNL Experience Edge] als [!DNL Experience Data Model] (XDM) gegevens voor [!DNL Analytics].<!-- The library will send the StitchID to [!DNL Experience Edge] as `[_adcloud.advertisingStitchID](https://github.com/adobe/xdm/blob/master/docs/reference/adobe/experience/adcloud/stitch.schema.md)`. --> [!DNL Analytics] gebruikt de waarde als een `SDID`.

**Toe te voegen eigenschap:**

```
     "_adcloud": {
       "advertisingStitchID": stitchId
     }
```

**Voorbeeld:**

```
<script>
  alloy("sendEvent", {
    "xdm": {
      "commerce": {
        "order": {
                ………
        }
     },
     "_adcloud": {
       "advertisingStitchID": stitchId
     }
    }
  });
</script>
```

>[!MORELIKETHIS]
>
>* [Overzicht van [!DNL Analytics for Advertising Cloud]](overview.md)
>* [JavaScript-code voor [!DNL Analytics for Advertising Cloud]](/help/integrations/analytics/javascript.md)

