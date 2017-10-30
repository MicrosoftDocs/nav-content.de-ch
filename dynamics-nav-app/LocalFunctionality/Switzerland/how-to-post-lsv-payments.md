---
title: Buchen von LSV+-Zahlungen
description: "Zahlungen können nach Empfang einer LSV+ (Lastschrift Verfahren)-Zahlungsanzeige von der Bank gebucht werden."
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
ms.openlocfilehash: 895dedf4b86157dca24b1107495df2047135fd67
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-lsv-payments"></a>Gewusst wie: Buchen von LSV+-Zahlungen
Zahlungen können nach Empfang einer LSV+ (Lastschrift Verfahren)-Zahlungsanzeige von der Bank gebucht werden.  
  
### <a name="to-post-lsv-payments"></a>So buchen Sie LSV+-Zahlungen  
  
1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und öffnen **Zlg.-Eing. Erfassungsjournale**. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie das erforderliche Journal aus, und wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Erf.-Journal bearbeiten**.  
  
    > [!NOTE]  
    >  Sie können den Erf.-Journalnamen für LSV auswählen, wo das betreffende Gegenkonto definiert ist. Es kann jeweils nur eine LSV-Journalzeile in ein Zahlungseingangs Erf.-Journal importiert werden. Weitere Informationen finden Sie im Fenster "Zahlungseingangs Erf.-Journal".  
  
3.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Aus LSV Journal abrufen** aus.  
  
4.  Wählen Sie im Fenster **LSV-Journal Liste** die LSV-Journalzeile aus, die Sie in das Zahlungseingangs Erf.-Journal importieren möchten.  
  
    > [!NOTE]  
    >  Es können nur Erf.-Journalzeilen importiert werden, in denen das Feld **LSV-Status** auf **Datei erstellt** festgelegt ist.  
  
5.  Wählen Sie die Schaltfläche **OK** aus.  
  
     Die LSV-Journalzeile wird in das Zahlungseingangs Erf.-Journal importiert. Der Wert im Feld **LSV-Status** im Fenster **LSV-Journal Liste** ändert sich von **Datei erstellt** in **Beendet**.  
  
     Sie können die importierten Zahlungen überprüfen und sie mit der Bankzahlungsanzeige im Fenster **Zahlungseingangs Erf.-Journal** vergleichen. Sie können auch die Zahlungszeilen löschen, die von der Bank nicht verarbeitet werden konnten und für die Sie sich manuell mit dem Debitor in Verbindung setzen müssen.  
  
6.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Buchen** die Option **Buchen** aus.  
  
## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md)   
 [Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md)   
 [Gewusst wie: Abschliessen eines LSV-Einzugs](how-to-close-an-lsv-collection.md)   
 [Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md)   
 Zahlungseingangs Erf.-Journal   
 LSV Journal   
 LSV-Journalzeile
