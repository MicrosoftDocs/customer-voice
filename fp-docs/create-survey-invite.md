---
title: "Create a survey invitation by using Microsoft Flow | MicrosoftDocs"
description: "Instructions for creating a survey invitation by using Microsoft Flow"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 05/22/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 8579EFA2-7734-4516-ACFA-F65999983379
ms.custom: 
---

# Create a survey invitation

[!include[cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

If you want to send a survey using a platform other than Microsoft Forms Pro, such as Outlook, Gmail, or SMS, you can create a survey invitation using Microsoft Flow and send it accordingly. A survey invitation creates a unique survey invitation ID and a personalized link that can be distributed by using a platform of your choice.

1. Sign in to [flow.microsoft.com](https://flow.microsoft.com).

2. Start to create a flow from scratch. For information on creating a flow from scratch, see [Create a flow in Microsoft Flow](https://docs.microsoft.com/en-us/flow/get-started-logic-flow).

3. In the flow editor, add a trigger to start your flow.

4. After adding the trigger, add a new step and search for the **Microsoft Forms Pro** connector.

4. In search results, select **Microsoft Forms Pro**.

    > [!div class=mx-imgBorder]
    > ![Select Microsoft Forms Pro connector](media/search-connector.png "Select Microsoft Forms Pro connector")  

5. Select the **Create an invitation (preview)** action.

    > [!div class=mx-imgBorder]
    > ![Select Create an invitation (preview) action](media/select-flow-action.png "Select Create an invitation (preview) action")  

6. In the **Create an invitation** action, enter or select the following information:

    - **Survey**: Select the survey to be sent.
    - **Email**: Enter the recipient's email address.

    > [!NOTE]
    > - If you want to associate your survey invitation and response with Common Data Service, you must enter values in **Regarding** and **Recipient details** fields accordingly.
    > - If you've used personalized data placeholders in your survey, those fields will be visible in this action and you can specify the values accordingly. More information: [Specify values in a flow](personalize-survey.md#specify-values-in-a-flow)

7. Add a new step and select the action to send the email. In this procedure, we have used Outlook to send the survey.

8. In the **Send an email** action, enter the following information: 

    - **To**: Recipient's email address.
    - **Subject**: Subject of the email.
    - **Body**: Enter the required text and add **Invitation Id** and **Invitation link** dynamic contents.

    After entering the required details, the flow looks as shown in the following image:

    > [!div class=mx-imgBorder]
    > ![Survey invitation flow](media/survey-invite-flow.png "Survey invitation flow")

    The flow runs as per the configured trigger and the sends the survey.
    
    In the following example, Gmail is used to send the survey:

    > [!div class=mx-imgBorder]
    > ![Survey invitation flow using Gmail](media/survey-invite-flow-gmail.png "Survey invitation flow using Gmail")


## See also

[Define who can respond to a survey](invite-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Microsoft Flow](send-survey-microsoft-flow.md)<br>
[Embed survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)


