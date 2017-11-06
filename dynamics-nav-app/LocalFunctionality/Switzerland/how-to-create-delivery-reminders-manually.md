---
title: Manuelles Erstellen von Lieferbenachrichtigungen
description: In ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/how-to-generate-delivery-reminders.md).
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
ms.openlocfilehash: 8db551fa5341c6c25ad368782a4e3f3ceca95760
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-delivery-reminders-manually"></a>Gewusst wie: Manuelles Erstellen von Lieferbenachrichtigungen
In [!INCLUDE[navnow](../../includes/navnow_md.md)], können Sie Lieferbenachrichtigungen erstellen, wenn eine Bestellung nicht wie erwartet geliefert wurde. Sie können eine einzelne Lieferbenachrichtigung manuell erstellen oder Sie können Lieferbenachrichtigungen für alle überfälligen Lieferungen erstellen. Weitere Informationen finden Sie unter [Gewusst wie: Erstellen von Lieferbenachrichtigungen](how-to-generate-delivery-reminders.md).

> [!NOTE]
> Um Lieferbenachrichtigungen zu erstellen, müssen Sie die Eigenschaften für Lieferbenachrichtigungen einrichten. Weitere Informationen finden Sie unter [Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminders.md).

## <a name="to-create-a-delivery-reminder-manually"></a>So erstellen Sie eine Lieferbenachrichtigung manuell  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und öffnen die **Lieferbenachrichtigung**. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Neu** aus.  
3.  Füllen Sie im Fenster **Lieferbenachrichtigung** im Inforegister **Allgemein** die Felder gemäss der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Die eindeutige Kennnummer für die Lieferbenachrichtigung.|  
    |**Kreditorennr**|Die Nummer des Kreditors, für den Sie die Lieferbenachrichtigung buchen möchten.<br /><br /> Wenn Sie die Kreditorennummer auswählen, werden die Felder **Name**, **Adresse**, **PLZ-Code/Ort** und **Kontakt** automatisch ausgefüllt.|  
    |**Buchungsdatum**|Das Buchungsdatum für die Lieferbenachrichtigung. Dieses Datum wird in alle Lieferbenachrichtigungsposten kopiert.|  
    |**Belegdatum**|Das Belegdatum für die Lieferbenachrichtigung. Dieses Datum wird auch verwendet, um das Fälligkeitsdatum der Lieferbenachrichtigung zu berechnen. Sie können das Buchungsdatum bei Bedarf ändern.|  
    |**Mahnstufe**|Die Lieferbenachrichtigungsstufe. Dieser Wert basiert auf der Anzahl der Lieferbenachrichtigungen, die bereits gesendet wurden. Weitere Informationen finden Sie unter [Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).|  
    |**Mahnmethodencode**|Geben Sie den Lieferbenachrichtigungsmethodencode an, der für den Kreditor eingerichtet ist.|  
    |**Fälligkeitsdatum**|Das Fälligkeitsdatum für die Lieferbenachrichtigung.|  

4.  Wählen Sie die Aktion **Mahnungszeile vorschlagen**  

    Bei überfälligen Lieferungen vom angegebenen Kreditor werden diese der Lieferbenachrichtigung hinzugefügt.  

5.  Wählen Sie die Schaltfläche **OK** aus.  

    Die Lieferbenachrichtigung wird erstellt. Jetzt können Sie die Lieferbenachrichtigungen ausstellen und drucken.  

## <a name="see-also"></a>Siehe auch  
 [Lieferbenachrichtigungen](delivery-reminders.md)   
 [Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-generate-delivery-reminders.md)   
 [Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminders.md)   
 [Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md)   
 [Gewusst wie: Zuweisen von Lieferbenachrichtigungscodes zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md)   
 [Gewusst wie: Lieferbenachrichtigungen ausstellen](how-to-issue-delivery-reminders.md)   
 [Gewusst wie: Drucken von Testberichten für Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md)

