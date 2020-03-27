---
title: "Work with environments in Microsoft Forms Pro | MicrosoftDocs"
description: "Learn about working with environments in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/02/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 90EFF51F-36E3-4973-8768-82F12629B0B3
ms.custom: 
search.appverid:
  - FPR160
---

# Work with environments

An environment is a space to store, manage, and share your organization's business data, apps, and flows. It also serves as a container to separate apps that might have different roles, security requirements, or target audiences. More information: [Environments overview](https://docs.microsoft.com/power-platform/admin/environments-overview)

You can create environments for different purposes such as survey development, testing, and production. After developing and testing the survey, you can copy the survey to the production environment.

When you sign in to Microsoft Forms Pro, only the surveys that are available in the selected environment are displayed. When you create a survey, the survey is connected to the selected environment and isn't available in other environments. The invitations and responses are stored in the same environment in which the survey was created.

You can switch the environment at any time and start working in it. You can also copy a survey from one environment to another. When you copy a survey to another environment, only the survey structure and its branching rules are copied&mdash;invitations, responses, and associated flows aren't copied.

To work with surveys in an environment, install the [Forms Pro app from Microsoft AppSource](https://appsource.microsoft.com/product/dynamics-365/mscrm.shimla?tab=Overview), and assign the Survey Owner role to users. If you switch to an environment that doesn't have Forms Pro, an error message is displayed.

> [!NOTE]
> - If you have organizations for Dynamics 365 Sales, Customer Service, Marketing, and Talent, Forms Pro entities are already installed in these organizations.
> - If you choose to work with the default environment, there are a few limitations to it. For information on limitations, see [Service Protection API Limits](https://docs.microsoft.com/powerapps/developer/common-data-service/api-limits).

## Privileges required

- Ensure that you've assigned the Survey Owner role to users.
- If you've created any custom entities that you want Forms Pro to interact with, assign the **Append To** privilege of the entities to the user.

In this section, you'll learn how to:

- [Change an environment](change-environment.md)
- [Copy a survey to another environment](copy-survey-environment.md)

