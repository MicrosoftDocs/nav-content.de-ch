---
title: Abschliessen eines LSV-Einzugs
description: "LSV+ (Lastschrift Verfahren)-Einzüge müssen abgeschlossen werden, um LSV-Dateien zu schreiben, die zum Zahlungseinzug an die Bank gesendet werden können. Wenn Sie einen Einzug abschliessen, ist dieser beendet, und die Buchungen im LSV-Journal werden kombiniert."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1d63f24a50024f4561b5827f2b6b1328c207a873
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-an-lsv-collection"></a>Gewusst wie: Abschliessen eines LSV-Einzugs
LSV+ (Lastschrift Verfahren)-Einzüge müssen abgeschlossen werden, um LSV-Dateien zu schreiben, die zum Zahlungseinzug an die Bank gesendet werden können. Wenn Sie einen Einzug abschliessen, ist dieser beendet, und die Buchungen im LSV-Journal werden kombiniert.  
  
 Wenn der Einzug abgeschlossen ist, wird die aktuelle Einzugsnummer im LSV-Journal auf Grundlage des letzten Einzugs zugeordnet. Diese LSV-Nummer wird für alle ausstehenden Rechnungen an die Debitorenposten übertragen. Anhand der LSV-Nummer kann die Einzugsdatei jederzeit rekonstruiert werden. Das Feld **Abwarten** wird auch mit **LSV** in den Debitorenposten ausgefüllt, um die Duplizierung von offenen Posten zu vermeiden. Weitere Informationen finden Sie in den Tabellen **LSV Journal** und **Debitorenposten**. Ausserdem kann ein abgeschlossener Einzug auch erneut geöffnet werden.  
  
### <a name="to-close-an-lsv-collection"></a>So schliessen Sie einen LSV-Einzug  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite ober Bericht suchen"), und öffnen Sie **LSV-Journal Liste**. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie die erforderliche Erf.-Journalzeile aus, und wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Buchungsdatum korrigieren** aus. Dadurch wird der Wert im Feld **Valutadatum** geändert, indem der während des LSV-Einzugs vorgeschlagene Wert verwendet wird.  
  
3.  Geben Sie im Feld **Neues Datum** das neue Datum ein.  
  
4.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** **Einzug abschliessen** aus.  
  
    > [!NOTE]  
    >  Die Felder auf dem Inforegister **Optionen** für die Stapelverarbeitung **LSV Einzug abschliessen** können nicht geändert werden und entsprechen der ausgewählten Erf.-Journalzeile.  
  
5.  Wählen Sie die Schaltfläche **OK** aus.  
  
     Im Fenster **LSV-Journal Liste** wird der Wert im Feld **LSV-Status** von **Bearbeiten** in **Freigegeben** geändert. Die Erf.-Journalzeilen können nicht mehr geändert werden.  
  
### <a name="to-reopen-an-lsv-collection"></a>So öffnen Sie einen LSV-Einzug erneut  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite ober Bericht suchen"), und öffnen Sie **LSV-Journal Liste**. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie die erforderliche Erf.-Journalzeile aus, für die Sie den Einzug erneut öffnen möchten, wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktion** **Einzug erneut öffnen** aus.  
  
    > [!NOTE]  
    >  Der Einzug kann nur erneut geöffnet werden, wenn die LSV+-Datei noch nicht an die Bank übermittelt wurde.  
  
3.  Wählen Sie die Schaltfläche **Ja**, um das erneute Öffnen des Einzugs zu bestätigen.  
  
## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md)   
 [Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md)   
 [Gewusst wie: Buchen von LSV+-Zahlungen](how-to-post-lsv-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md)   
 LSV Journal   
 LSV-Journalzeile   
 Debitorenposten
