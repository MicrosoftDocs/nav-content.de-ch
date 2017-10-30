---
title: Exportieren von Zahlungen mit EZAG
description: "Sie können eine Datei für elektronische Zahlung mithilfe der EZAG (Elektronischer Zahlungsauftrag)-Methode generieren und sie exportieren, damit sie von der Bank für Zahlungen verwendet werden."
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
ms.openlocfilehash: b9ea004d65e3d288c1c1db9771f4ed486c9f232b
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-payments-using-ezag"></a>Gewusst wie: Exportieren von Zahlungen mit EZAG
Sie können eine Datei für elektronische Zahlung mithilfe der EZAG (Elektronischer Zahlungsauftrag)-Methode generieren und sie exportieren, damit sie von der Bank für Zahlungen verwendet werden.  
  
### <a name="to-export-payments-using-ezag"></a>So exportieren Sie Zahlungen mit EZAG  
  
1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), öffnen **Zlg.-Ausg. Erfassungsjournale** und wählen den zugehörenden Link aus.  
  
2.  Wählen Sie im Feld **Erf.-Journalname** den Erf.-Journalnamen aus.  
  
3.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **EZAG Datei schreiben** aus.  
  
4.  Füllen Sie im Stapelverarbeitungsauftrag **EZAG Datei** die Felder auf dem Inforegister **Optionen** wie in der folgenden Tabelle beschrieben aus.  
  
    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Belastung auf Bank**|Geben Sie den Code der zu belastenden Bank an.|  
    |**Sammelzahlung pro Kreditor**|Geben Sie an, ob die Zahlungszeilen in der generierten EZAG-Datei, die den gleichen Kreditor, die gleiche Währung, die gleiche Bank und die gleiche Belastungsbank besitzen, kombiniert werden sollen.|  
    |**Versand per Diskette**|Geben Sie an, ob die EZAG-Datei auf einem Datenträger gespeichert werden soll, damit Sie sie der Bank zukommen lassen können.|  
  
5.  Wählen Sie die Schaltfläche **OK** aus. Die EZAG-Datei wird generiert.  
  
## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md)   
 [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md)   
 [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md)   
 [Gewusst wie: Senden von DTA-Zahlungen](how-to-submit-dta-payments.md)   
 DTA Einrichtung   
 Zhlg.-Erf.-Journal
