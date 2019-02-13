---
title: "Analyze survey invitations | MicrosoftDocs"
description: "Instructions for analyzing survey invitations"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/08/2019
ms.service: 
ms.topic: article
ms.assetid: efa240ce-9ef0-40e6-b634-143a347201e9
ms.custom: 
---
# Analyze survey invitations

A survey invitation record is created for each survey email that is sent, either manually or with Microsoft Flow. To see the survey invitations associated with a survey, go to **View Responses** &gt; **Overview**, and then select **Invitations** from the summary information.

![Survey invitations](media/survey-invites.png "Survey invitations")

<!--note from editor--in sentence below, is "across the top" referring to "across the top of the screen"?-->

The following survey invitation statistics are displayed across the top and the list of survey invitations sent for a survey is displayed below the statistics in the grid format.

<!--note from editor: In list below: 1) What does "failed invitation" mean? That the email got bounced back? 2)What is "invitation status"--does that refer to "responded to, sent, failed, in-progress? 3) Unclear to me what "Invitation trend" is measuring. -->

- **Average turnaround time**: Average time between sending a survey invitation and receiving a survey response. The unanswered survey invites are ignored for this.

- **Failed invitations**: Number of failed invitations in the last week.

- **Invitation status**: A pie chart showing the distribution of survey invitations by status.

- **Invitation trend**: A line chart showing the distribution of survey invitation trends.

![Survey invitations details](media/survey-invites-details.png "Survey invitations details")

## Filter invitations

You can filter the invitations by using the following:
- **Pre-defined filters**: Use the Sent, Responded, In Progress, Failed, and Unsubscribed filters to filter the invitations.
- **Date range**: Select 30 days, 90 days, or a custom date range.
- **Recipient's name or email address**: Enter the recipient's name or email address in the search box.

## View invitation details

To view details of a survey invitation, select an invitation in the grid. You'll see the number of responses received for the invitation.

A summary of response details is also displayed for the survey invitation on the invitation details page.

## Export survey invitations

You can export a single survey invitation or multiple survey invitations to Microsoft Excel. To export survey invitation(s), select the required invitation(s), and then select **Export** in the **Invitations details** section.

Each invitation property is a column and each invitation becomes a row in the Excel workbook. 

![Export survey invitations](media/export-survey-invite.png "Export survey invitations")

## Delete survey invitations

You can delete a single survey invitation or multiple survey invitations from Forms, CDS, and insights store. When a survey invitation is deleted, the associated survey response is also deleted.

To delete survey invitation(s), select the required invitation(s), and then select **Delete** in the **Invitations details** section. Select **Delete** in the confirmation message.

![Delete survey invitations](media/delete-survey-invite.png "Delete survey invitations")


