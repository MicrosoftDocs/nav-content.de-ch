---
title: 'Gewusst wie: Verarbeiten eines LSV-Einzugs'
description: "Mithilfe von **LSV-Journalen** können Zahlungen von LSV+-Debitoren (Lastschriftverfahren) erstellt und verarbeitet werden. Sie können diese Zahlungen im Zahlungseingangs-Erfassungsjournal erfassen, eine LSV-Datei erstellen und dann den Einzugsauftrag drucken."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: a7503fec71d315d3a2bf4e9e1e3a734209990e14
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-process-an-lsv-collection"></a>Gewusst wie: Verarbeiten eines LSV-Einzugs
Mithilfe von **LSV-Journalen** können Zahlungen von LSV+-Debitoren (Lastschriftverfahren) erstellt und verarbeitet werden. Sie können diese Zahlungen im Zahlungseingangs-Erfassungsjournal erfassen, eine LSV-Datei erstellen und dann den Einzugsauftrag drucken. Weitere Informationen finden Sie im Fenster Zahlung von Debitoren Erf.-Journal und [Gewusst wie: Zahlungen mithilfe von LSV exportieren](how-to-export-payments-using-lsv.md).  

Wenn Sie den Stapelverarbeitungsauftrag **LSV Einzugsvorschlag** ausführen, wird jeder vorgeschlagene Einzug in einer LSV-Journalzeile erfasst, und die offenen Rechnungen werden in die LSV-Journale übertragen. Weitere Informationen finden Sie unter LSV-Erf.-Journal – Tabelle.  

Sie können die vorgeschlagenen Zahlungszeilen anzeigen, bearbeiten oder löschen. Falls Sie den vorgeschlagenen Betrag korrigieren, wird die Differenz als Rabatt markiert. Der Stapelverarbeitungsauftrag kann mehrmals für unterschiedliche Debitorengruppen ausgeführt werden. Die Vorschlagszeilen können in dasselbe Erfassungsjournal eingefügt werden.  

## <a name="to-create-an-lsv-collection"></a>So erstellen Sie einen LSV-Einzug  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite ober Bericht suchen") und geben **LSV Erf.-Journal Liste** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Neu** aus.  
3.  Füllen Sie im Fenster **LSV-Journal Liste** die erforderlichen Felder wie in der folgenden Tabelle beschrieben aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**LSV Bankcode**|Wählen Sie den LSV Bankcode für die Bank, die die Konsolidierung durchführt.|  
    |**LSV Journalbeschreibung**|Geben Sie eine Beschreibung für den Eintrag ein.|

4.  Wählen Sie den erforderlichen LSV-Journaleintrag, und wählen die Aktion **LSV Sammlung vorschlagen** aus, um die Zahlungen automatisch von LSV zu erfassen.  
5.  Füllen Sie im Fenster **LSV Einzugsvorschlag** die Felder auf dem Inforegister **Optionen** wie in der folgenden Tabelle beschrieben aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Geben Sie die LSV Erf.-Journalzeilen ein.|  
    |**Von Fälligkeitsdatum**|Geben Sie das Start- Fälligkeitsdatum von offenen Posten an, die für die Sammlung vorgeschlagen werden sollen.|  
    |**Bis Fälligkeitsdatum**|Geben Sie das End- Fälligkeitsdatum von offenen Posten an, die für die Sammlung vorgeschlagen werden sollen.|  
    |**Einzugsdatum**|Geben Sie das Datum an, an dem die Sammlung schließt. Der LSV+-Einzugsauftrag muss mindestens drei Banktage vor dem Einzugsdatum gesendet werden.|  

6.  Wählen Sie die Schaltfläche **OK** aus.  

Alle zugehörigen Zeilen werden in das LSV-Journal übertragen. Nach der Verarbeitung des LSV-Einzugs können Sie die vorgeschlagenen Zahlungen im Fenster **LSV Journal** anzeigen, überprüfen oder bearbeiten. Weitere Informationen finden Sie unter LSV-Erf.-Journal-Zeilen – Tabelle.  

## <a name="to-manage-suggested-payments"></a>So verwalten Sie vorgeschlagene Zahlungen  

1.  Im Fenster **LSV-Erf.-Journal-Liste** wählen Sie den erforderlichen Journaleintrag, und wählen die **LSV-Erf.-Journalzeile** Aktion aus.  

    Sie können die vorgeschlagenen Zahlungen in diesem Fenster anzeigen und ändern. Dieser Wert kann bei Bedarf manuell eingegeben oder geändert werden. Für neue Erfassungsjournalzeilen wird das Feld **LSV-Status** auf **Öffnen** festgelegt, um anzugeben, dass die Rechnung unbezahlt ist.  

3.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="see-also"></a>Siehe auch  
 [Schweizer Elektronische Zahlungen mithilfe von LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Gewusst wie: Abschliessen eines LSV-Einzugs](how-to-close-an-lsv-collection.md)   
 [Gewusst wie: Buchen von LSV+-Zahlungen](how-to-post-lsv-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md)

