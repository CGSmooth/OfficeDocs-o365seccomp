---
title: "Email threading"
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

description: ""
---

# Email threading

Consider an email conversation that has been going on for a while. In most cases, the last email on the thread will include the contents of all the preceding emails; reviewing the last email will give a complete context of the conversation that happened in the thread. Email threading identifies such emails so that reviewers can review a fraction of collected documents without losing any context.

## What does email threading do?

Email threading parses each email and desconstructs it to individual messages; each email is a chain of individual messages. Then, it analyzes all emails in the working set to determine whether an email has unique content or if the chain is wholly contained in a different email. In the end emails are divided into four categories:

- **Inclusive**: the last message in the email has unique content, and the email has all of the attachments that were included in other emails of which the content is wholly contained in this email.


- **Inclusive minus**: the last message in the email has unique content, but the email does not contain some of the attachments that were included in other emails of which the content is wholly contained in this email.

- **Inclusive copy**: an exact copy of an inclusive/inclusive minus email

- **None**: The content of this email is wholly contained in at least one email that is marked as inclusive/inclusive minus.

## How is it different from conversations in Outlook?
At a glance, this sounds very similar to conversation groupings in Outlook. However, there are some important distinctions. Consider an email conversation that got forked into two conversation; for instance, someone responded to an email that is not the latest in the conversation so the last two emails in the conversation both have unique content.

Outlook would still group the emails into a single conversation; reading only the last email would mean missing the context of the second-to-last email, which also contains unique content. Because email threading parses out each email into individual components and compares them, email threading would mark both of the last two emails as inclusives, ensuring that you won't miss any context as long as you read all emails marked as inclusive.