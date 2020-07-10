---
title: "Send a survey by using QR code | MicrosoftDocs"
description: "Instructions for sending a survey by using QR code"
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Send a survey by using QR code

A QR code (Quick Response code) is a type of matrix barcode. You can print the QR code or display it on your website. A QR code stores information such as URL for a website. A QR code can be scanned by using any smartphone or tablet. 

QR code for your survey contains a direct link to your survey. You can include the QR code on receipts, posters, or any print media to reach your recipients and collect feedback. Recipients can scan the QR code on a phone or tablet to access the survey.

> [!NOTE]
> - The survey link generated is a non-personalized link. You won't be able to record the respondent's name and whether the respondent has submitted only one response if **Only people in my organization can respond** is turned off in [distribution settings](distribution-settings.md).
> - If you've personalized your survey by using variables, they will not be replaced with their values and the variable names are displayed as is because the link is a non-personalized survey link.

**To send a survey by using QR code**

1. Open the survey and go to the **Send** tab.

2. Select **QR code**.

    > [!NOTE]
    > If you've sent your survey through email once, the invitation summary is displayed. To get your survey's QR code, select **Resend** > **QR code**.

3. In the **Download a QR code pop-up**, select **Download**.

    > [!div class=mx-imgBorder]
    > ![get the survey qr code for sharing](media/survey-qrcode.png "Get the survey QR code for sharing")

    Share the QR code wherever your intended audience can scan it with a QR code scanner, such as on a mobile device.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)
