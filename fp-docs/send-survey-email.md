---
title: "Send a survey by using email"
description: "Instructions for sending a survey by using email"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/24/2020
ms.service: forms-pro
ms.topic: article
ms.assetid: c5d53c06-299d-43bc-a7ac-e6185c9695e3
ms.custom: 
search.appverid:
  - FPR160
---

# Send a survey by using email

After creating a survey, you can send it through email by following these steps.

1.  Open the survey you want to send, and select **Send** from the toolbar at the top of the page. 

2. Select **Email**. A default subject line and email message appear, along with a link to your survey in the message body. You can modify and format the text to meet your requirements.

3.  In the **To** field, enter the recipient's name or email address. You can populate the **To** field by using any of the following methods:

    - Entering an email address manually.
    - Entering a name, email address, or a distribution list from Azure Active Directory.
    - Entering a contact or contact list/view from Common Data Service. The contacts are populated from the selected environment. More information: [Work with environments](choose-environment.md)
    - Uploading a CSV file by selecting **Import recipients**. The CSV file supports importing a maximum of 10,000 recipients.

4.  To insert the survey link into your email message, see [Insert a survey link](#insert-survey-link).  

5.  To add an unsubscribe link to your email message, see [Insert an unsubscribe link](#unsubscribe-from-a-survey).  

6.  To personalize the email by using survey variables, see [Personalize the survey email](#personalize-an-email).

7. To embed the first question of the survey into your email message, see [Embed a survey in an email](#embed-survey-in-an-email).

8.  To select an email template, select a template from the **Template** list. **Default Template** is selected by default. More information: [Use email templates](#use-email-templates)

9.  When you're ready to send your survey, select **Send**.

> [!NOTE]
> You can send a survey invitation to a maximum of 10,000 recipients.

<a name="insert-survey-link"></a>

## Insert a survey link

The survey link is added to your email message by default. To insert the survey link in a different location in your email message, place the cursor at the location you want, and then select **Insert** > **Survey link**. You can also select text, and then select **Insert** > **Survey link** to display that text as the survey link.

<a name="unsubscribe-from-a-survey"></a>

## Insert an unsubscribe link

You can configure your email message to include a link that allows a respondent to unsubscribe from the survey. To insert the unsubscribe link in the email message, place the cursor at the required location, and then select **Insert** > **Unsubscribe link**. You can also select text, and then select **Insert** > **Unsubscribe link** to display that text as the unsubscribe link. By default, the unsubscribe link is added to all email message templates.

<a name="personalize-an-email"></a>

## Personalize the survey email

Use survey variables to personalize your survey email&mdash;for example, you can add the respondent's first name. Place the cursor where you want the name to appear, select **Variables**, and then select **First name** from the list. The first name of the respondent will be automatically inserted. All the survey variables created in a survey are displayed in the **Variables** list.

To create a new variable, select **New variable** from the **Variables** list. If default values haven't been defined for survey variables, a warning message is displayed at the top of the page. For more information about creating variables and providing values for them, see [Personalize a survey](personalize-survey.md).

<a name="embed-survey-in-an-email"></a>

## Embed a survey in an email

If you have added a Choice (single answer), Rating (star or smiley symbol), or Net Promoter Score question as the first question in your survey, you can embed it in your email message. To embed the question, select **Embed first question**. When you embed a question, the text in the email message is replaced by the question. When a responder selects an option to answer the question, the whole survey is opened in a web browser and the responder can continue with completing the survey.

> [!div class=mx-imgBorder]
> ![Embed a survey in an email](media/embed-ques-email.png "Embed a survey in an email")

> [!NOTE]
> - You can't embed a question in an email if you have enabled question shuffling in the survey.
> - If you want to send embedded survey in an email through Power Automate, you must embed the question in an email and save it as a new email template. While configuring a flow, you must select the new email template. More information on email templates: [Use email templates](#use-email-templates)

If you've created a multilingual survey, you can use survey variables to set the default locale for displaying the survey. To set the default locale, open the **Survey variables** pane, and then specify a value for the **locale** variable. The value must be a language code, for example **en** or **fr**.

<a name="use-email-templates"></a>

## Use email templates

You can use an email template&mdash;a preformatted email message&mdash;to quickly create and send email messages. You can modify the text, and then save your changes to the current email template or save the changes to a new email template. Unless you make another selection, **Default Template** is selected for use in an email message.

You can perform these actions on an email template:

- **Save**: Save your changes to the current email template.

- **Save as**: Save your changes to a new email template.

- **Delete**: Delete the current email template.

- **Rename**: Rename the current email template.


> [!NOTE]
> - You can save a maximum of 10 email templates.
> - If an email template includes survey variables that aren't part of the survey, an error message is displayed at the top of the page and you won't be allowed to send the survey through email or Microsoft Power Automate. The survey variables will be highlighted in red; you must remove these highlighted variables from the email message before you can send the survey.

### See also

[Work with survey settings](invite-settings.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)
