---
title: "Survey invitation settings in Microsoft Forms Pro | MicrosoftDocs"
description: "Instructions for updating survey invitation settings in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/21/2019
ms.service: forms-pro 
ms.topic: article
ms.assetid: 1f6ec6f5-b3d2-4305-8dca-3a0b67a1083c
ms.custom: 
---

# Define who can respond to a survey 

[!include[cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

You can create two types of surveys:

-   External surveys to get responses from customers on things like case resolutions or order closures.

-   Internal surveys to get responses about internal organization events such as an outing.

For external surveys:

1. Select **Settings** ![Settings](media/settings-icon.png "Settings") from the upper-right corner of the page.
2. Select **Anyone with the link can respond**. When you select this option, respondents are not required to sign in with their credentials.
3. Optionally, you can select one of the following options:
    - **Record name**: Respondent's name is recorded.
    - **One response per person**: A respondent can submit only one response. This option is enabled only when **Record name** is selected.

    ![Invitation settings for external surveys](media/invite-settings-external.png "Invitation settings for external surveys")

For internal surveys:

1. Select **Settings** ![Settings](media/settings-icon.png "Settings") from the upper-right corner of the page.
2. Select **Only people in my organization can respond**. When you select this option, respondents are required to sign in with their credentials. 
3. Optionally, you can select one of the following options:
    - **Record name**: Respondent's name is recorded.
    - **One response per person**: A respondent can submit only one response.

    ![Invitation settings for internal surveys](media/invite-settings-internal.png "Invitation settings for internal surveys")

When you've defined who can respond to your survey, you can select the following options:

- **Accept responses**: Specify whether the survey is open and accepting responses. By default, this option is selected. If you want to stop your survey, clear the option, and specify a message for the recipients.
- **Start date**: Specify a date when the survey will be open. 
- **End date**: Specify a date when the survey will be closed.
- **Shuffle questions**: Specify whether the questions in the survey should be shuffled.
- **Email notification of each response**: Specify whether email notification is required when a response is submitted.

    ![Response options for surveys](media/invite-settings-options.png "Response options for surveys")

> [!NOTE]
> - Currently for this preview, you can't change the settings for **Anyone with the link can respond.** It is always set to **Record name**, which records respondents names.
> - You can modify the authentication settings at any time, even after distributing the survey by email or other channels.
> - Anyone with the link address is able to see and complete your survey. Be sure you're comfortable sharing the contents before changing this default option.

