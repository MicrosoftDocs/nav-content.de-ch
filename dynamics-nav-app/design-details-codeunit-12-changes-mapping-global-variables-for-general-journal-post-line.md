---
title: "Designdetails – Codeunit 12 Änderungen im Zuordnen von globalen Variablen für Fibu Erf.-Journal-Beitrags-Zeile"
description: "Die folgenden Änderungen wurden in dieser Version von [!INCLUDE[d365fin](includes/d365fin_md.md)] implementiert."
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
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e993e36da687b10fb5f91e96f0ed34c288530202
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a><span data-ttu-id="e0252-103">Codeunit 12 Änderungen: Zuordnen der globalen Variablen für Fibu Erf.-Journal-Beitrags-Zeile</span><span class="sxs-lookup"><span data-stu-id="e0252-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>
<span data-ttu-id="e0252-104">Die folgenden Änderungen wurden in dieser Version von [!INCLUDE[d365fin](includes/d365fin_md.md)] implementiert.</span><span class="sxs-lookup"><span data-stu-id="e0252-104">The following changes have been implemented in this release of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

|<span data-ttu-id="e0252-105">**Microsoft Dynamics NAV 2009 R2**</span><span class="sxs-lookup"><span data-stu-id="e0252-105">**Microsoft Dynamics NAV 2009 R2**</span></span>|<span data-ttu-id="e0252-106">**Microsoft Dynamics NAV 2013 R2**</span><span class="sxs-lookup"><span data-stu-id="e0252-106">**Microsoft Dynamics NAV 2013 R2**</span></span>|<span data-ttu-id="e0252-107">**Bemerkung**</span><span class="sxs-lookup"><span data-stu-id="e0252-107">**Comment**</span></span>|  
|----------------------------------------|----------------------------------------|-----------------|  
|<span data-ttu-id="e0252-108">GLSetup@1009Datensatz 98:</span><span class="sxs-lookup"><span data-stu-id="e0252-108">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="e0252-109">GLSetup@1009Datensatz 98:</span><span class="sxs-lookup"><span data-stu-id="e0252-109">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="e0252-110">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-110">Unchanged</span></span>|  
|<span data-ttu-id="e0252-111">SalesSetup@1010Datensatz 311:</span><span class="sxs-lookup"><span data-stu-id="e0252-111">SalesSetup@1010 : Record 311;</span></span>||<span data-ttu-id="e0252-112">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-112">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-113">PurchSetup@1011Datensatz 312:</span><span class="sxs-lookup"><span data-stu-id="e0252-113">PurchSetup@1011 : Record 312;</span></span>||<span data-ttu-id="e0252-114">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-114">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-115">AccountingPeriod@1012Datensatz 50:</span><span class="sxs-lookup"><span data-stu-id="e0252-115">AccountingPeriod@1012 : Record 50;</span></span>||<span data-ttu-id="e0252-116">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-116">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-117">GLAcc@1013Datensatz 15:</span><span class="sxs-lookup"><span data-stu-id="e0252-117">GLAcc@1013 : Record 15;</span></span>||<span data-ttu-id="e0252-118">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-118">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-119">GLEntry@1014Datensatz 17:</span><span class="sxs-lookup"><span data-stu-id="e0252-119">GLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="e0252-120">GlobalGLEntry@1014Datensatz 17:</span><span class="sxs-lookup"><span data-stu-id="e0252-120">GlobalGLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="e0252-121">Umbenannt</span><span class="sxs-lookup"><span data-stu-id="e0252-121">Renamed</span></span>|  
|<span data-ttu-id="e0252-122">GLEntryTmp@1015 : TEMPORÄRER Datensatz 17;</span><span class="sxs-lookup"><span data-stu-id="e0252-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e0252-123">TempGLEntryBuf@1010 : TEMPORÄRER Datensatz 17;</span><span class="sxs-lookup"><span data-stu-id="e0252-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e0252-124">Umbenannt</span><span class="sxs-lookup"><span data-stu-id="e0252-124">Renamed</span></span>|  
|<span data-ttu-id="e0252-125">TempGLEntryVAT@1016 : TEMPORÄRER Datensatz 17;</span><span class="sxs-lookup"><span data-stu-id="e0252-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e0252-126">TempGLEntryVAT@1016 : TEMPORÄRER Datensatz 17;</span><span class="sxs-lookup"><span data-stu-id="e0252-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e0252-127">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-127">Unchanged</span></span>|  
|<span data-ttu-id="e0252-128">OrigGLEntry@1017Datensatz 17:</span><span class="sxs-lookup"><span data-stu-id="e0252-128">OrigGLEntry@1017 : Record 17;</span></span>||<span data-ttu-id="e0252-129">Gelöscht</span><span class="sxs-lookup"><span data-stu-id="e0252-129">Deleted</span></span>|  
|<span data-ttu-id="e0252-130">VATPostingSetup@1019Datensatz 325:</span><span class="sxs-lookup"><span data-stu-id="e0252-130">VATPostingSetup@1019 : Record 325;</span></span>||<span data-ttu-id="e0252-131">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-131">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-132">Cust@1020Datensatz 18:</span><span class="sxs-lookup"><span data-stu-id="e0252-132">Cust@1020 : Record 18;</span></span>||<span data-ttu-id="e0252-133">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-133">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-134">Vend@1021Datensatz 23:</span><span class="sxs-lookup"><span data-stu-id="e0252-134">Vend@1021 : Record 23;</span></span>||<span data-ttu-id="e0252-135">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-135">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-136">GenJnlLine@1022Datensatz 81:</span><span class="sxs-lookup"><span data-stu-id="e0252-136">GenJnlLine@1022 : Record 81;</span></span>||<span data-ttu-id="e0252-137">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-137">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-138">GLReg@1029Datensatz 45:</span><span class="sxs-lookup"><span data-stu-id="e0252-138">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="e0252-139">GLReg@1029Datensatz 45:</span><span class="sxs-lookup"><span data-stu-id="e0252-139">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="e0252-140">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-140">Unchanged</span></span>|  
|<span data-ttu-id="e0252-141">CustPostingGr@1030Datensatz 92:</span><span class="sxs-lookup"><span data-stu-id="e0252-141">CustPostingGr@1030 : Record 92;</span></span>||<span data-ttu-id="e0252-142">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-142">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-143">VendPostingGr@1031Datensatz 93:</span><span class="sxs-lookup"><span data-stu-id="e0252-143">VendPostingGr@1031 : Record 93;</span></span>||<span data-ttu-id="e0252-144">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-144">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-145">Currency@1032Datensatz 4:</span><span class="sxs-lookup"><span data-stu-id="e0252-145">Currency@1032 : Record 4;</span></span>||<span data-ttu-id="e0252-146">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-146">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-147">AddCurrency@1033Datensatz 4:</span><span class="sxs-lookup"><span data-stu-id="e0252-147">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="e0252-148">AddCurrency@1033Datensatz 4:</span><span class="sxs-lookup"><span data-stu-id="e0252-148">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="e0252-149">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-149">Unchanged</span></span>|  
|<span data-ttu-id="e0252-150">ApplnCurrency@1034Datensatz 4:</span><span class="sxs-lookup"><span data-stu-id="e0252-150">ApplnCurrency@1034 : Record 4;</span></span>||<span data-ttu-id="e0252-151">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-151">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-152">CurrExchRate@1035Datensatz 330:</span><span class="sxs-lookup"><span data-stu-id="e0252-152">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="e0252-153">CurrExchRate@1035Datensatz 330:</span><span class="sxs-lookup"><span data-stu-id="e0252-153">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="e0252-154">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-154">Unchanged</span></span>|  
|<span data-ttu-id="e0252-155">VATEntry@1038Datensatz 254:</span><span class="sxs-lookup"><span data-stu-id="e0252-155">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="e0252-156">VATEntry@1038Datensatz 254:</span><span class="sxs-lookup"><span data-stu-id="e0252-156">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="e0252-157">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-157">Unchanged</span></span>|  
|<span data-ttu-id="e0252-158">BankAcc@1039Datensatz 270:</span><span class="sxs-lookup"><span data-stu-id="e0252-158">BankAcc@1039 : Record 270;</span></span>||<span data-ttu-id="e0252-159">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-159">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-160">BankAccLedgEntry@1040Datensatz 271:</span><span class="sxs-lookup"><span data-stu-id="e0252-160">BankAccLedgEntry@1040 : Record 271;</span></span>||<span data-ttu-id="e0252-161">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-161">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-162">CheckLedgEntry@1041Datensatz 272:</span><span class="sxs-lookup"><span data-stu-id="e0252-162">CheckLedgEntry@1041 : Record 272;</span></span>||<span data-ttu-id="e0252-163">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-163">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-164">CheckLedgEntry2@1042Datensatz 272:</span><span class="sxs-lookup"><span data-stu-id="e0252-164">CheckLedgEntry2@1042 : Record 272;</span></span>||<span data-ttu-id="e0252-165">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-165">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-166">BankAccPostingGr@1043Datensatz 277:</span><span class="sxs-lookup"><span data-stu-id="e0252-166">BankAccPostingGr@1043 : Record 277;</span></span>||<span data-ttu-id="e0252-167">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-167">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-168">GenJnlTemplate@1044Datensatz 80:</span><span class="sxs-lookup"><span data-stu-id="e0252-168">GenJnlTemplate@1044 : Record 80;</span></span>||<span data-ttu-id="e0252-169">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-169">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-170">TaxJurisdiction@1045Datensatz 320:</span><span class="sxs-lookup"><span data-stu-id="e0252-170">TaxJurisdiction@1045 : Record 320;</span></span>||<span data-ttu-id="e0252-171">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-171">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-172">TaxDetail@1046Datensatz 322:</span><span class="sxs-lookup"><span data-stu-id="e0252-172">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="e0252-173">TaxDetail@1046Datensatz 322:</span><span class="sxs-lookup"><span data-stu-id="e0252-173">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="e0252-174">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-174">Unchanged</span></span>|  
|<span data-ttu-id="e0252-175">FAGLPostBuf@1047 : TEMPORÄRER Datensatz 5637;</span><span class="sxs-lookup"><span data-stu-id="e0252-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span></span>||<span data-ttu-id="e0252-176">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-176">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-177">UnrealizedCustLedgEntry@1084Datensatz 21:</span><span class="sxs-lookup"><span data-stu-id="e0252-177">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="e0252-178">UnrealizedCustLedgEntry@1084Datensatz 21:</span><span class="sxs-lookup"><span data-stu-id="e0252-178">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="e0252-179">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-179">Unchanged</span></span>|  
|<span data-ttu-id="e0252-180">UnrealizedVendLedgEntry@1085Datensatz 25:</span><span class="sxs-lookup"><span data-stu-id="e0252-180">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="e0252-181">UnrealizedVendLedgEntry@1085Datensatz 25:</span><span class="sxs-lookup"><span data-stu-id="e0252-181">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="e0252-182">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-182">Unchanged</span></span>|  
|<span data-ttu-id="e0252-183">GLEntryVATEntryLink@1087Datensatz 253:</span><span class="sxs-lookup"><span data-stu-id="e0252-183">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="e0252-184">GLEntryVATEntryLink@1087Datensatz 253:</span><span class="sxs-lookup"><span data-stu-id="e0252-184">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="e0252-185">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-185">Unchanged</span></span>|  
|<span data-ttu-id="e0252-186">TempVATEntry@1088 : TEMPORÄRER Datensatz 254;</span><span class="sxs-lookup"><span data-stu-id="e0252-186">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="e0252-187">TempVATEntry@1088 : TEMPORÄRER Datensatz 254;</span><span class="sxs-lookup"><span data-stu-id="e0252-187">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="e0252-188">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-188">Unchanged</span></span>|  
|<span data-ttu-id="e0252-189">ReversedGLEntryTemp@1089 : TEMPORÄRER Datensatz 17;</span><span class="sxs-lookup"><span data-stu-id="e0252-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span></span>||<span data-ttu-id="e0252-190">Verschoben zu Codeunit17</span><span class="sxs-lookup"><span data-stu-id="e0252-190">Moved to Codeunit17</span></span>|  
|<span data-ttu-id="e0252-191">CostAccSetup@1092Datensatz 1108:</span><span class="sxs-lookup"><span data-stu-id="e0252-191">CostAccSetup@1092 : Record 1108;</span></span>||<span data-ttu-id="e0252-192">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-192">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-193">GenJnlCheckLine@1048: Codeunit11;</span><span class="sxs-lookup"><span data-stu-id="e0252-193">GenJnlCheckLine@1048 : Codeunit 11;</span></span>|<span data-ttu-id="e0252-194">GenJnlCheckLine@1001Codeunit11;</span><span class="sxs-lookup"><span data-stu-id="e0252-194">GenJnlCheckLine@1001 : Codeunit 11;</span></span>|<span data-ttu-id="e0252-195">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-195">Unchanged</span></span>|  
|<span data-ttu-id="e0252-196">ExchAccGLJnlLine@1049: Codeunit366;</span><span class="sxs-lookup"><span data-stu-id="e0252-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span></span>||<span data-ttu-id="e0252-197">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-197">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-198">FAJnlPostLine@1050 : Codeunit 5632;</span><span class="sxs-lookup"><span data-stu-id="e0252-198">FAJnlPostLine@1050 : Codeunit 5632;</span></span>||<span data-ttu-id="e0252-199">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-199">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-200">SalesTaxCalculate@1051 : Codeunit 398;</span><span class="sxs-lookup"><span data-stu-id="e0252-200">SalesTaxCalculate@1051 : Codeunit 398;</span></span>||<span data-ttu-id="e0252-201">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-201">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-202">GenJnlApply@1052 : Codeunit 225;</span><span class="sxs-lookup"><span data-stu-id="e0252-202">GenJnlApply@1052 : Codeunit 225;</span></span>||<span data-ttu-id="e0252-203">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-203">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-204">DimMgt@1053 : Codeunit 408;</span><span class="sxs-lookup"><span data-stu-id="e0252-204">DimMgt@1053 : Codeunit 408;</span></span>||<span data-ttu-id="e0252-205">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-205">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-206">JobPostLine@1028 : Codeunit 1001;</span><span class="sxs-lookup"><span data-stu-id="e0252-206">JobPostLine@1028 : Codeunit 1001;</span></span>||<span data-ttu-id="e0252-207">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-207">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span><span class="sxs-lookup"><span data-stu-id="e0252-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span></span>||<span data-ttu-id="e0252-209">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-209">Changed to Local</span></span>|  
||<span data-ttu-id="e0252-210">PaymentToleranceMgt@1002 : Codeunit 426;</span><span class="sxs-lookup"><span data-stu-id="e0252-210">PaymentToleranceMgt@1002 : Codeunit 426;</span></span>|<span data-ttu-id="e0252-211">Teil(e) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e0252-211">Added</span></span>|  
||<span data-ttu-id="e0252-212">AddCurrencyCode@1117: Code[10];</span><span class="sxs-lookup"><span data-stu-id="e0252-212">AddCurrencyCode@1117 : Code[10];</span></span>|<span data-ttu-id="e0252-213">Teil(e) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e0252-213">Added</span></span>|  
|<span data-ttu-id="e0252-214">FiscalYearStartDate@1054 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-214">FiscalYearStartDate@1054 : Date;</span></span>|<span data-ttu-id="e0252-215">FiscalYearStartDate@1011 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-215">FiscalYearStartDate@1011 : Date;</span></span>|<span data-ttu-id="e0252-216">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-216">Unchanged</span></span>|  
|<span data-ttu-id="e0252-217">NextEntryNo@1055: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-217">NextEntryNo@1055 : Integer;</span></span>|<span data-ttu-id="e0252-218">NextEntryNo@1022: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-218">NextEntryNo@1022 : Integer;</span></span>|<span data-ttu-id="e0252-219">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-219">Unchanged</span></span>|  
|<span data-ttu-id="e0252-220">BalanceCheckAmount@1056Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-220">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="e0252-221">BalanceCheckAmount@1056Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-221">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="e0252-222">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-222">Unchanged</span></span>|  
|<span data-ttu-id="e0252-223">BalanceCheckAmount2@1057Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-223">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="e0252-224">BalanceCheckAmount2@1057Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-224">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="e0252-225">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-225">Unchanged</span></span>|  
|<span data-ttu-id="e0252-226">BalanceCheckAddCurrAmount@1058Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="e0252-227">BalanceCheckAddCurrAmount@1058Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="e0252-228">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-228">Unchanged</span></span>|  
|<span data-ttu-id="e0252-229">BalanceCheckAddCurrAmount2@1059Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="e0252-230">BalanceCheckAddCurrAmount2@1059Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="e0252-231">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-231">Unchanged</span></span>|  
|<span data-ttu-id="e0252-232">CurrentBalance@1060Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-232">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="e0252-233">CurrentBalance@1060Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-233">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="e0252-234">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-234">Unchanged</span></span>|  
|<span data-ttu-id="e0252-235">SalesTaxBaseAmount@1061Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-235">SalesTaxBaseAmount@1061 : Decimal;</span></span>||<span data-ttu-id="e0252-236">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-236">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-237">TotalAddCurrAmount@1062 Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-237">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="e0252-238">TotalAddCurrAmount@1062 Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-238">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="e0252-239">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-239">Unchanged</span></span>|  
|<span data-ttu-id="e0252-240">TotalAmount@1063Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-240">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="e0252-241">TotalAmount@1063Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-241">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="e0252-242">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-242">Unchanged</span></span>|  
|<span data-ttu-id="e0252-243">UnrealizedRemainingAmountCust@1086Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="e0252-244">UnrealizedRemainingAmountCust@1086Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="e0252-245">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-245">Unchanged</span></span>|  
|<span data-ttu-id="e0252-246">UnrealizedRemainingAmountVend@1074Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="e0252-247">UnrealizedRemainingAmountVend@1074Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="e0252-248">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-248">Unchanged</span></span>|  
|<span data-ttu-id="e0252-249">NextVATEntryNo@1064: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-249">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="e0252-250">NextVATEntryNo@1064: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-250">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="e0252-251">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-251">Unchanged</span></span>|  
|<span data-ttu-id="e0252-252">FirstNewVATEntryNo@1065: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-252">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="e0252-253">FirstNewVATEntryNo@1065: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-253">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="e0252-254">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-254">Unchanged</span></span>|  
|<span data-ttu-id="e0252-255">NextTransactionNo@1066: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-255">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="e0252-256">NextTransactionNo@1066: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-256">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="e0252-257">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-257">Unchanged</span></span>|  
|<span data-ttu-id="e0252-258">NextConnectionNo@1067: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-258">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="e0252-259">NextConnectionNo@1067: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-259">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="e0252-260">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-260">Unchanged</span></span>|  
|<span data-ttu-id="e0252-261">InsertedTempGLEntryVAT@1068: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-261">InsertedTempGLEntryVAT@1068 : Integer;</span></span>|<span data-ttu-id="e0252-262">InsertedTempGLEntryVAT@1027: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-262">InsertedTempGLEntryVAT@1027 : Integer;</span></span>|<span data-ttu-id="e0252-263">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-263">Unchanged</span></span>|  
|<span data-ttu-id="e0252-264">LastDocNo@1069: Code[20];</span><span class="sxs-lookup"><span data-stu-id="e0252-264">LastDocNo@1069 : Code[20];</span></span>|<span data-ttu-id="e0252-265">LastDocNo@1023: Code[20];</span><span class="sxs-lookup"><span data-stu-id="e0252-265">LastDocNo@1023 : Code[20];</span></span>|<span data-ttu-id="e0252-266">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-266">Unchanged</span></span>|  
|<span data-ttu-id="e0252-267">LastLineNo@1070: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-267">LastLineNo@1070 : Integer;</span></span>||<span data-ttu-id="e0252-268">Gelöscht</span><span class="sxs-lookup"><span data-stu-id="e0252-268">Deleted</span></span>|  
|<span data-ttu-id="e0252-269">LastDate@1071 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-269">LastDate@1071 : Date;</span></span>|<span data-ttu-id="e0252-270">LastDate@1021 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-270">LastDate@1021 : Date;</span></span>|<span data-ttu-id="e0252-271">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-271">Unchanged</span></span>|  
|<span data-ttu-id="e0252-272">LastDocType@1072 Rechnung, Zahlung, Gutschrift, Zinsrechnung oder Mahnung.</span><span class="sxs-lookup"><span data-stu-id="e0252-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="e0252-273">LastDocType@1025 Rechnung, Zahlung, Gutschrift, Zinsrechnung oder Mahnung.</span><span class="sxs-lookup"><span data-stu-id="e0252-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="e0252-274">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-274">Unchanged</span></span>|  
|<span data-ttu-id="e0252-275">NextCheckEntryNo@1073: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-275">NextCheckEntryNo@1073 : Integer;</span></span>|<span data-ttu-id="e0252-276">NextCheckEntryNo@1028: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-276">NextCheckEntryNo@1028 : Integer;</span></span>|<span data-ttu-id="e0252-277">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-277">Unchanged</span></span>|  
|<span data-ttu-id="e0252-278">AddCurrGLEntryVATAmt@1075Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span></span>|<span data-ttu-id="e0252-279">AddCurrGLEntryVATAmt@1017Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span></span>|<span data-ttu-id="e0252-280">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-280">Unchanged</span></span>|  
|<span data-ttu-id="e0252-281">CurrencyDate@1076 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-281">CurrencyDate@1076 : Date;</span></span>|<span data-ttu-id="e0252-282">CurrencyDate@1020 : Datum;</span><span class="sxs-lookup"><span data-stu-id="e0252-282">CurrencyDate@1020 : Date;</span></span>|<span data-ttu-id="e0252-283">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-283">Unchanged</span></span>|  
|<span data-ttu-id="e0252-284">CurrencyFactor@1077Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-284">CurrencyFactor@1077 : Decimal;</span></span>|<span data-ttu-id="e0252-285">CurrencyFactor@1019Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-285">CurrencyFactor@1019 : Decimal;</span></span>|<span data-ttu-id="e0252-286">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-286">Unchanged</span></span>|  
|<span data-ttu-id="e0252-287">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-287">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="e0252-288">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-288">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="e0252-289">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-289">Unchanged</span></span>|  
|<span data-ttu-id="e0252-290">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-290">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="e0252-291">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-291">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="e0252-292">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-292">Unchanged</span></span>|  
|<span data-ttu-id="e0252-293">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-293">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="e0252-294">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-294">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="e0252-295">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-295">Unchanged</span></span>|  
|<span data-ttu-id="e0252-296">AllApplied@1081 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-296">AllApplied@1081 : Boolean;</span></span>||<span data-ttu-id="e0252-297">Geändert zu lokal</span><span class="sxs-lookup"><span data-stu-id="e0252-297">Changed to Local</span></span>|  
|<span data-ttu-id="e0252-298">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-298">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="e0252-299">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-299">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="e0252-300">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-300">Unchanged</span></span>|  
|<span data-ttu-id="e0252-301">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-301">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="e0252-302">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-302">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="e0252-303">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-303">Unchanged</span></span>|  
|<span data-ttu-id="e0252-304">Prepayment@1037 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-304">Prepayment@1037 : Boolean;</span></span>||<span data-ttu-id="e0252-305">Gelöscht</span><span class="sxs-lookup"><span data-stu-id="e0252-305">Deleted</span></span>|  
|<span data-ttu-id="e0252-306">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-306">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="e0252-307">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-307">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="e0252-308">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-308">Unchanged</span></span>|  
|<span data-ttu-id="e0252-309">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-309">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="e0252-310">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-310">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="e0252-311">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-311">Unchanged</span></span>|  
|<span data-ttu-id="e0252-312">GLEntryNo@1090: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-312">GLEntryNo@1090 : Integer;</span></span>|<span data-ttu-id="e0252-313">GLEntryNo@1026: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-313">GLEntryNo@1026 : Integer;</span></span>|<span data-ttu-id="e0252-314">Nicht geändert</span><span class="sxs-lookup"><span data-stu-id="e0252-314">Unchanged</span></span>|  
||<span data-ttu-id="e0252-315">GLSetupRead@1015 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e0252-315">GLSetupRead@1015 : Boolean;</span></span>|<span data-ttu-id="e0252-316">Teil(e) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e0252-316">Added</span></span>|  
||<span data-ttu-id="e0252-317">AmountRoundingPrecision@1012Dezimal;</span><span class="sxs-lookup"><span data-stu-id="e0252-317">AmountRoundingPrecision@1012 : Decimal;</span></span>|<span data-ttu-id="e0252-318">Teil(e) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e0252-318">Added</span></span>|  
||<span data-ttu-id="e0252-319">CrCardTransactionEntryNo@1013: Integer;</span><span class="sxs-lookup"><span data-stu-id="e0252-319">CrCardTransactionEntryNo@1013 : Integer;</span></span>|<span data-ttu-id="e0252-320">Teil(e) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e0252-320">Added</span></span>|  

## <a name="see-also"></a><span data-ttu-id="e0252-321">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e0252-321">See Also</span></span>  
 [<span data-ttu-id="e0252-322">Designdetails: Codeunit 12 Änderungen: Änderungen in Fibu Erf.-Journal-Beitrags-Verfahren</span><span class="sxs-lookup"><span data-stu-id="e0252-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)
