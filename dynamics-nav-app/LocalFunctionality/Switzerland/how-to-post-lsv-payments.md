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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 628c8e23bbd6cdd1dd518d57eb05b1be6f1245fa
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-post-lsv-payments"></a>Gewusst wie: Buchen von LSV+-Zahlungen
Zahlungen können nach Empfang einer LSV+ (Lastschrift Verfahren)-Zahlungsanzeige von der Bank gebucht werden.  

## <a name="to-post-lsv-payments"></a>So buchen Sie LSV+-Zahlungen  

1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Barbeleg-Buchblatt** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie das entsprechende Journal aus und wählen Sie dass **Journal bearbeiten** aus.  

    > [!NOTE]  
    >  Sie können den Erf.-Journalnamen für LSV auswählen, wo das betreffende Gegenkonto definiert ist. Es kann jeweils nur eine LSV-Journalzeile in ein Zahlungseingangs Erf.-Journal importiert werden. Weitere Informationen finden Sie im Fenster "Zahlungseingangs Erf.-Journal".  

3.  Wählen Sie die Aktion **von LSV-Erf.-Journal abrufen** aus.  
4.  Wählen Sie im Fenster **LSV-Journal Liste** die LSV-Journalzeile aus, die Sie in das Zahlungseingangs Erf.-Journal importieren möchten.  

    > [!NOTE]  
    >  Es können nur Erf.-Journalzeilen importiert werden, in denen das Feld **LSV-Status** auf **Datei erstellt** festgelegt ist.  

5.  Wählen Sie die Schaltfläche **OK** aus.  

    Die LSV-Journalzeile wird in das Zahlungseingangs Erf.-Journal importiert. Der Wert im Feld **LSV-Status** im Fenster **LSV-Journal Liste** ändert sich von **Datei erstellt** in **Beendet**.  

    Sie können die importierten Zahlungen überprüfen und sie mit der Bankzahlungsanzeige im Fenster **Zahlungseingangs Erf.-Journal** vergleichen. Sie können auch die Zahlungszeilen löschen, die von der Bank nicht verarbeitet werden konnten und für die Sie sich manuell mit dem Debitor in Verbindung setzen müssen.  

6.  Wählen Sie die Aktion **Buchen** aus.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md)   
 [Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md)   
 [Gewusst wie: Abschliessen eines LSV-Einzugs](how-to-close-an-lsv-collection.md)   
 [Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md) 

