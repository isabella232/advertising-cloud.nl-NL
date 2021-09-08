---
title: Een aangepast doel maken
description: Een aangepast doel maken
feature: Optimization
exl-id: 440ded21-92d3-41ad-839f-ebc8376aa932
source-git-commit: 0f0a2e907d39900968b29c3b59c8034b604911ce
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Een aangepast doel maken

>[!TIP]
>
>Zie [beste praktijken voor het creëren van douanedoelstellingen](custom-goal-best-practices.md) voor uiteinden op hoe te om uw douanedoelstellingen te vormen.

1. Meld u aan bij Advertising Cloud Search (Amerikaanse bedrijven) [`https://enterprise-na.efrontier.com`](https://enterprise-na.efrontier.com) of (bedrijven in alle andere landen) [`https://enterprise-intl.efrontier.com`](https://enterprise-intl.efrontier.com).
1. Zorg ervoor dat de metriek die u in uw doel wilt opnemen, is bijgehouden, beschikbaar is in het product en een weergavenaam bevat:
   1. Klik in het hoofdmenu op **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Transaction Properties]**.
   1. Bepaal de plaats van metrisch, en zorg ervoor dat **[!UICONTROL Show in UI and Reports]** voor metrisch wordt toegelaten.
   1. Als metrisch geen waarde in **[!UICONTROL Display Name]** kolom heeft, klik in de cel, ga de vertoningsnaam in, en klik dan **[!UICONTROL Apply].**.
1. Creeer het douanedoel als *doelstelling*:
   1. Klik in het hoofdmenu op **[!UICONTROL Search]> [!UICONTROL Optimization] >[!UICONTROL Objectives]**.
   1. Klik in de werkbalk op **[!UICONTROL Create objective].**
   1. Voer de objectieve instellingen in:
      1. Voer in het veld **[!UICONTROL Change Objective Name]** de objectieve naam in.

         De objectieve naam wordt weergegeven in de lijst [!UICONTROL Custom Goals] in Advertising Cloud DSP-pakketinstellingen.

      1. Eigenschappen koppelen aan het doel:

         >[!NOTE]
         >
         > Alle transactieeigenschappen die voor de adverteerder worden gevolgd worden door gebrek vermeld in [!UICONTROL Available Properties] lijst.

         * Als u een CSV-bestand met eigenschappen en hun gewichten wilt importeren, klikt u op **[!UICONTROL Import]** en zoekt u het bestand dat u wilt importeren.

            De geïmporteerde eigenschappen moeten al bestaan voor de adverteerder; de namen zijn niet hoofdlettergevoelig.

            De geïmporteerde eigenschappen vervangen de bestaande opgegeven eigenschappen.

         * Als u de eerste eigenschap handmatig wilt opgeven met de standaarddikte (1), selecteert u een optie in een lijst met alle transactieeigenschappen die voor de adverteerder worden bijgehouden.

         * Als u handmatig een andere eigenschap met de standaarddikte (1) wilt toevoegen, klikt u op **[!UICONTROL +]**.

            >[!TIP]
            >
            > Als u naar een eigenschap in de lijst wilt zoeken, voert u een tekenreeks in vanuit de naam van de eigenschap.

         * Als u handmatig meerdere eigenschappen wilt toevoegen, klikt u op **[!UICONTROL Add Multiple Properties].** Klik voor elke eigenschap die u wilt toevoegen op de naam van de eigenschap in de  [!UICONTROL Available Properties] kolom en sleep deze naar de  [!UICONTROL Added Properties] kolom. Wanneer u klaar bent met het toevoegen van eigenschappen, klikt u op **[!UICONTROL Add]**.

            >[!TIP]
            >
            >* Als u naar een eigenschap in de lijst wilt zoeken, voert u in het invoerveld een tekenreeks in vanuit de naam van de eigenschap.
            >* Als u de lijst wilt filteren om eigenschappen uit te sluiten die zijn uitgesloten in rapporten, selecteert u de optie **[!UICONTROL Hide properties excluded from reports].**


         * (Als de doelstelling meerdere eigenschappen bevat) Als u het gewicht van een eigenschap wilt wijzigen ten opzichte van de andere eigenschappen in de doelstelling, voert u waarden in in het veld **[!UICONTROL Weight]**.
      1. Klik onder aan de instellingen op **[!UICONTROL Save]**.


Zodra u een doel creeert, kunt u het aan een pakket van Advertising Cloud DSP als douanedoel toewijzen wanneer het optimalisatiedoel &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot;of &quot;[!UICONTROL Lowest CPA - Custom Goal]&quot; is.

>[!TIP]
>
>Voor geoptimaliseerde <!-- optimum? Or optimization won't happen at all w/out it? -->prestaties, moeten de gecombineerde metriek in het douanedoel (doelstelling) in totaal minstens 10 omzettingen per dag omvatten. Als dat niet het geval is, kunt u het beste aanvullende ondersteunende gebeurtenissen (transactieeigenschappen), zoals productpagina&#39;s of toepassingen, aan het doel toevoegen. Zie [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md) voor richtlijnen.

>[!MORELIKETHIS]
>
>* [Aangepaste doelen](custom-goal-about.md)
>* [Beste praktijken voor het Bouwen van een Doel van de Douane](custom-goal-best-practices.md)
>* [Optimalisatiedoelstellingen en hoe deze te gebruiken](optimization-goals.md)
>* [Pakketinstellingen](/help/dsp/campaign-management/packages/package-settings.md)
> * [Hoe DSP uw campagnes optimaliseert](optimization-how-dsp-optimizes-campaigns.md)

