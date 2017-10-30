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
# <a name="how-to-import-swiss-bank-clearing-numbers"></a><span data-ttu-id="f9120-105">Gewusst wie: Importieren von Bankenclearing-Nummern (Schweiz)</span><span class="sxs-lookup"><span data-stu-id="f9120-105">How to: Import Swiss Bank Clearing Numbers</span></span>
<span data-ttu-id="f9120-106">Bankenclearingnummern sind eindeutige Nummern zur Kennzeichnung der einzelnen Bankagenturen oder Filialen im Bankenstamm.</span><span class="sxs-lookup"><span data-stu-id="f9120-106">Bank clearing numbers are unique numbers used to identify each bank agency or branch in the bank directory.</span></span> <span data-ttu-id="f9120-107">Diese Informationen sind Voraussetzung für elektronische Zahlung.</span><span class="sxs-lookup"><span data-stu-id="f9120-107">This information is required for electronic payment.</span></span> <span data-ttu-id="f9120-108">Die Datei kann auf der Website von [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121) heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="f9120-108">The file can be downloaded from the [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121) website.</span></span>  
  
 <span data-ttu-id="f9120-109">Die BC-Bankstammdatei – die offizielle Schweizer Bankenclearingnummer-Datei – kann importiert werden, um die Bankenclearingnummer-Informationen im Bankenstamm zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f9120-109">You can import the BC Bank Master file—the official Swiss bank clearing number file—to update the bank clearing number information in the bank directory.</span></span> <span data-ttu-id="f9120-110">Wenn Sie die Bankenclearingnummer-Datei importieren, werden die Daten in die Tabelle **Bankenstamm** importiert, und die vorhandenen Daten werden überschrieben.</span><span class="sxs-lookup"><span data-stu-id="f9120-110">When you import the bank clearing number file, the data is imported to the **Bank Directory** table, and the existing data is overwritten.</span></span> <span data-ttu-id="f9120-111">Nach dem Importieren der Bankenclearingnummer-Datei können Sie die aktualisierte Bankfilialnummer für Debitoren und Kreditoren definieren.</span><span class="sxs-lookup"><span data-stu-id="f9120-111">After importing the bank clearing number file, you can define the updated bank branch number for customers and vendors.</span></span> <span data-ttu-id="f9120-112">Weitere Informationen finden Sie in den Tabellen "Debitor Bankkonto" und "Kreditor Bankkonto".</span><span class="sxs-lookup"><span data-stu-id="f9120-112">For more information, see the Customer Bank Account table and the Vendor Bank Account table.</span></span>  
  
### <a name="to-import-swiss-bank-clearing-numbers"></a><span data-ttu-id="f9120-113">So importieren Sie Bankenclearingnummern für Schweiz</span><span class="sxs-lookup"><span data-stu-id="f9120-113">To import Swiss bank clearing numbers</span></span>  
  
1.  <span data-ttu-id="f9120-114">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), und öffnen Sie **Bankenstamm**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Directory**, and choose the related link.</span></span>  
  
2.  <span data-ttu-id="f9120-115">Wählen Sie auf der Registerkarte **Start** in der Gruppe **Vorgang** die Option **Bankenstamm einlesen** aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-115">On the **Home** tab, in the **Process** group, select **Import Bank Directory**.</span></span>  
  
3.  <span data-ttu-id="f9120-116">Aktivieren Sie im Fenster **Bankenstamm einlesen** auf dem Inforegister **Optionen** das Feld **Clearingnummern automatisch aktualisieren**, um die Bankenclearingnummern automatisch zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f9120-116">In the **Import Bank Directory** window, on the **Options** FastTab, select the **Automatically Update Clearing Numbers** field to update the bank clearing numbers automatically.</span></span>  
  
4.  <span data-ttu-id="f9120-117">Klicken Sie auf die Schaltfläche **Drucken** oder auf **Seitenansicht**, um die Bankenclearingnummern zu importieren, und suchen Sie anschliessend im Fenster **Öffnen** die Datei, die Sie von der Website von SIX Interbank Clearing heruntergeladen haben.</span><span class="sxs-lookup"><span data-stu-id="f9120-117">Choose the **Print** button or the **Preview** button to import the bank clearing numbers, and then, in the **Open** window, locate the file that you have downloaded from the SIX Interbank Clearing website.</span></span> <span data-ttu-id="f9120-118">Wählen Sie die Schaltfläche **Öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-118">Choose the **Open** button.</span></span>  
  
     <span data-ttu-id="f9120-119">Falls Sie die Schaltfläche **Drucken** wählen, werden die Inhalte der Datei gedruckt.</span><span class="sxs-lookup"><span data-stu-id="f9120-119">If you choose the **Print** button, the contents of the file will be printed.</span></span> <span data-ttu-id="f9120-120">Falls Sie auf die Schaltfläche **Seitenansicht** klicken, wird die Tabelle **Bankenstamm** aktualisiert und ein Bericht, dessen Clearingnummern geändert wurden, wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9120-120">If you choose the **Preview** button, the **Bank Directory** table will be updated and a report that has clearing numbers that have changed will be displayed.</span></span>  
  
 <span data-ttu-id="f9120-121">Nachfolgend wird beschrieben, wie Bankfilialnummern für Debitorenbankkonten definiert werden. Diese Schritte gelten jedoch auch für die Definition von Bankfilialnummern für Kreditorenbankkonten.</span><span class="sxs-lookup"><span data-stu-id="f9120-121">The following procedure describes how to define bank branch numbers for customer bank accounts, but the same steps also apply for defining bank branch numbers for vendor bank accounts.</span></span>  
  
### <a name="to-define-bank-branch-numbers-for-customer-bank-accounts"></a><span data-ttu-id="f9120-122">So definieren Sie Bankfilialnummern für Debitorenbankkonten</span><span class="sxs-lookup"><span data-stu-id="f9120-122">To define bank branch numbers for customer bank accounts</span></span>  
  
1.  <span data-ttu-id="f9120-123">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und öffnen **Kunden**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="f9120-124">Wählen Sie den Debitor aus, für den Sie Bankkontoinformationen erstellen möchten, und wählen Sie auf der Registerkarte **Navigieren** in der Gruppe **Debitor** **Bankkonten** aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-124">Select the customer for whom you want to create bank account information, and on the **Navigate** tab, in the **Customer** group, select **Bank Accounts**.</span></span>  
  
3.  <span data-ttu-id="f9120-125">Wählen Sie im Fenster **Debitor Bankkontenliste** das erforderliche Bankkonto aus, und wählen Sie auf der Registerkarte **Start** **Bearbeiten** aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-125">In the **Customer Bank Account List** window, select the required bank account, and on the **Home** tab, select **Edit**.</span></span>  
  
4.  <span data-ttu-id="f9120-126">Wählen Sie auf dem Inforegister **Allgemein** im Feld **BLZ**</span><span class="sxs-lookup"><span data-stu-id="f9120-126">On the **General** FastTab, in the **Bank Branch No.**</span></span> <span data-ttu-id="f9120-127">die Nummer der Bankagentur oder -filiale aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-127">field, select the number of the bank agency or branch.</span></span>  
  
5.  <span data-ttu-id="f9120-128">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="f9120-128">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f9120-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f9120-129">See Also</span></span>  
 <span data-ttu-id="f9120-130">[Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f9120-130">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 <span data-ttu-id="f9120-131">Bankenstamm</span><span class="sxs-lookup"><span data-stu-id="f9120-131">Bank Directory</span></span>   
 <span data-ttu-id="f9120-132">Debitor Bankkonto</span><span class="sxs-lookup"><span data-stu-id="f9120-132">Customer Bank Account</span></span>   
 <span data-ttu-id="f9120-133">Kreditor Bankkonto</span><span class="sxs-lookup"><span data-stu-id="f9120-133">Vendor Bank Account</span></span>   
 [<span data-ttu-id="f9120-134">Vorgehensweise: Einrichten von Kreditorbankkonten</span><span class="sxs-lookup"><span data-stu-id="f9120-134">How to: Set Up Vendor Bank Accounts</span></span>](how-to-set-up-vendor-bank-accounts.md)
