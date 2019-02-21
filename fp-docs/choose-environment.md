---
title: "Choose an environment for working with Microsoft Forms Pro | MicrosoftDocs"
description: "Instructions for choosing an environment for working with Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/21/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 90EFF51F-36E3-4973-8768-82F12629B0B3
ms.custom: 
---

# Choose environment for your survey

An environment is a space to store, manage, and share your organization’s business data, apps, and flows. They also serve as containers to separate apps that may have different roles, security requirements, or target audiences. More information: [Environments overview](https://docs.microsoft.com/en-us/power-platform/admin/environments-overview)

You can create environments for different purpose. For example, you can create an environment each for survey development, testing, and production. After developing and testing the survey, you can copy the survey to the production environment. 

When you sign in to Microsoft Forms Pro, only the surveys that are available in the selected environment are displayed. When you create a survey, the survey is connected to the selected environment and is not available in other environments. The invitations and responses are stored in the same environment in which the survey is created. You can switch the environment as per your requirement and start working in it. You can also copy a survey from one environment to another.  When you copy a survey to another environment, only the survey structure and its branching rules are copied. The invitations, responses, and associated flows are not copied to another environment.

To work with surveys in an environment, you must install the Microsoft Forms Pro app from Microsoft AppSource and assign the Survey User role to the users. If you switch to an environment that doesn't have Microsoft Forms Pro, an error is displayed.

## Change an environment

By default, all environments under the tenant you are signed in are displayed. You can switch the environment as per your requirement and start working in it.
To change an environment:

1. Sign in to Microsoft Forms Pro. 
2. Select your user name from the upper-right corner of the page.
3. A list of environments are displayed under the **Environments** section.
4. Select the required environment.

## Copy survey to another environment

You can create a copy of your survey in the same environment or in another environment. To copy a survey to another environment:

1. Sign in to Microsoft Forms Pro. 

2. Find the survey you want to copy from the list of surveys and select **More form actions** (...) in the upper-right corner of the survey window. 

    ![Survey more actions](media/survey-more-actions.png "Survey more actions")

3. Select **Copy**.

    ![Survey copy action](media/survey-copy.png "Survey copy action")

    Two options are displayed for copying the survey.

4. Select **Copy to**.

    ![Survey copy options](media/survey-copy-options.png "Survey copy options")

    A list of environments are displayed in a pane on the right-side of the screen

5. Select an environment to which you want to copy the survey.


