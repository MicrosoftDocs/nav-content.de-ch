---
title: 'Vorgehensweise: Umstrukturieren von Lagern'
description: "Es kann sein, dass Sie Ihr Lager neu strukturieren und dabei neue Lagerplatzcodes und Eigenschaften von Zonen berücksichtigen möchten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 852aa1a36b150d13d763e2c398265b9eaec5c3ea
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-restructure-warehouses"></a>Vorgehensweise: Umstrukturieren von Lagern
Es kann sein, dass Sie Ihr Lager neu strukturieren und dabei neue Lagerplatzcodes und Eigenschaften von Zonen berücksichtigen möchten. Diese Art von Aktivität werden Sie nicht oft ausführen. Es können jedoch Situationen auftreten, in denen eine Neustrukturierung notwendig ist, um effektivere Arbeitsabläufe zu erreichen. Beispiel:  

- Sie möchten zu Lagerplatzcodes übergehen, die die Verwendung der mobilen Datenerfassung unterstützen, z. B. mit tragbaren Geräten.  
- Für das Lager wurde ein neues Regalsystem angeschafft, dass Ihnen neue Möglichkeiten der Lagerung bietet.  
- Das Unternehmen hat sein Produktsortiment geändert und das Lager an einen neuen Ort verlagert, um sich diesen Veränderungen anzupassen.  

Wenn Ihr Lager so eingerichtet wurde, dass es Lagerplätze verwendet, aber keine gesteuerte Einlagerung und Kommissionierung, strukturieren Sie Ihr Lager neu, indem Sie die neuen Lagerplätze erstellen, die Sie zukünftig verwenden möchten.  

## <a name="to-restructure-a-basic-warehouse-that-uses-bins-only"></a>Um ein Basislager neu zu strukturieren, das nur Lagerplätze verwendet  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Setzen Sie im Inforegister **Logistik** das Feld **Vorg.-Lagerplatzauswahl** auf **Zuletzt verwendeter Lagerplatz**.  
3.  Lagern Sie alle Inhalte Ihrer aktuellen Lagerplätze in die neuen Lagerplätze um, die Sie gerade angelegt haben.  

    1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Artikel Umlag. Erf.-Journal bearbeiten** ein und wählen den zugehörenden Link aus.  
    2.  Wählen Sie eine Erf.-Journalzeile aus, und wählen Sie die **Lagerplatzinhalt holen** Aktion aus.  
    3.  Legen Sie im Inforegister **Lagerplatzinhalt** in den Feldern **Lagerortcode**, **Lagerplatzcode** und **Artikelnr.** Filter fest, um den Inhalt anzugeben, den Sie umlagern möchten.  
    4.  Klicken Sie auf die Schaltfläche **OK**, um eine Erfassungsjournalzeile zu füllen.  
    5.  Wählen Sie im Feld **Neuer Lagerplatzcode** den Lagerplatz aus, in den Sie die Artikel umlagern möchten.  
    6.  Wiederholen Sie die Schritte b bis e für alle Lagerplatzinhalte, die Sie umlagern möchten.  
    7.  Wählen Sie die Aktion **Buchen** aus.  

Sie haben jetzt die Lagerplätze geleert, an denen die Artikel bisher gelagert wurden. Die Standardlagerplätze Ihrer Artikel wurden jetzt in die neuen Lagerplätze geändert.  

## <a name="to-restructure-an-advanced-warehouse-that-uses-directed-put-away-and-pick"></a>Um ein erweitertes Lager, das eine gesteuerte Einlagerung und Kommissionierung verwendet, neu zu strukturieren  

1.  Legen Sie die neuen Lagerplätze an, die Sie in Zukunft verwenden möchten. Weitere Informationen finden Sie unter [Gewusst wie: Lagerplätze erstellen](warehouse-how-to-create-individual-bins.md).  
2.  Lagern Sie alle Inhalte Ihrer aktuellen Lagerplätze in die neuen Lagerplätze um, die Sie gerade angelegt haben.  

    1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Logistik Umlagerungs Erf.-Journal** ein und wählen den zugehörenden Link aus.  
    2.  Für die Lagerplätze, bei denen keine tatsächliche Artikelumlagerung stattfindet, erstellen Sie eine Zeile für jeden der aktuellen Lagerplätze im **Logistik Umlagerungs Erfassungsjournal** mit dem alten Lagerplatzcode (**Von Lagerplatzcode**) und dem neuen Lagerplatzcode (**Nach Lagerplatzcode)**.  
    3.  Wenn einige der Umlagerungen tatsächliche physische Umlagerungen beinhalten, die die Lagermitarbeiter durchführen sollen, verwenden Sie den **Lagerplatzumlagerungsvorschlag**, um die Umlagerungsanweisungen vorzubereiten, anstatt das Umlagerungs Erfassungsjournal zu verwenden. Weitere Informationen finden Sie unter [Vorgehensweise: Umlagern von Artikeln in erweiterten Lagerkonfigurationen](warehouse-how-to-move-items-in-advanced-warehousing.md).  

3.  Wenn die alten Lagerplätze geleert sind, buchen Sie diese als Lagerplätze vom Typ **QK** um, um sicherzustellen, dass sie nicht in den Artikelströmen enthalten sind.  

    1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
    2.  Wählen Sie die Zeile mit dem Lagerort aus und wählen Sie dann Aktion **Lagerplätze** aus.  
    3.  Geben Sie im Fenster **Lagerplätze** im Feld **Lagerplatzartencode** für jeden der alten Lagerplätze, die Sie in Schritt 3 des vorherigen Verfahrens geleert haben, **QC** ein.  

Sie haben die Lagerplätze jetzt aus dem Warenfluss entfernt und sie als QC-Lagerplätze umgebucht. Qc-Lagerplätze haben im Fenster **Lagerplatzarten** keine ausgewählten Aktivitätenprotokollposten und werden daher durch den Warenfluss nicht berücksichtigt. Weitere Informationen finden Sie unter [Vorgehensweise: Einrichten von Lagerplatzarten](warehouse-how-to-set-up-bin-types.md).  

## <a name="to-delete-a-bin"></a>So löschen Sie einen Lagerplatz:  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie den Lagerort aus, an dem Sie Lagerplätze löschen möchten. Wählen Sie die **Lagerplätze** Aktion aus.  
3.  Wählen Sie die Zeilen für die zu löschenden Lagerplätze aus.  
4.  Wählen Sie die Aktion **Löschen** aus.  

Wenn Sie **Ja** wählen, wird der Lagerplatz für die zukünftige Verwendung gelöscht, der Lagerplatzcode in allen Lagerplatzposten bleibt jedoch derselbe.  

Wenn Sie einen Lagerplatz umbenennen möchten, so dass alle Datensätze zu diesem Lagerplatz ebenfalls umbenannt werden (die Datensätze umfassen Lagerplatzinhalte, Lageraktivitätszeilen, registrierte Lageraktivitätszeilen, Zeilen in Logistikvorschlägen, Wareneingangszeilen, gebuchte Wareneingangszeilen, Warenausgangszeilen, gebuchte Warenausgangszeilen sowie Lagerplatzposten), können Sie dies im Fenster **Lagerplätze** tun.  

## <a name="to-rename-a-bin-and-change-the-bin-code-in-all-records"></a>So benennen Sie einen Lagerplatz um und ändern den Lagerplatzcode in allen Datensätzen:  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie den Lagerort aus, an dem Sie einen Lagerplatz umbenennen oder für den Sie den Lagerplatzcode ändern möchten, und wählen Sie dann die Aktion **Lagerplätze** aus.  
3.  Wählen Sie den Lagerplatz aus, den Sie ändern möchten, und geben Sie im Feld **Code** einen neuen Code für den Lagerort ein.  
4.  Wählen Sie die Schaltfläche **Ja** aus.  

> [!NOTE]  
>  Wenn Sie **Ja** wählen und es viele Datensätze zu diesem Lagerplatz gibt (z. B. weil Sie lange keine Logistikbelege mehr gelöscht haben), kann es einige Zeit dauern, bis die Anwendung alle Datensätze umbenannt hat. Wenn Sie diese Methode verwenden, sollten Sie daher eventuell die Stapelverarbeitung **Registrierte Logistikbelege löschen** ausführen, bevor Sie die Umbenennung starten. Beachten Sie darüber hinaus, dass die einzigen Belege, die durch diese Stapelverarbeitung gelöscht werden, Einlagerungen, Kommissionierungen und Lagerplatzumlagerungen sind.  
>   
>  Wenn Sie einen Wareneingangslagerplatz oder einen Warenausgangslagerplatz umbenennen, müssen alle gebuchten Wareneingänge oder Warenausgänge, die sich auf den jeweiligen Lagerplatz beziehen, umbenannt werden.  

## <a name="see-also"></a>Siehe auch  
[Logistik](warehouse-manage-warehouse.md)  
[Lagerbesttand](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

