---
title: "Distribute a survey by using Microsoft Flow | MicrosoftDocs"
description: "Instructions to distribute a survey by using Microsoft Flow"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 2/21/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 11ac9528-c0a6-4fe6-9886-d2a4bfaa72f4
ms.custom: 
---
# Distribute a survey by using Microsoft Flow

After creating a survey, you can choose to send it to respondents based on a business trigger, for example, on resolution of a case, fulfillment of an order, and so on. You can either select a built-in template or create a flow from scratch by using Microsoft Flow.

1.  Open the survey you want to distribute and go to **Send Survey** &gt; **Microsoft Flow**.

2.  Compose the email.

3.  Select **Configure Flow**.

4.  Select a built-in template or choose to create a flow from blank. For information on how to work with Microsoft Flow, see [here](https://docs.microsoft.com/en-us/flow/get-started-logic-template).  

> [!NOTE]
> While configuring a flow, the template page might display duplicate templates. To resolve this issue, you must navigate out of the **Send Survey** tab, and then come back to create the flow again.

5.  Select **Create Flow**.

## View flow history

Flow history is the information that is stored per survey as you configure flows to send a survey. Before configuring a new flow for a survey, you might want to know the flows that are already configured for the survey. Flow history gives you the required information about the configured flows such as the total number of runs, failures, and so on.

Flow history is displayed in a grid with the following information:

- **Date modified**: Date when the flow was modified.

- **Flow**: Name of the flow.

- **Message template**: Email message template(s) used by the flow.

- **Runs**: Total number of times a flow has run. The count will be displayed up to 200 only. If a flow has run more than 200 time, 200+ will be displayed as the count. You can click the count to view more details about the run.

- **Failures (last 200 runs)**: Number of times a flow has failed out of last 200 runs.

- **Status**: Status of the flow: on or off. You can update a flow’s status from Microsoft Flow. More information on managing a flow, see [Manage a flow](https://docs.microsoft.com/en-us/flow/get-started-logic-flow#manage-a-flow).  

If required, you can also edit a flow by selecting the **Edit** icon. The flow editor opens in Microsoft Flow in which you make the required changes.

![edit a flow](media/edit-flow.png "Edit a flow")  

To view flow history:

1.  Open the survey you want to view flow history and go to **Send Survey** &gt; **Microsoft Flow**.

2.  Select **Flow history** from the toolbar at the top.

    ![view flow history](media/view-flow-history.png "View flow history")  

    A grid with the configured flows is displayed.

    ![flow history details](media/flow-history-details.png "Flow history details")  

