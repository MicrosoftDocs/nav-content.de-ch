---
title: Lieferbenachrichtigungen
description: "Lieferbenachrichtigung werden verwendet, um überfällige Kreditorenlieferungen zu verfolgen und um Kreditoren an überfällige Lieferungen zu erinnern."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 263a1a00f4e0511b6e49ffb749ac06518828e30a
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="delivery-reminders"></a>Lieferbenachrichtigungen
Lieferbenachrichtigung werden verwendet, um überfällige Kreditorenlieferungen zu verfolgen und um Kreditoren an überfällige Lieferungen zu erinnern. Um Lieferbenachrichtigung zu erstellen, müssen Sie Folgendes einrichten:  

- Lieferbenachrichtigungsbestimmungen  

    Lieferbenachrichtigungsbestimmungen werden durch einen Code identifiziert, der Kreditoren zugewiesen werden muss. Wenn mehr als eine Kombination der Einstellungen verwendet werden soll, müssen Sie für jede Kombination einen eigenen Code einrichten. Sie können eine beliebige Anzahl an Lieferbenachrichtigungsbestimmungen einrichten.  

- Lieferbenachrichtigungsstufen  

    Für jede Lieferbenachrichtigungsbestimmung müssen Sie Lieferbenachrichtigungsebenen definieren. Diese Stufen legen fest, wie häufig Lieferbenachrichtigung für eine bestimmte Methode erstellt werden können. Stufe 1 ist die erste Lieferbenachrichtigung, die Sie für eine überfällige Lieferung erstellen. Stufe 2 ist die zweite Lieferbenachrichtigung und so weiter. Wenn Lieferbenachrichtigungen erstellt werden, werden die Anzahl von Mahnungen, die zuvor erzeugt wurden und die aktuelle Nummer verwendet, um Methoden anzuwenden.  

- Lieferbenachrichtigungstextnachrichten  

    Für jede Lieferbenachrichtigungstextnachricht müssen Sie Lieferbenachrichtigungsebenen definieren. Es gibt zwei Arten von Lieferbenachrichtigungstexten: Vortexte und Nachtexte. Die Vortextnachricht wird unter dem Kopfabschnitt gedruckt, vor der Liste der Posten, die zur Mahnung markiert sind. Die Nachtextnachricht wird nach dieser Liste gedruckt.  

Weitere Informationen finden Sie unter [Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).  

Nach dem Einrichten der Lieferbestimmungen müssen die Lieferbenachrichtigungsbestimmungscodes den Kreditoren zuweisen. Weitere Informationen finden Sie unter [Gewusst wie: Zuweisen von Lieferbenachrichtigungen zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md).  

Lieferbenachrichtigung können manuell oder automatisch erstellt werden. Sie können die Stapelverarbeitung **Lieferbenachrichtigung erstellen** verwenden, um Lieferbenachrichtigungen automatisch zu erstellen. Dieser Batchauftrag ermöglicht es Ihnen, die Bestellungen auszuwählen, für die Lieferbenachrichtigungen erstellt werden müssen. Weitere Informationen finden Sie unter [Gewusst wie: Erstellen von Lieferbenachrichtigungen](how-to-issue-delivery-reminders.md).  

Sie können Belege auch in Bezug auf Bestellzeilen und Verkaufsauftragszeilen nachverfolgen.  

[!INCLUDE[navnow](../../includes/navnow_md.md)] stellt die folgenden Berichte bereit:  

- **Registrierte Lieferbenachrichtigung** -, Um die Lieferbenachrichtigung für Kreditoren anzuzeigen.  
- **Lieferbenachrichtigung - Test** -, Um die Lieferbenachrichtigung zu prüfen, bevor Sie diese registrieren.  

Weitere Informationen finden Sie unter [Gewusst wie: Drucken von Testberichten für Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md).  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-set-up-delivery-reminders.md)   
 [Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md)   
 [Gewusst wie: Zuweisen von Lieferbenachrichtigungscodes zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md)   
 [Gewusst wie: Einrichten von Lieferbenachrichtigungen](how-to-generate-delivery-reminders.md)   
 [Gewusst wie: Manuelles Erstellen von Lieferbenachrichtigungen](how-to-create-delivery-reminders-manually.md)   
 [Gewusst wie: Lieferbenachrichtigungen ausstellen](how-to-issue-delivery-reminders.md)   
 [Gewusst wie: Drucken von Testberichten für Lieferbenachrichtigungen](how-to-print-test-reports-for-delivery-reminders.md)

