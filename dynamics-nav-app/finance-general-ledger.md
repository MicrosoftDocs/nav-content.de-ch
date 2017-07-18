---
title: Die Fibuposten und der Kontenplan
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: de-ch
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Die Fibuposten und der Kontenplan
Die Fibuposten speichern Ihre Finanzdaten, und der Kontenplan zeigt die Konten, auf die alle Fibuposten gebucht werden, an. Dynamics NAV umfasst einen Standardkontenplan, der zur Unterstützung Ihres Unternehmens bereit steht.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Fibuposten Einrichtung und Buchungsmatrix Einrichtung
Im Zentrum Ihrer Geschäftsprozesse stehen die Fibuposten und wie Buchungen von Daten im Fibuposten konfiguriert werden sollen.
Im Fenster **Finanzbuchhaltung Einrichtung** geben Sie an, wie bestimmte finanzbuchhalterische Sachverhalte in Ihrem Unternehmen gehandhabt werden sollen. Dies beinhaltet Details zur Rechnungsrundung, Adressformate, und ob Sie beispielsweise eine zusätzliche Berichtswährung verwenden wollen.
Ebenso geben Sie im Fenster **Buchungsmatrix Einrichtung** an, wie Sie Kombinationen aus Geschäftsbuchungsgruppen und Produktbuchungsgruppen einrichten wollen. Für jede Kombination aus Geschäftsbuchungsgruppe und Produktbuchungsgruppe geben Sie eine Zeile ein.  

## <a name="the-chart-of-accounts"></a>Kontenplan
Der Kontenplan zeigt alle Konten an. Hier können Sie verschiedene Berichte öffnen, die Ihre Fibuposten und Salden anzeigen, und Sie können eine Erfolgsrechnung-Kontennullstellung durchführen. Für jedes Konto können Sie die Fibukontokarte öffnen und Einstellungen hinzufügen oder ändern. Sie können außerdem eine Liste von Buchungsgruppen anzeigen, die auf dieses Konto buchen.  

Dynamics NAV verhindert, dass Sie einen Fipuposten löschen, in dem Daten gespeichert werden, die im Kontenplan erforderlich sind.  

## <a name="account-categories"></a>Kontokategorien
Mit Kontokategorien können Sie Fibukonten Kategorien zuordnen und so die Struktur Ihrer Finanzberichte anpassen.  

Das Fenster **Fibukontokategorien** zeigt Ihre vorhandenen Haupt- und Unterkategorien und die Fibukonten an, die Sie jeder Kategorie zugeordnet haben. Sie können neue Unterkategorien erstellen und diese bestehenden Konten zuweisen.  

Sie können die Kontenkategorien gruppieren, indem Sie einzelne Unterkategorien einrücken. Dieses erleichtert Ihnen den Überblick, da jede Gruppierung einen Gesamtsaldo anzeigt. Beispielsweise können Sie Unterkategorien für unterschiedliche Arten von Anlagen erstellen und dann Kategoriengruppen für Anlagen gegenüber Umlaufvermögen erstellen. Sie erstellen eine Kategoriengruppe, indem Sie weitere Unterkategorien unter einer Zeile im Fenster **Fibukontokategorien** einrücken.  

Für jede Unterkategorie können Sie festlegen, ob Konten dieser Kategorie in bestimmte Arten von Finanzberichten enthalten sein müssen. Die Kontengruppen helfen Ihnen dabei, das Layout Ihrer Finanzberichte zu definieren. Beispielsweise gibt es in der Standardsaldoabrechnung einen einzigen Posten für Zahlungen unter Anlagen. Wenn die Saldoabrechnung Untereinträge für Handkasse und Girokonto haben soll, können Sie zwei neue Unterkategorien hinzufügen, die zusätzliche Berichtsdefinition "Bargeldkonto" für jede festlegen und sie unter der Bargeldunterkategorie einrücken. Wenn Sie ein Kontenschema auf Grundlage Ihre Änderungen erstellt haben, wird die nächste Saldoabrechnung ein Gesamtsaldo für Zahlungen und zwei Zeilen mit Salden für Handgeld und das Girokonto anzeigen.     

##<a name="see-also"></a>Siehe auch
[Finanzen](finance-setup.md)  
[Einrichten oder Ändern des Kontenplans](finance-setup-setup-chart-accounts.md)  
[Kontenschemata](finance-setup-account-schedule.md)  

