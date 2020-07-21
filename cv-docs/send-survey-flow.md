---
title: "Send a survey by using Power Automate | MicrosoftDocs"
description: "Instructions for sending a survey by using Power Automate"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Send a survey by using Power Automate

After creating a survey, you can send it to respondents based on a business trigger&#8212;resolution of a case or fulfillment of an order, for example. You can either select a built-in template or create a flow from scratch by using Power Automate. The following Power Automate templates are available out of the box in Dynamics 365 Customer Voice:

- **Send a survey when a case is resolved in Dynamics 365**: This template sends a survey when a case is resolved in Dynamics 365.
- **Send a survey when a lead is qualified in Dynamics 365**: This template sends a survey when a lead is qualified in Dynamics 365.
- **Send a survey when an order is fulfilled in Dynamics 365**: This template sends a survey when an order is fulfilled in Dynamics 365.
- **Send a survey when a button is clicked in Power Apps**: This template sends a survey to the specified list of recipients when a button is selected in Power Apps.
- **Send a survey when a case is closed in Salesforce**: This template sends a survey when a case is closed in Salesforce.

**To send a survey by using Power Automate**

1.  Open the survey, and go to the **Send** tab.

2. Select **Automation**.

    > [!NOTE]
    > If you've sent your survey through email once, the invitation summary is displayed. To send your survey by using Power Automate, select **Resend** > **Automate**.

3.  To configure a built-in flow, select a template. More information: [Create a flow from a template in Power Automate](https://docs.microsoft.com/flow/get-started-logic-template)

5.  To create a flow from scratch, select **Create from blank**. More information: [Create a flow in Power Automate](https://docs.microsoft.com/flow/get-started-logic-flow)

    > [!NOTE]
    > - The flow will use the default email template for sending emails. If you want to send email by using a specific email template, ensure that you've selected it from the **Email template** list in the [send a survey](#send-a-survey-action) action.
    > - While configuring a flow, you might see duplicate templates on the template page. To resolve this issue, navigate out of the tab, and then come back to create the flow again.
    > - If you've added personalized data to your survey, you must specify values for it in the flow. More information: [Specify values in a flow](personalize-survey.md#specify-values-in-a-flow)

5.  Select **Create Flow**.

When you send a survey by using Power Automate, a survey invitation record is created. You can associate your survey invitation and response with Common Data Service.

## Send a survey action

This action sends a survey to a specified list of recipients and creates a survey invitation for each recipient. You can also associate your survey invitation and response with Common Data Service. When you create a flow from scratch, this can be achieved through the **Regarding** and **Recipient details** fields in a flow. If you choose to create a flow from a template, the **Regarding** and **Recipient details** fields are populated accordingly.

Let's say you need to send a survey every time a case is closed. You can use the **Regarding** field to specify the case record so that when an invitation and response are created for a particular case resolution, they're attached to that case. The case manager then can set up reports to show customer satisfaction (CSAT) scores by case, or reopen a case if the CSAT is very low.

Use the **Recipient details** field to associate your survey invitation and response records to the appropriate contact (the recipient). This allows sales personnel, or anyone, to see the contact record and the response of the customer. This can help them formulate their conversation with the customer accordingly.

### Attributes

|Name|Description|
|---|----|
|To|The email address to send the survey invitation to. If you're entering multiple email addresses, separate them by a semicolon.<br>**Note**: The email address should be valid and should not return null.|
|Survey|The survey to be sent.<br>**Note**: You must select a survey from the list and not enter a custom value.|
|Email template|The email template to use while sending the invitation.<br>**Note**: You must select an email template from the list and not enter a custom value.|
|Regarding|The record that associates the survey invitation and response. This value is stored in the survey invitation's **Regarding** field. <br> **Note:** You must enter an entity logical name in this field.|
|Recipient details|The contact to associate your survey invitation and response records with. This value is stored in the survey invitation's **To** field.<br>**Note**: Only the Contact record is supported.|
|||

> [!NOTE]
> If you've used personalized data placeholders in your survey, those fields will be visible in this action and you can specify the values accordingly. More information: [Specify values in a flow](personalize-survey.md#specify-values-in-a-flow)

The values from the **Regarding** and **Recipient details** fields are stored in the survey invitation, as shown in the following image.

> [!div class=mx-imgBorder]
> ![Survey invitation record](media/survey-invite.png "Survey invitation record")  

> [!NOTE]
> The **To** field isn't displayed by default on the form. You must go to **Advanced Find**, search for the invitation, and then add the required columns to see their values.
>
> [!div class=mx-imgBorder]
> ![Search survey invite using Advanced Find](media/survey-invite-adv-find.png "Search survey invitation using Advanced Find") 

<!-- Shubham: will update later as per UI
## View flow history

Flow history is the information that's stored for each survey as you configure flows to send a survey. Before configuring a new flow, you might want to know more about the flows that are already configured for the survey. Flow history gives you the required information about the configured flows, such as the total number of runs, failures, and so on.

Flow history is displayed in a grid with the following information:

- **Date modified**: Date when the flow was modified.

- **Flow**: Name of the flow.

- **Message template**: Email message template(s) used by the flow.

- **Runs**: Total number of times a flow has run. Values of up to 200 are displayed. If a flow has run more than 200 times, 200+ is displayed as the count. You can select the count value to view more details about the run.

- **Failures (last 200 runs)**: Number of times a flow has failed out of the last 200 runs.

- **Status**: Status of the flow: on or off. You can update a flow's status from Power Automate. For more information, see [Manage a flow](https://docs.microsoft.com/flow/get-started-logic-flow#manage-a-flow).  

If required, you can also edit a flow by selecting the **Edit** symbol. The flow editor opens in Power Automate, from which you make your changes.

**To view flow history**

1.  Open the survey for which you want to view flow history, and then select **Send** from the toolbar at the top of the page.

2.  On the **Power Automate** tile, select **Flows configured**. A grid with the configured flows is displayed.
-->
### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)
