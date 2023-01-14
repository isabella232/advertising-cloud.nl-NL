---
title: Een aangepast doel maken
description: Een aangepast doel maken
feature: DSP Optimization
exl-id: 440ded21-92d3-41ad-839f-ebc8376aa932
source-git-commit: ad4ab8b9b0a4b5b1cc4aab540900363d2fe671c2
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Een aangepast doel maken

U kunt aangepaste doelen maken als *doelstellingen* binnen [!DNL Adobe Advertising Search].

Als u een aangepast doel wilt maken, moet de DSP-account zijn gekoppeld aan een [!DNL Search] account met dezelfde Adobe Experience Cloud-organisatie-id, van binnen de [!DNL Search] clientinstellingen. Als uw DSP niet is gekoppeld aan een [!DNL Search] account, neem contact op met uw [!DNL Adobe] accountteam.

>[!TIP]
>
>Zie de [aanbevolen procedures voor het maken van aangepaste doelen](custom-goal-best-practices.md) voor uiteinden op hoe te om uw douanedoelstellingen te vormen.

1. Aanmelden [!DNL Adobe Advertising Search] bij (Amerikaanse ondernemingen) [`https://enterprise-na.efrontier.com`](https://enterprise-na.efrontier.com) of (ondernemingen in alle andere landen) [`https://enterprise-intl.efrontier.com`](https://enterprise-intl.efrontier.com).
1. Zorg ervoor dat de meetgegevens die u in uw doel wilt opnemen, zijn bijgehouden, beschikbaar zijn in het product en een weergavenaam bevatten:
   1. Klik in het hoofdmenu op **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Transaction Properties]**.
   1. Bepaal de plaats van metrisch, en zorg ervoor dat **[!UICONTROL Show in UI and Reports]** wordt toegelaten voor metrisch.
   1. Als metrisch geen waarde in metrisch heeft **[!UICONTROL Display Name]** , klikt u in de cel, voert u de weergavenaam in en klikt u op **[!UICONTROL Apply].**
1. Het aangepaste doel maken als een *doel*:
   1. Klik in het hoofdmenu op **[!UICONTROL Search]> [!UICONTROL Optimization] >[!UICONTROL Objectives]**.
   1. Klik op de werkbalk op **[!UICONTROL Create objective].**
   1. Voer de objectieve instellingen in:
      1. In de **[!UICONTROL Change Objective Name]** voert u de objectieve naam in.

         De objectieve naam wordt weergegeven in het [!UICONTROL Custom Goals] in de instellingen van het DSP pakket.

      1. Eigenschappen koppelen aan het doel:

         >[!NOTE]
         >
         > Alle transactieeigenschappen die voor de adverteerder worden bijgehouden, worden standaard vermeld in het dialoogvenster [!UICONTROL Available Properties] lijst.

         * Als u een CSV-bestand met eigenschappen en hun gewichten wilt importeren, klikt u op **[!UICONTROL Import]** en zoek het bestand dat u wilt importeren.

            De geïmporteerde eigenschappen moeten al bestaan voor de adverteerder; de namen zijn niet hoofdlettergevoelig.

            De geïmporteerde eigenschappen vervangen de bestaande opgegeven eigenschappen.

         * Als u de eerste eigenschap handmatig wilt opgeven met de standaarddikte (1), selecteert u een optie in een lijst met alle transactieeigenschappen die voor de adverteerder worden bijgehouden.

         * Als u handmatig een andere eigenschap met de standaarddikte (1) wilt toevoegen, klikt u op **[!UICONTROL +]** .

            >[!TIP]
            >
            > Als u naar een eigenschap in de lijst wilt zoeken, voert u een tekenreeks in vanuit de naam van de eigenschap.

         * Als u handmatig meerdere eigenschappen wilt toevoegen, klikt u op **[!UICONTROL Add Multiple Properties].** Voor elke eigenschap die u wilt toevoegen, klikt u op de naam van de eigenschap in het dialoogvenster [!UICONTROL Available Properties] en sleep deze naar de [!UICONTROL Added Properties] kolom. Wanneer u klaar bent met het toevoegen van eigenschappen, klikt u op **[!UICONTROL Add]**.

            >[!TIP]
            >
            >* Als u naar een eigenschap in de lijst wilt zoeken, voert u in het invoerveld een tekenreeks in vanuit de naam van de eigenschap.
            >* Als u de lijst wilt filteren om eigenschappen uit te sluiten die zijn uitgesloten in rapporten, selecteert u de optie **[!UICONTROL Hide properties excluded from reports].**


         * (Als het doel meerdere eigenschappen bevat) Als u het gewicht van een eigenschap wilt wijzigen ten opzichte van de andere eigenschappen in het doel, voert u waarden in in het dialoogvenster **[!UICONTROL Weight]** veld(en).
      1. Klik onder aan de instellingen op **[!UICONTROL Save]**.


Wanneer u een doel hebt gemaakt, kunt u het als aangepast doel toewijzen aan een DSP pakket wanneer het optimalisatiedoel &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot; of &quot;[!UICONTROL Lowest CPA - Custom Goal].&quot;

>[!TIP]
>
>Voor optimale prestaties, moeten de gecombineerde metriek in het douanedoel (doelstelling) minstens tien omzettingen per dag in totaal omvatten. Als dat niet het geval is, kunt u het beste aanvullende ondersteunende gebeurtenissen (transactieeigenschappen), zoals productpagina&#39;s of toepassingen, aan het doel toevoegen. Zie [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md) voor richtsnoeren.

>[!MORELIKETHIS]
>
>* [Aangepaste doelen](custom-goal-about.md)
>* [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)

