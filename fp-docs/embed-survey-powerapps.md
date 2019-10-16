---
title: "Embed a survey in PowerApps | MicrosoftDocs"
description: "Instructions for embedding surveys in PowerApps"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 08/19/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: F5543364-ADB8-465D-96A6-81B2C840299F
ms.custom:
search.appverid:
  - FPR160
---

# Embed a survey in PowerApps

[!include[cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

You can embed your surveys in the canvas apps created using PowerApps. This allows users to respond to the surveys directly from the apps.

> [!NOTE]
> You must have PowerApps Plan 1 to embed your surveys in a canvas app. For more information on purchasing PowerApps, see [Purchase PowerApps for your organization](https://docs.microsoft.com/en-us/power-platform/admin/signup-for-powerapps-admin).

1.	Sign in to [PowerApps](https://web.powerapps.com/).

2.	Create a blank canvas app or use one of the available templates. For more information on creating a canvas app, see [Create a canvas app from scratch using Common Data Service](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/data-platform-create-app-scratch).

3.	On the **Insert** tab, open the **Controls** menu and then add the **Forms Pro survey (Preview)** control.

    > [!div class=mx-imgBorder]
    > ![Add the Forms Pro survey (Preview) control](media/insert-control.png "Add the Forms Pro survey (Preview) control")  

4.	In the options pane, select **No data**.

    > [!div class=mx-imgBorder]
    > ![Options pane](media/options-pane.png "Options pane")  

5.	In the **Data** pane, select the survey you want to embed from the **Select survey** list.

    > [!div class=mx-imgBorder]
    > ![Select survey in the Data pane](media/data-pane.png "Select survey in the Data pane") 

    The selected survey is rendered in the control.

    > [!div class=mx-imgBorder]
    > ![Survey rendered in the control](media/survey-render.png "Survey rendered in the control") 

6.	To define context parameters, go to the **Advanced** tab in the options pane.

7.	In the **ContextParameters** field, enter context parameters as comma-separated key/value pairs. For example, `{Name:TextInput1.Text,Email:TextInput2.Text, PageTitle:Label1.Text}`. 
    Context parameters allow you to capture your respondent's information and the context in which the response was provided and store that data in the survey response. 

    > [!div class=mx-imgBorder]
    > ![Add context parameters](media/context-param.png "Add context parameters")

    If a response contains context parameters, they are displayed on the **Personalized data** tab. 

    > [!div class=mx-imgBorder]
    > ![Context parameters in a survey response](media/context-param-powerapps.png "Context parameters in a survey response") 

## See also

[Work with survey settings](invite-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Microsoft Flow](send-survey-microsoft-flow.md)<br>
[Embed survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Create a survey invitation](create-survey-invite.md)
