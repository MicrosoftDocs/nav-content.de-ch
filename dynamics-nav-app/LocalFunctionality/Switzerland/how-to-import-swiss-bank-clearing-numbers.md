---
title: Importieren von Bankenclearing-Nummern (Schweiz)
description: "Bankenclearingnummern sind eindeutige Nummern zur Kennzeichnung der einzelnen Bankagenturen oder Filialen im Bankenstamm. Diese Informationen sind Voraussetzung für elektronische Zahlung. Die Datei kann auf der Website von [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121) heruntergeladen werden."
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
ms.openlocfilehash: a45e794b745e76444b20b2fa953434517302d7ae
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-import-swiss-bank-clearing-numbers"></a>Gewusst wie: Importieren von Bankenclearing-Nummern (Schweiz)
Bankenclearingnummern sind eindeutige Nummern zur Kennzeichnung der einzelnen Bankagenturen oder Filialen im Bankenstamm. Diese Informationen sind Voraussetzung für elektronische Zahlung. Die Datei kann auf der Website von [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121) heruntergeladen werden.  
  
 Die BC-Bankstammdatei – die offizielle Schweizer Bankenclearingnummer-Datei – kann importiert werden, um die Bankenclearingnummer-Informationen im Bankenstamm zu aktualisieren. Wenn Sie die Bankenclearingnummer-Datei importieren, werden die Daten in die Tabelle **Bankenstamm** importiert, und die vorhandenen Daten werden überschrieben. Nach dem Importieren der Bankenclearingnummer-Datei können Sie die aktualisierte Bankfilialnummer für Debitoren und Kreditoren definieren. Weitere Informationen finden Sie in den Tabellen "Debitor Bankkonto" und "Kreditor Bankkonto".  
  
### <a name="to-import-swiss-bank-clearing-numbers"></a>So importieren Sie Bankenclearingnummern für Schweiz  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), und öffnen Sie **Bankenstamm**. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Bankenstamm einlesen** aus.  
  
3.  Aktivieren Sie im Fenster **Bankenstamm einlesen** auf dem Inforegister **Optionen** das Feld **Clearingnummern automatisch aktualisieren**, um die Bankenclearingnummern automatisch zu aktualisieren.  
  
4.  Klicken Sie auf die Schaltfläche **Drucken** oder auf **Seitenansicht**, um die Bankenclearingnummern zu importieren, und suchen Sie anschliessend im Fenster **Öffnen** die Datei, die Sie von der Website von SIX Interbank Clearing heruntergeladen haben. Wählen Sie die Schaltfläche **Öffnen** aus.  
  
     Falls Sie die Schaltfläche **Drucken** wählen, werden die Inhalte der Datei gedruckt. Falls Sie auf die Schaltfläche **Seitenansicht** klicken, wird die Tabelle **Bankenstamm** aktualisiert und ein Bericht, dessen Clearingnummern geändert wurden, wird angezeigt.  
  
 Nachfolgend wird beschrieben, wie Bankfilialnummern für Debitorenbankkonten definiert werden. Diese Schritte gelten jedoch auch für die Definition von Bankfilialnummern für Kreditorenbankkonten.  
  
### <a name="to-define-bank-branch-numbers-for-customer-bank-accounts"></a>So definieren Sie Bankfilialnummern für Debitorenbankkonten  
  
1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und öffnen **Kunden**. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Wählen Sie den Debitor aus, für den Sie Bankkontoinformationen erstellen möchten, und wählen Sie auf der Registerkarte **Navigieren** in der Gruppe **Debitor** **Bankkonten** aus.  
  
3.  Wählen Sie im Fenster **Debitor Bankkontenliste** das erforderliche Bankkonto aus, und wählen Sie auf der Registerkarte **Start** **Bearbeiten** aus.  
  
4.  Wählen Sie auf dem Inforegister **Allgemein** im Feld **BLZ** die Nummer der Bankagentur oder -filiale aus.  
  
5.  Wählen Sie die Schaltfläche **OK** aus.  
  
## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md)   
 Bankenstamm   
 Debitor Bankkonto   
 Kreditor Bankkonto   
 [Vorgehensweise: Einrichten von Kreditorbankkonten](how-to-set-up-vendor-bank-accounts.md)
