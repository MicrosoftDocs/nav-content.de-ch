---
title: 'Exemplarische Vorgehensweise: Kommissionierung und Lieferung in Basis-Lagerkonfigurationen'
description: "In  [!INCLUDE[d365fin](includes/d365fin_md.md)]  können die ausgehenden Prozesse für die Komissionierung und Lieferung auf vier Arten, mit den verschiedenen Funktionen, abhängig von der Lagerkomplexitätsebene, ausgeführt werden."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce9d58f93edeebd4933a532deb7c4672ced6f76a
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a>Exemplarische Vorgehensweise: Kommissionierung und Lieferung in Basis-Lagerkonfigurationen
In [!INCLUDE[d365fin](includes/d365fin_md.md)] können die ausgehenden Prozesse für die Komissionierung und Lieferung auf vier Arten, mit den verschiedenen Funktionen, abhängig von der Lagerkomplexitätsebene, ausgeführt werden.  

|Art|Eingangsprozess|Lagerplätze|Kommissionierungen|Lieferungen|Komplexitätsebene anzeigen (siehe [Designdetails: Lagerhaus-Einrichtung](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Beitragsentnahme und -Lieferung aus der Auftragszeile|X|||2|  
|B|Buchen Sie die Kommissionierung und den Warenausgang aus einem Lagerkommissionierungsbeleg||X||3|  
|L|Buchen Sie die Kommissionierung und den Warenausgang aus einem Warenausgangsbeleg|||X|4/5/6|  
|T|Buchen Sie die Kommissionierung von einem Kommissionierbeleg und buchen Sie den Warenausgang aus einem Warenausgangsbeleg||X|X|4/5/6|  

Weitere Informationen finden Sie unter [Designdetails: Ausgehender Lagerfluss](design-details-outbound-warehouse-flow.md).  

In der folgenden Vorgehensweise wird Methode B in der vorhergegangenen Tabelle beschrieben.  

## <a name="about-this-walkthrough"></a>Informationen zu dieser exemplarischen Vorgehensweise  
Bei Basis-Lagerkonfigurationen gilt Folgendes: Wenn ein Lagerort so eingerichtet wurde, dass Kommissionierung erforderlich ist, jedoch Warenausgang nicht erforderlich ist, verwenden Sie das Fenster **Lagerkommissionierung**, um Kommissionier- und Warenausgangsinformationen für Ihre Herkunftsbelege zu erfassen und zu buchen. Der ausgehende Herkunftsbeleg kann ein Verkaufsauftrag, eine Einkaufsreklamation, ein ausgehender Umlagerungsauftrag, ein Fertigungsauftrag oder ein Komponentenbedarf sein.  

In dieser exemplarischen Vorgehensweise werden folgende Aufgaben erläutert:  

-   Einrichtung des SILBERNEN Lagerorts für Lagerkommissionierung.  
-   Erstellen eines Verkaufsauftrags für den Debitor 10000 für 30 Lautsprecher.  
-   Freigeben des Verkaufsauftrags für Lagerdurchlaufzeit.  
-   Erstellen einer Lagerkommissionierung basierend auf einem freigegebenen Herkunftsbeleg.  
-   Erfassen der Lagerplatzumlagerung aus dem Lager und gleichzeitig Buchen der Verkaufslieferung für den ursprünglichen Verkaufsauftrag.  

## <a name="roles"></a>Rollen  
Die Aufgaben in dieser Demonstration werden von den folgenden Benutzerrollen ausgeführt:  

-   Lagerortleiter  
-   Auftragsverarbeitung  
-   Lagermitarbeiter  

## <a name="prerequisites"></a>Voraussetzungen  
Für diese exemplarische Vorgehensweise gelten folgende Voraussetzungen:  

-   CRONUS International Ltd. installiert.  
-   Machen Sie sich anhand der nachfolgenden Schritte zu einem Lagermitarbeiter am Standort SILVER:  

    1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Lagerhaus-Mitarbeiter** ein. Wählen Sie dann den zugehörigen Link aus.  
    2.  Wählen Sie das Feld **Benutzer-ID** aus, und wählen Sie Ihr eigenes Benutzerkonto im Fenster **Benutzer** aus.  
    3.  Geben Sie im Feld **Lagerortcode** SILVER ein.  
    4.  Wählen Sie das Feld **Standard** aus.  

-   Stellen Sie Artikel LS-81 am SILBERNEN Lagerort bereit, indem Sie die folgenden Schritte ausführen:  

    1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Fibu Buchblatt** ein und wählen den zugehörenden Link aus.  
    2.  Öffnen Sie das Stand Erf.-Journal, und erstellen Sie dann zwei Artikel Erfassungsjournalzeilen mit den folgenden Informationen über das Arbeitsdatum (23. Januar).  

        |Postentyp|Artikelnummer|Lagerortcode|Lagerplatzcode|Menge|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |Zugang|LS-81|SILBER|S-01-0001 **Hinweis:**  Der Standardlagerplatz des Artikels in CRONUS .|20|  
        |Zugang|LS-81|SILBER|S-01-0002|20|  

    3.  Wählen Sie die Aktion **Beleg buchen**aus und wählen Sie dann die Schaltfläche **Ja** aus.  

## <a name="story"></a>Hintergrund  
Ellen, die Lagermanagerin bei CRONUS, richtet das SILBER-Lager für grundlegende Komissionierungshandlung ein, in dem Lagermitarbeiter ausgehende Aufträge einzeln verarbeiten. Martha, die Verkaufsauftragsbearbeiterin, erstellt einen Verkaufsauftrag für 30 Einheiten des Artikels LS-81, die dem Debitor 10000 aus dem SILBERNEN Lager geliefert werden. John, der Lagermitarbeiter muss sicherstellen, dass die Lieferung an den Debitor vorbereitet und geliefert wird. John verwaltet alle beteiligten Aufgaben in Fenster **Lagerkommissionierung**, das automatisch auf die Lagerplätze verweist, in denen LS-81 gespeichert wird.  

## <a name="setting-up-the-location"></a>Einrichten des Lagerorts  
Das Einrichten des Fensters **Standortkarte** definiert die Warenflüsse des Unternehmens.  

### <a name="to-set-up-the-location"></a>So richten Sie den Lagerort ein  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie die SILBERNE Lagerortkarte.  
3.  Aktivieren Sie das Kontrollkästchen **Kommissionierung erforderlich**  

## <a name="creating-the-sales-order"></a>Erstellen des Verkaufsauftrags  
Verkaufsaufträge sind die häufigste Art des ausgehenden Herkunftsbelegs.  

### <a name="to-create-the-sales-order"></a>So erstellen Sie den Verkaufsauftrag  
1.  Alternativ wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Verkaufsauftrag** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Neu** aus.  
3.  Erstellen Sie einen Verkaufsauftrag für den Kreditor 10000 auf das Arbeitsdatum (23. Januar) mit den folgenden Verkaufszeilen.  

    |Artikel|Lagerortcode |Menge|  
    |----------|-------------------|--------------|  
    |LS_81|SILBER|30|  

     Fahren Sie fort, das Lager zu informieren, dass die Verkaufsbestellung in Lagerdurchlaufzeit bereit ist, wenn die Lieferung eingeht.  

4.  Wählen Sie die Aktion **Freigabe** aus.  

    John fährt fort, die Verkaufsartikel zu kommissionieren und zu liefern.  

## <a name="picking-and-shipping-items"></a>Kommissionierung und Versand von Artikeln  
Im Fenster **Lagerkommissionierung** können Sie alle ausgehenden Lageraktivitäten für einen bestimmten Herkunftsbeleg, wie einen Verkauf, verwalten.  

### <a name="to-pick-and-ship-items"></a>So kommissionieren Sie Artikel und liefern diese aus  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerkommissionierung** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Neu** aus.  
3.  Wählen Sie das Feld **Quellendokument** , und wählen Sie **Verkaufsauftrag** aus.  
4.  Wählen Sie das Feld **Herkunftsnr.** aus, wählen Sie die Zeile für den Verkauf an Debitor 10000 aus, und wählen Sie dann die Schaltfläche **OK**.  

    Alternativ auf der Registerkarte Aktionen, in der Gruppe Funktion, wählen Sie **Herkunftsbeleg holen** und wählen Sie die Auftrag aus.  
5.  Wählen Sie die **Die zu verarbeitende Menge automatisch ausfüllen** Aktion aus.  

    Alternativ im Feld **Menge zu verarbeiten**geben Sie 10 und 30 jeweils auf den zwei Lagerkommissionierzeilen ein.  
6.  Wählen Sie die Aktion **Buchen** und **Versand** und klicken Sie anschließend auf die Schaltfläche **OK**.  

    Die 30 Lautsprecher werden nun erfasst, wie von den Lagerplätzen S-01-0001 und S-01-0002 kommissioniert, und ein negativer Lagerposten wird, die gebuchte Verkaufslieferung reflektierend, erstellt.  

## <a name="see-also"></a>Siehe auch  
 [So wird's gemacht: Artikel mit der Lagerkommissionierung kommissionieren](warehouse-how-to-pick-items-with-inventory-picks.md)   
 [Vorgehensweise: Kommissionieren von Artikeln für den Warenausgang](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
 [Vorgehensweise: Einrichten von Basislagern mit Vorgangsbereichen](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Vorgehensweise: Umlagern von Komponenten in einen Arbeitsgangbereich in Basis-Lagerkonfigurationen](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Vorgehensweise: Kommissionierung für die Produktion oder Montage](warehouse-how-to-pick-for-production.md)   
 [Vorgehensweise: Ad-hoc-Umlagerung von Artikeln in Basis-Lagerkonfigurationen](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Designdetails: Ausgehender Lagerfluss](design-details-outbound-warehouse-flow.md)   
 [Exemplarische Vorgehensweisen für Geschäftsprozesse](walkthrough-business-process-walkthroughs.md)  
 [Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

