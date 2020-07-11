---
title: "Survey distribution settings"
description: "Instructions for updating survey distribution settings in Customer Voice to control who can respond to your survey and other survey response options"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Work with survey distribution settings

After you've created a survey, you can select distribution settings to control responses to your survey. You can choose whether anyone can respond to the survey, or only people in your organization. The former option doesn't require a respondent to sign in, whereas the latter option does require a respondent to sign in. You can also define various response and notification options.

**To update survey distribution settings**

1. Open the survey.

2. On the **Send** tab, select **Customization** at the right side of the page, and then select **Distribution**.

3. Update the settings as described in the following sections.

## Respondents

You can select the options to define who can respond to a survey, whether to anonymize responses, and more.

Consider a scenario where you've created a survey to collect customer feedback when a support case is resolved. In this scenario, you'll require feedback from the people outside your organization.

Let's consider another scenario where you've created a survey to collect feedback about an internal organization event. In this case, you'll require feedback from the people in your organization only to respond to the survey.

The available settings are:

- **Only people in my organization can respond**: Specify whether anyone with the survey link can respond to the survey or only people in an organization can respond to the survey.
    
    By default, this setting is turned off and anyone with the survey link can respond to the survey. The respondents are not required to sign in to open the survey.

    When you turn on this setting, only the respondents who are in the same organization as the survey creator can respond to the survey. It also requires a respondent to sign in to open the survey.

- **Anonymize responses**: Specify whether to record a respondent's name.

    By default, this setting is turned off and the respondent's name is recorded.
    
    When you turn on this setting, the respondent's name is not recorded. This is helpful when you want to collect survey responses anonymously.

- **One response per person**: Specify whether a respondent can submit only one response.

    By default, this setting is turned off and a respondent can submit can submit more than one response. 
    
    When you turn on this setting, a respondent can submit only one response. This setting is disabled when **Only people in my organization can respond** and **Anonymize responses** are turned off.

- **Add respondents as Contacts**: Specify whether the respondent should be added as a contact in Common Data Service.

    By default, this setting is turned on and respondents are added as a contact in Common Data Service. It works only with surveys sent through email.

## Response restrictions

You can select whether your survey is open for receiving responses and also specify a time period when to start and stop receiving responses.

The available settings are:

- **Accept responses**: Specify whether the survey is open and accepting responses. By default, this setting is turned on.

    If you want to stop receiving responses, turn off this setting and enter a message in the **Message to recipients** field. The message you enter will be shown to the respondents when they open a survey.

- **Specific time window**: Specify a time period for receiving responses. By default, it is not selected.

    When you select this option, you can specify a start date-time and end date-time for your survey. **Start date** and **Start time** denotes a date and time when a survey will be open for respondents. **End date** and **End time** denotes a date and time when the survey will stop receiving responses.
    
    This setting is displayed only when **Accept responses** is turned on. 

- **Response limit**: Specify the maximum number of responses to be received, after which the responses will no longer be counted and the survey will be stopped. By default, it is not selected.

    When you select this option, you can set the maximum number of responses to be received as per the requirement. By default, the value is set to 50,000. You can enter a value lower than the default value or up to the maximum of 50,000.

    This setting is displayed only when **Accept responses** is turned on.

## Link expirations

You can specify the number of days your survey will be open after you send the survey invitation.

The available setting is:

- **Block responses for older links**: Specify whether to block responses from older personalized links. By default, this setting is turned off.

    If you want to block responses, turn on this setting and enter the number of days in the **Disable links older than** field. By default, the value is set to 30. You can enter a value lower than the default value or up to the maximum of 1,095. Respondents can use the personalized link to complete the survey from the date they receive the invitation until the specified number of days have passed.

## Email

You can select the custom email address that you want to use for sending email. After you've set up a custom email, select it from the **Sender** list. More information on setting up a custom email: [Customize the sender's email address](send-survey-email#customize-the-senders-email-address)

## Notifications

You can set response notification options for the sender as well as the respondent.

The available settings are:

- **Send email receipt to all recipients**: Specify whether respondents should receive an email confirmation of their responses. This setting is enabled only when **Only people in my organization can respond** is turned on and **Anonymize responses** is turned off. By default, this setting is turned off.

    When you turn on this setting, your respondents will see the option **Send me an email receipt of my responses** after completing a survey. After submitting responses, respondents will then receive a confirmation email, which includes a thank-you message and link to view their responses.

- **Receive email notifications for every response**: Specify whether you need an email notification whenever a response is submitted. By default, this setting is turned off.

## Work with personalized links

Personalized survey links or trackable links are generated when a survey is sent by using the built-in email composer and Power Automate. A survey link is unique to its recipient, and helps to record the respondent's name and/or whether the respondent can submit only one response.

When you send a survey by generating a link or a QR code, the survey links aren't personalized. In these cases, you won't be able to record the respondent's name and whether the respondent has submitted only one response, if **Only people in my organization can respond** is turned off.

### See also

[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)<br>
[Administrator settings for Customer Voice](admin-settings.md)