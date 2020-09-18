---
title: "Share a survey by using a survey link | MicrosoftDocs"
description: "Instructions for sharing a survey by using a link"
ms.date: 09/17/2020
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Send a survey link to others

If you don't have the email addresses of the people from whom you want to collect feedback, or if you don't want to use the built-in email composer for this purpose, you can easily copy a link to your survey. You can then send your survey by pasting the link in an email, on a webpage, or in any mode of communication you want to use. The recipients can select the link and complete the survey. The survey link will be a short URL that can be easily distributed by the platforms that have a lower character limit (for example, SMS or Twitter). The short URL will be in the following format: `https://<region>.dcv.ms/<10-digit code>`

> [!NOTE]
> - The survey link generated is a non-personalized link. If the **Only people in my organization can respond** setting is turned off in [distribution settings](distribution-settings.md), you won't be able to record the respondent's name or determine whether the respondent has submitted only one response.
> - If you've personalized your survey by using variables, they won't be replaced with their values and the variable names will be displayed as-is.

**To send a survey by using a link**

1. Open the survey, and go to the **Send** tab.

2. Select **Link**.

    > [!NOTE]
    > If you've sent your survey through email once, the invitation summary is displayed. To get your survey's link, select **Resend** > **Link**.

3. In the **Link to your survey** pop-up window, select **Copy**.

    > [!div class=mx-imgBorder]
    > ![Get the survey link for sharing](media/survey-link.png "Get the survey link for sharing")

    Paste the survey link to a place that's visible to your intended audience. They can select the link to access your survey.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)
