---
title: "Embed a survey in Power Apps | MicrosoftDocs"
description: "Instructions for embedding surveys in Power Apps"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Embed a survey in Power Apps
<!--
[!include[cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]
-->
You can embed your surveys in the canvas apps created by using Power Apps. This allows users to respond to the surveys directly from the apps.

> [!NOTE]
> You must have Power Apps Plan 1 to embed your surveys in a canvas app. For more information about purchasing Power Apps, see [Purchase Power Apps for your organization](https://docs.microsoft.com/power-platform/admin/signup-for-powerapps-admin).

1.	Sign in to [Power Apps](https://web.powerapps.com/).

2.	Create a blank canvas app or use one of the available templates. For more information about creating a canvas app, see [Create a canvas app from scratch using Common Data Service](https://docs.microsoft.com/powerapps/maker/canvas-apps/data-platform-create-app-scratch).

3.	On the **Insert** tab, open the **Controls** menu, and then add the **Customer Voice survey (Preview)** control.

4.	In the options pane, select **No data**.

5.	In the **Data** pane, select the survey you want to embed from the **Select survey** list.

    The selected survey is rendered in the control.

6.	To define context parameters, go to the **Advanced** tab in the options pane.

7.	In the **ContextParameters** field, enter context parameters as comma-separated key/value pairs. For example, `{Name:TextInput1.Text,Email:TextInput2.Text, PageTitle:Label1.Text}`.
    You use context parameters to capture your respondent's information and the context in which the response was provided, and store that data in the survey response.

    If a response contains context parameters, they're displayed on the **Personalized data** tab.


### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Create a survey invitation](create-survey-invite.md)
