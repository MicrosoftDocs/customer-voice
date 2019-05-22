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

If you want to use your own survey distribution platform, such as Outlook, Gmail, or SMS, you can create a survey invitation using Microsoft Flow. A survey invitation creates a personalized survey invitation link that you can distributed by using platform of your choice.

1. Sign in to [flow.microsoft.com](https://flow.microsoft.com).

2. Start to create a flow from scratch. For information on creating a flow from scratch, see [Create a flow in Microsoft Flow](https://docs.microsoft.com/en-us/flow/get-started-logic-flow).

3. In the flow editor, add a new step and search for **Microsoft Forms Pro** connector.

4. In search results, select **Microsoft Forms Pro**.

    > [!div class=mx-imgBorder]
    > ![Select Microsoft Forms Pro connector](media/search-connector.png "Select Microsoft Forms Pro connector")  

5. Select the **Create an invitation (preview)** action.

    > [!div class=mx-imgBorder]
    > ![Select Create an invitation (preview) action](media/select-flow-action.png "Select Create an invitation (preview) action")  

6. In the **Create an invitation** action, enter the following values:

    - **Survey**: Select the survey to be sent.
    - **Email**: Recipient's email address.

7. Add a new step and select the action to send the email. For this scenario, we have used Outlook to send the survey.

8. In the **Send an email** action, enter the following values: 
    - **To**: Recipient's email address.
    - **Subject**: Subject of the email.
    - **Body**: Enter the required text and add **Invitation Id** and **Invitation link** dynamic contents.

    After entering the required details, the flow looks as below:

    > [!div class=mx-imgBorder]
    > ![Survey invitation flow](media/survey-invite-flow.png "Survey invitation flow")

    You can run the flow as per your required trigger and send the survey.


