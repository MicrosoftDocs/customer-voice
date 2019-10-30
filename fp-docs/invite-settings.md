---
title: "Survey settings | MicrosoftDocs"
description: "Instructions for updating survey settings in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 10/30/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 1f6ec6f5-b3d2-4305-8dca-3a0b67a1083c
ms.custom: 
search.appverid:
  - FPR160
---


# Work with survey settings 

After you have created a survey, you can select settings to control the responses to your survey. You can select whether anyone can respond to the survey or only the people in your organization can respond. The former option does not require a respondent to sign in, whereas the latter option does require a respondent to sign in. You can also define various response and notification options.

## Define who can respond to a survey

Consider a scenario where you have created a survey to collect customer feedback when a support case is resolved. In this scenario, you will require feedback from the people outside of your organization. To accomplish this, you will select the option **Anyone with the link can respond** in the survey settings. More information: [Anyone with the link can respond](#anyone-with-the-link-can-respond)

Let's consider another scenario where you have created a survey to collect feedback about an internal organization event and you want only the people in your organization to respond to the survey. To accomplish this, you will select the option **Only people in my organization can respond** in the survey settings. More information: [Only people in my organization can respond](#only-people-in-my-organization-can-respond)

Let's now see the options you can select to define who can respond to a survey and select options whether to record the respondent's name and limit the respondent to submit only one response.

### Anyone with the link can respond

1. Open the survey for which you want to change survey settings.
2. Select the **ellipsis** button (…) from the toolbar at the top of the page, and then select **Settings**.
    > [!div class=mx-imgBorder]
    > ![Settings](media/settings-icon.png "Settings")
3. Select **Anyone with the link can respond**. When you select this option, respondents are not required to sign in with their credentials.
4. Optionally, you can select one or both of the following options:
    - **Record name**: Respondent's name is recorded. This option works only if a [personalized survey link](#work-with-personalized-links) is generated.
    - **One response per person**: A respondent can submit only one response. This option is enabled only when **Record name** is selected and works only if a [personalized survey link](#work-with-personalized-links) is generated.
    
    > [!div class=mx-imgBorder]
    > ![Invitation settings for external surveys](media/invite-settings-external.png "Invitation settings for external surveys")

### Only people in my organization can respond

1. Open the survey for which you want to change survey settings.
2. Select the **ellipsis** button (…) from the toolbar at the top of the page, and then select **Settings**.
    > [!div class=mx-imgBorder]
    > ![Settings](media/settings-icon.png "Settings")
3. Select **Only people in my organization can respond**. When you select this option, respondents are required to sign in with their credentials. 
4. Optionally, you can select one or both of the following options:
    - **Record name**: Respondent's name is recorded.
    - **One response per person**: A respondent can submit only one response.
    
    > [!div class=mx-imgBorder]
    > ![Invitation settings for internal surveys](media/invite-settings-internal.png "Invitation settings for internal surveys")

## Select survey response and notification options

When you've defined who can respond to your survey, you can select or clear the following options:

- **Accept responses**: Specify whether the survey is open and accepting responses. By default, it is selected. If you want to stop your survey, clear the option, and specify a message for the recipients.
- **Start date**: Specify a date when the survey will be open. 
- **End date**: Specify a date when the survey will be closed.
- **Shuffle questions**: Specify whether the questions in the survey should be shuffled.
- **Show question numbers**: Specify whether the question numbers should be displayed in the survey. By default, it is selected.
- **Customize thank you message**: Specify a customized thank you message for your responders.
- **Customize footer text**: Specify a customized footer text to be displayed for your survey.
- **Add respondents as**: Specify if the respondent should be added as a contact in Common Data Service. By default, it is selected. This option works only with surveys sent through email.
- **Send email receipt to respondents**: Specify if respondents should receive an email confirmation of their responses. This option is enabled only when **Record name** is selected under **Only people in my organization can respond**. Once your respondent has filled out your survey, the option, **Send me an email receipt of my responses**, is displayed. After submitting responses, respondents will then receive a confirmation email, which includes a thank you message and link to view their responses.
- **Get email notification of each response**: Specify if you need an email notification whenever a response is submitted.

    > [!div class=mx-imgBorder]
    > ![Response options for surveys](media/invite-settings-options.png "Response options for surveys")

You can modify the authentication settings at any time, even after distributing the survey by email or other channels.

## Work with personalized links

Personalized survey links or trackable links are generated when a survey is sent by using the built-in email composer and Microsoft Flow. A survey link is unique to its recipient and helps to record the respondent's name and/or whether the respondent must submit only one response.

When you send a survey by generating a link or a QR code, the survey links are not personalized. In these cases, you will not be able to record the respondent's name and whether the respondent has submitted only one response if you have selected **Anyone with the link can respond**.

## See also

[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Microsoft Flow](send-survey-microsoft-flow.md)<br>
[Embed survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in PowerApps](embed-survey-powerapps.md)
