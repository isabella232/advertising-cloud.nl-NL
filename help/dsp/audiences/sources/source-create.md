---
title: Creeer een Bron van het Publiek om Eerste Publiek te activeren
description: Leer hoe u een bron kunt maken voor het importeren van soorten publiek naar uw account of een adverteerderaccount.
feature: DSP Audiences
source-git-commit: d1ebbd79b6ccf0249829feef134122f083060563
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Creeer een Bron van het Publiek om Eerste Publiek te activeren

*Beta, functie*

<!-- Will this remain for admin users/Adobe account teams only? -->

Maak een bron voor het importeren van soorten publiek naar uw DSP of een advertentieaccount. U kunt op dit moment soorten publiek importeren uit [de [!DNL Adobe Real-Time Customer Data Profile (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html).

>[!NOTE]
>
>Nadat u een bron voor het [!DNL Real-Time CDP], moet u uw [!DNL Real-Time CDP] publiek door de bestemming Adobe Advertising Cloud DSP binnen [!DNL Real-Time CDP] om te beginnen met het importeren ervan. Zie [de stappen in de activeringsworkflow](source-about.md#workflow-sources).

1. Klik in het hoofdmenu op **[!UICONTROL Audiences] > [!UICONTROL Sources (BETA)].

1. Klik op [!UICONTROL Add Source].

1. In de [!UICONTROL Select a Type] selecteert u het type bron.

   *[!UICONTROL RT-CDP]*: Dit type bron, voor [de [!DNL Adobe Real-Time Customer Data Profile]](source-about.md), is de enige optie.

1. Geef de [!UICONTROL Data Visibility Level]: *[!UICONTROL Advertiser]* of *[!UICONTROL Account]*.

1. Geef de resterende gegevens op [broninstellingen](source-settings.md).

   Bewaar een kopie van de [!UICONTROL Source Key] dat wordt gegenereerd. U hebt de waarde later nodig.

1. Klik op **[!UICONTROL Save]**.

1. Maak in Experience Platform een Adobe Advertising Cloud DSP-doelverbinding met de [!UICONTROL Source Key] die is gegenereerd in de DSP broninstellingen.

Voor instructies voor het activeren van de Advertising Cloud bestemmingsverbinding, het selecteren van segmenten, en de toegang tot van controletoestemmingen, zie &quot;[Adobe Advertising Cloud DSP-verbinding](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).&quot;

>[!MORELIKETHIS]
>
>* [Broninstellingen voor publiek](source-settings.md)
>* [Ongeveer het Activeren van Authenticated Segmenten van de Bronnen van het Publiek](source-about.md)
>* [Activeer Erkende Segmenten van de Duurzame Partners van identiteitskaart](source-durable-id.md)<!-- title?-->
>* [Adobe Advertising Cloud DSP-verbinding](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [Over Audience Management](/help/dsp/audiences/audience-about.md)

