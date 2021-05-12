---
title: "Frequently asked questions | MicrosoftDocs"
description: "Use this topic to know about the frequently asked questions and their answers in Dynamics 365 Customer Voice."
ms.date: 04/28/2021
ms.service: dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Dynamics 365 Customer Voice FAQ

We've compiled a list of frequently asked questions and provided brief answers to help you get to your information quickly.

## I created a guest user in Azure Active Directory, but the user is unable to access Dynamics 365 Customer Voice.

Guest user access is not supported in Dynamics 365 Customer Voice. You must create a new user in your tenant and then provide access to the new user.

## How is the owner of a survey response determined?

A response owner is determined by the following logic:

- For responses to a survey invitation, the invitation owner is set as the response owner.
- If the survey invitation owner doesn't have sufficient privileges to own responses, or if the response is anonymous, the survey owner is set as the response owner.
- If the account of a survey owner has been disabled or the survey owner is unable to access the application due to licensing issues, the application user is set as the response owner.

## I deleted data from Microsoft Dataverse but it is visible in reports.

It is recommended not to delete data directly from Microsoft Dataverse. If you delete any data directly from Microsoft Dataverse, it is not synchronized with Customer Voice services. If you want to delete any data, you must delete using the Dynamics 365 Customer Voice interface.

## Why does the application user require the System Administrator role?

The application user requires the System Administrator role to associate survey invites and responses to any of the entities, including custom entities.


[!INCLUDE[footer-include](includes/footer-banner.md)]
