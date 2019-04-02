---
title: "Send a survey by using Microsoft Flow | MicrosoftDocs"
description: "Instructions for sending a survey by using Microsoft Flow"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/02/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 11ac9528-c0a6-4fe6-9886-d2a4bfaa72f4
ms.custom: 
---

# Send a survey by using Microsoft Flow

[!include[cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

After creating a survey, you can send it to respondents based on a business trigger&#8212;resolution of a case or fulfillment of an order, for example. You can either select a built-in template or create a flow from scratch by using Microsoft Flow. The following flow templates are available out of the box in Forms Pro:

- **Send a survey when a case is resolved in Dynamics 365**: This template sends a survey when a case is resolved in Dynamics 365.
- **Send a survey when a lead is qualified in Dynamics 365**: This template sends a survey when a lead is qualified in Dynamics 365.
- **Send a survey when an order is fulfilled in Dynamics 365**: This template sends a survey when an order is fulfilled in Dynamics 365.
- **Send a survey when a button is clicked in PowerApps**: This template sends a survey to the specified list of recipients when a button is clicked in PowerApps.
- **Send a survey when a case is closed in Salesforce**: This template sends a survey when a case is closed in Salesforce.

To send a survey by using Microsoft Flow:

1.  Open the survey you want to send, and go to **Send Survey** &gt; **Microsoft Flow**.

2.  Compose the email.

3.  Select **Configure Flow**.

4.  To configure a built-in flow, select a template. For information on creating a flow from a template, see [Create a flow from a template in Microsoft Flow](https://docs.microsoft.com/en-us/flow/get-started-logic-template). 

5.  To create a flow from scratch, select **Create from blank**. For information on creating a flow from scratch, see [Create a flow in Microsoft Flow](https://docs.microsoft.com/en-us/flow/get-started-logic-flow).

> [!NOTE]
> While configuring a flow, the template page might display duplicate templates. To resolve this issue, navigate out of the **Send Survey** tab, and then come back to create the flow again.

5.  Select **Create Flow**.

## View flow history

Flow history is the information that is stored for each survey as you configure flows to send a survey. Before configuring a new flow, you might want to know more about the flows that are already configured for the survey. Flow history gives you the required information about the configured flows, such as the total number of runs, failures, and so on.

Flow history is displayed in a grid with the following information:

- **Date modified**: Date when the flow was modified.

- **Flow**: Name of the flow.

- **Message template**: Email message template(s) used by the flow.

- **Runs**: Total number of times a flow has run. Values of up to 200 are displayed. If a flow has run more than 200 times, 200+ is displayed as the count. You can select the count value to view more details about the run.

- **Failures (last 200 runs)**: Number of times a flow has failed out of the last 200 runs.

- **Status**: Status of the flow: on or off. You can update a flow’s status from Microsoft Flow. For more information, see [Manage a flow](https://docs.microsoft.com/en-us/flow/get-started-logic-flow#manage-a-flow).  

If required, you can also edit a flow by selecting the **Edit** symbol. The flow editor opens in Microsoft Flow, from which you make your changes.

![edit a flow](media/edit-flow.png "Edit a flow")  

To view flow history:

1.  Open the survey for which you want to view flow history, and go to **Send Survey** &gt; **Microsoft Flow**.

2.  On the **Send Survey** tab, select **Flow history** ![view flow history](media/view-flow-history.png "View flow history")  from the toolbar at the top of the page.

    A grid with the configured flows is displayed.

    ![flow history details](media/flow-history-details.png "Flow history details")  

## See also

[Define who can respond to a survey](invite-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Embed in a web page](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)