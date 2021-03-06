---
title: "Release notes for Data Investigations (Preview) in Microsoft 365"
ms.author: markjjo
author: markjjo
manager: laurawi
ms.date: 
ms.audience: Admin
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
ms.collection: 
search.appverid: 
- MOE150
- MET150
ms.assetid: 

description: "This article describes the new version of Advanced eDiscovery (Preview) in Microsoft 365."
---

# Release notes for Data Investigations (Preview) in Microsoft 365

You can use the new Data Investigations (Preview) tool in in Microsoft 365 to triage, investigate, and remediate data related incidents, such as a data spillage incident or an internal investigation. The Public Preview of Data investigations provides you with early access to the upcoming functionality and updates. To get early access to the newest features, create a new investigation in Data investigations (Preview) in the Office 365 Security & Compliance Center. To learn how, see [Manage a data spillage incident in Microsoft 365](manage-data-spillage-incidents.md).

## What’s new 

- **Investigations** - You can group searches and incidents by creating an investigation. Manage who can access the investigation by adding or removing members.  You can also select and mark your favorite investigations. Track and monitor activity within and across investigations using new dashboards. After you complete your investigation, you can close or delete it.

- **People of interest** – When you add users to investigations as people of interest, you can see their mailbox, OneDrive for Business account, and Microsoft Teams sites. You can use them to scope your investigative content searches. To further investigate a person of interest, you can also view audit records related to their activities in Office 365 and other Microsoft services.

- **Searches** – Create a organization-wide search using various search condition. If you know users or sites that you want to search, you can do so by adding those users as people of interest or specifying site locations in search creation wizard. 

- **Incidents** – Create a new incident and add search results that you want to review. You can review individual documents, annotate to leave investigation notes, and export results to move to a different environment. 

- **Review** – Use a native, text, and near-native view to review the documents added to an incident. You can also apply analytics to documents to group items by duplicates, email threads, and themes, which can help assist your review of the incident. 

- **Redact, tag, and annotate** – Redact text, apply tags, and make annotations as you review documents.
  
- **Deep indexing** – If there are any partially indexed items, they will be re-indexed on demand so that all data will be available for searching.

- **Error remediation** – Remediate or download processing errors. This includes remediation support for large file types, password protected files, and other issues related to indexing errors. 

- **Jobs** – Track status of long-running processes.

- **Hard-delete mailbox items** - In urgent situations, you might need to permanently delete misplaced items. To do this, you can run the **New-ComplianceSearchAction -Purge -PurgeType HardDelete** command in Security & Compliance Center PowerShell to permanently remove items from mailboxes. For more information, see [New-ComplianceSearchAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-compliancesearchaction).
