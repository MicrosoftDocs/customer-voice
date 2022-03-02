---
title: "Frequently asked questions | MicrosoftDocs"
description: "Use this topic to know about the frequently asked questions and their answers in Dynamics 365 Customer Voice."
ms.date: 03/02/2022
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

## What happens if the project owner leaves the organization?

If the project owner leaves the organization, the project will be deleted once the user is removed from the organization. If the project was shared by the user before leaving the organization, the existing user, with whom the project is shared, must create a [copy of the project](manage-projects.md#copy-a-project) and use the copied project.

## What languages are supported for sentiment analysis?

Dynamics 365 Customer Voice supports the following languages for sentiment analysis:

|     Language                 |     Language code    |
|------------------------------|------------------------|
|     Chinese                  |     zh                 |
|     Chinese-Simplified       |     zh-hans            |
|     Chinese-Traditional      |     zh-hant            |
|     Dutch                    |     nl                 |
|     English                  |     en                 |
|     French                   |     fr                 |
|     German                   |     de                 |
|     Hindi                    |     hi                 |
|     Italian                  |     it                 |
|     Japanese                 |     ja                 |
|     Korean                   |     ko                 |
|     Norwegian (Bokmål)       |     no                 |
|     Portuguese (Brazil)      |     pt-BR              |
|     Portuguese (Portugal)    |     pt-PT              |
|     Portuguese               |     pt                 |
|     Spanish                  |     es                 |
|     Turkish                  |     tr                 |
|||

Survey responses received in languages other than the ones specified above are considered as English and sent to the cognitive services for further processing. In this case, the accuracy would be impacted.

## I deleted the old surveys and survey responses, and want to update values in the satisfaction metrics report accordingly.

This is an unsupported scenario. Deleting old surveys and survey responses will not update values in the satisfaction metrics report.

## I want to delete multiple responses from the Dynamics 365 Customer Voice interface.

Deleting multiple responses from the Dynamics 365 Customer Voice interface is not supported.

## I restored Microsoft Dataverse and want Dynamics 365 Customer Voice and survey responses to work with it.

This is an unsupported scenario.

## How can I share new feature requirements or ideas?

You can share your new feature requirements or ideas on the [Customer Voice Ideas](https://aka.ms/customervoiceideas) page.


[!INCLUDE[footer-include](includes/footer-banner.md)]
