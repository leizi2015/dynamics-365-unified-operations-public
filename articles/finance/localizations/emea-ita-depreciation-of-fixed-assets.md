---
title: Manual depreciation of fixed assets for Italy
description: This article provides information about fixed assets depreciation for legal entities in Italy.
author: AdamTrukawka
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.region: Italy
ms.author: atrukawk
ms.search.validFrom: 2016-05-31
ms.dyn365.ops.version: AX 7.0.1
ms.custom: 264294
ms.search.form: AssetDepreciationProfile, LedgerJournalTransApprove, LedgerJournalTransAsset, LedgerJournalTransDaily, LedgerJournalTransVendInvoice, PurchTable
---

# Manual depreciation of fixed assets for Italy

[!include [banner](../includes/banner.md)]

This article provides information about fixed assets depreciation for legal entities in Italy. 

For legal entities in Italy, the manual depreciation method has additional functionality that includes the following fields:

- <strong>Calculation basis</strong> -** <strong>This field has two options: **Days</strong> or <strong>Months</strong> on the <strong>Depreciation profiles</strong> page. Fixed assets depreciation is calculated for the year as follows:
  -   Days depreciation = Full years depreciation \* (number of days remaining/total days in the year)
  -   Months depreciation = Full years depreciation \* (number of months remaining/12)
- **Depreciation run date** - This field was added to the following pages:
  -   General journal
  -   Fixed asset journal
  -   Invoice approval journal
  -   Invoice journal
  -   Purchase order

The **Depreciation run date** should be set up at the time of acquisition and is set to the system date during the acquisition. The **Depreciation run date** is used to calculate depreciation for the **Number of days remaining** or **Number of Months remaining**, depending on the **Calculation basis** value. If the **Depreciation run date** is before the middle of the month (either the 15th or 14th for February), then the current month is included in number of months, otherwise the asset is considered as acquired in the next month.





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
