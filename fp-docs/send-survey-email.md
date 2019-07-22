---
title: "Send a survey by using email | MicrosoftDocs"
description: "Instructions for sending a survey by using email"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 07/01/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: c5d53c06-299d-43bc-a7ac-e6185c9695e3
ms.custom: 
search.appverid:
  - FPR160
---

# Send a survey by using email



After creating a survey, you can send it through email: 

1.  Open the survey you want to send, and go to **Send Survey** &gt; **Email**. A default subject line and email message appear, along with a link to your survey in the message body. You can modify and format the text to meet your requirements.

2.  In the **To** field, enter the recipient's name or email address. You can populate the **To** field by either of the following ways:
    - Entering an email address manually.
    - Entering a name, email address, or a distribution list from Azure Active Directory.
    - Entering a contact or contact list/view from Common Data Services for Apps. The contacts are populated from the selected environment. For more information on working with environments, see: [Work with environments](choose-environment.md). 
    - Uploading a .csv file by selecting **Import recipients**.

3.  To insert the survey link into your email message, see [Insert survey link](#insert-survey-link).  

4.  To add an unsubscribe link to your email message, see [Unsubscribe from a survey](#unsubscribe-from-a-survey).  

5.  To personalize the email by using first and last names of the respondent, see [Personalize an email](#personalize-an-email).  

6.  To select an email template, select a template from the **Template** drop-down list. By default, **Default Template** is selected. More information: [Use email templates](#use-email-templates).  

7.  When you're ready to send your survey, select **Send**.

> [!NOTE]
> For this release, you can send a survey invitation to maximum 100 recipients.

## Insert survey link

The survey link is added to your email message by default. To insert the survey link in a different location in your email message, place the cursor at the required location, and select **Insert survey link**. You can also select text, and then select **Insert survey link** to display that text as the survey link.

## Unsubscribe from a survey

You can configure your email message to include a link that allows a respondent to unsubscribe from the survey. To insert the unsubscribe link in the email message, place the cursor at the required location, and then select **Insert unsubscribe link**. You can also select text, and then select **Insert unsubscribe link** to display that text as the unsubscribe link. By default, the unsubscribe link is added to all email message templates.

## Personalize an email

Personalize your survey email by using placeholders. For example, place the cursor where you want a first name to appear. Select **Personalize**, and then select **First name** from the drop-down list. The first name of the respondent will be automatically inserted. 

The following variables are available:

- **First name**: Inserts first name of the recipient.

- **Last name**: Inserts last name of the recipient.


## Use email templates

An email template is a preformatted email message that allows you to quickly create and send email messages. You can modify the text, and then save your changes to the current email template or save the changes to a new email template. Unless you make another selection, **Default Template** is selected for use in an email message. 

You can perform these actions on an email template:

- **Save**: Save your changes to the current email template.

- **Save as**: Save your changes to a new email template.

- **Delete**: Delete the current email template.

- **Rename**: Rename the current email template.

> [!NOTE]
> You can save a maximum of 10 email templates.

## See also

[Define who can respond to a survey](invite-settings.md)<br>
[Send a survey by using Microsoft Flow](send-survey-microsoft-flow.md)<br>
[Embed survey in a web page](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)
