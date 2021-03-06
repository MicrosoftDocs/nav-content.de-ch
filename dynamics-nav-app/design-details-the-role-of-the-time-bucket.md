---
title: "Designdetails – Die Rolle des Zeitrahmens"
description: Der Zweck dieses Zeitrahmens ist, Bedarfsereignisse innerhalb des Zeitfensters zu erfassen, um einen gemeinsamen Beschaffungsauftrag zu erstellen.
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
ms.openlocfilehash: c05bb3ca1913b1f5d0abe0bfa26248d08e080ad6
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-time-bucket"></a>Designdetails: Die Rolle des Zeitrahmens
Der Zweck dieses Zeitrahmens ist, Bedarfsereignisse innerhalb des Zeitfensters zu erfassen, um einen gemeinsamen Beschaffungsauftrag zu erstellen.  
  
 Für Wiederbeschaffungsverfahren, die einen Minimalbestand verwenden, können Sie einen Zeitrahmen definieren. Dadurch ist sichergestellt, dass Bedarf innerhalb derselben Periode kumuliert wird, bevor die Auswirkungen auf den voraussichtlichen Lagerbestand geprüft werden, und ob der Minimalbestand unterschritten wurde. Wenn der Minimalbestand überschritten wird, wird ein neuer Beschaffungsauftrag vom Ende der durch den Zeitrahmen definierten Periode vorwärts geplant. Der Zeitrahmen beginnt am geplanten Startdatum.  
  
 Der Zeitrahmenkonzept spiegelt den manuellen Vorgang des Überprüfens des Lagerbestands auf häufiger Basis anstatt für jede Transaktion. Die Anwender muss die Häufigkeit (den Zeitrahmen) festlegen. Beispielsweise erfasst der Benutzer alle Artikelanforderungen von einem Kreditor, um einen wöchentlichen Auftrag zu platzieren.  
  
 ![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")  
  
 Das Zeitrahmen wird im Allgemeinen verwendet, um einen Kaskadeneffekt zu vermeiden. Zum Beispiel eine eine ausgeglichene Zeile von Bedarf und Vorrat, bei der ein frühzeitiger Bedarf storniert oder ein neuer Bedarf erstellt wird. Das Ergebnis würde sein, dass jeder Beschaffungsauftrag (mit Ausnahme des letzten) umgeplant würde.  
  
## <a name="see-also"></a>Siehe auch  
 [Designdetails: Wiederbeschaffungsverfahren](design-details-reordering-policies.md)   
 [Designdetails: Planungsparameter](design-details-planning-parameters.md)   
 [Designdetails: Umgang mit Wiederbeschaffungsverfahren](design-details-handling-reordering-policies.md)   
 [Designdetails: Vorratsplanung](design-details-supply-planning.md)
