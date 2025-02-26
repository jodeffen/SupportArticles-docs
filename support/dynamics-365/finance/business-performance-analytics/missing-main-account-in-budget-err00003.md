---
title: Missing main account in budget error
description: Provides information about the Missing main account in budget error (error code ERR00003) in business performance analytics in Microsoft Dynamics 365 Finance.
author: jinniew
ms.author: jiwo
ms.reviewer: twheeloc 
ms.date: 12/07/2023
ms.prod: 
ms.technology:
ms.custom:
ms.search.form: business-performance-analytics
audience: Application User
---
# Missing main account in budget: Error code: ERR00003 [Type: Warning]

> [!NOTE]
> The functionality that's described in this article is available as part of a preview release. The functionality and the content of this article are subject to change. For more information about how to participate in the public preview for [business performance analytics](/dynamics365/finance/business-performance-analytics/business-performance-analytics-home-page), contact <bpaquestions@service.microsoft.com>.

## Symptoms

Error code *ERR00003* is logged in the **Bpa self help logs** table in Microsoft Dataverse when budget transaction lines in Dynamics 365 Finance are missing the main account in the ledger dimension column. Transactions in the budget are linked to a `generalledgeraccountkey` value of **-1**.

## Resolution

If your transaction doesn't have to use the main account, this issue might not require immediate action. However, some Microsoft reports might show either fields that have no data or incomplete records. In these cases, you might have to create modified versions of the reports to address the gaps and ensure accurate reporting.

Here's an example of a record:

> 1 records in BudgetTransactionLine have missing MAINACCOUNT - [Row(BudgetTransactionLine_RECID=Decimal('5637145719'))]

> [!NOTE]
> No specific steps are required to address this scenario, and no correction is required.

## See also

[Business performance analytics self-help](business-performance-analytics-self-help-overview.md)
