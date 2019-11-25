---
title: "Analyze survey invitations | MicrosoftDocs"
description: "Instructions for analyzing survey invitations"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 12/05/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: efa240ce-9ef0-40e6-b634-143a347201e9
ms.custom: 
search.appverid:
  - FPR160
---

# Analyze survey invitations

A survey invitation record is created for each survey email that is sent, either manually or with Microsoft Flow. To see the survey invitations associated with a survey, go to **Responses** &gt; **Overview**, and then select **Invitations** from the summary information.

> [!div class=mx-imgBorder]
> ![Survey invitations](media/survey-invites.png "Survey invitations")

The following survey invitation statistics are displayed in a summary pane at the top of the page and the list of survey invitations sent for a survey is displayed below the statistics in the grid format.

- **Average turnaround time**: Average time between sending a survey invitation and receiving a survey response. The unanswered survey invites are ignored for this.

- **Failed invitations**: Number of failed invitations in the last week.

- **Invitation status**: A pie chart showing the distribution of survey invitations by status. Following statues are displayed:

  - **Queued**: The survey invitation email is queued to be sent.
  - **Sent**: The survey invitation email is successfully delivered to the recipient.
  - **Failed**: The survey invitation email is not delivered to the recipient due to an incorrect email address or any other error.
  - **Responded**: The recipient has responded to the survey.
  - **Unsubscribed**: The recipient has unsubscribed from receiving the survey related emails.
  - **Read**: The survey invitation email is read or opened.
  - **Delayed**: There is some delay is delivering the survey invitation email and is being retried.

- **Invitation trend**: A line chart showing the distribution of survey invitation trends.

> [!div class=mx-imgBorder]
> ![Survey invitations details](media/survey-invites-details.png "Survey invitations details")

## Filter invitations

You can filter the invitations by using the following:

- **Pre-defined filters**: Use the Sent, Responded, In Progress, Failed, and Unsubscribed filters to filter the invitations.

- **Date range**: Select 30 days, 90 days, or a custom date range.

- **Recipient's name or email address**: Enter the recipient's name or email address in the search box.

## Export survey invitations

You can export a single survey invitation or multiple survey invitations to Microsoft Excel. To export survey invitation(s), select the required invitation(s), and then select **Export** in the **Invitations details** section.

Each invitation property is a column and each invitation becomes a row in the Excel workbook. 

> [!div class=mx-imgBorder]
> ![Export survey invitations](media/export-survey-invite.png "Export survey invitations")

## Delete survey invitations

You can delete a single survey invitation or multiple survey invitations from Forms, CDS, and insights store. When a survey invitation is deleted, the associated survey response is also deleted.

To delete survey invitation(s), select the required invitation(s), and then select **Delete** in the **Invitations details** section. Select **Delete** in the confirmation message.

> [!div class=mx-imgBorder]
> ![Delete survey invitations](media/delete-survey-invite.png "Delete survey invitations")

## See also

[View summary information for your survey](view-summary-information.md)<br>
[View details for each question](view-details-each-question.md)<br>
[Analyze survey responses](analyze-survey-responses.md)<br>
[Analyze survey insights](analyze-survey-insights.md)
