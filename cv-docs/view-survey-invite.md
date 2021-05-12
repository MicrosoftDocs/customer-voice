---
title: "View survey invitations report | MicrosoftDocs"
description: "A survey invitation record is created for each survey email that's sent. This topic explains how to view the survey invitations report."
ms.date: 07/29/2020
ms.service: dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# View survey invitations report

A survey invitation record is created for each survey email that's sent, either manually or with Power Automate. The survey invitations associated with a survey are available on the **Send** tab.

The following survey invitation statistics are displayed in the upper part of the page, and an **Invites tracking** chart is displayed below the statistics:

- **Total invites**: Displays the total number of survey invitations sent.

- **Responses**: Displays the total number of recipients who responded to the survey invitations.

- **Not responded**: Displays the total number of recipients who haven't responded to the survey invitations. A pie chart is displayed that shows the distribution of survey invitations by status:

    - **Unread**: The survey invitation email wasn't read.

    - **Read**: The survey invitation email was read or opened.

    - **Opened**: The survey was opened, but hasn't been completed yet.

- **Unsubscribed**: Displays the total number of recipients who have unsubscribed from receiving survey-related emails.

- **Failed**: Displays the total number of survey invitations that weren't delivered to recipients due to an incorrect email address or other error.

![Survey invitation report](media/invite-report.png "Survey invitation report")

## View invitation details

You can view details of an invitation statistic by selecting **Details** in the upper-right corner of the statistic tile. For example, if you want to see details about the total number of invitations, select **Details** on the **Total invites** tile.

![Survey invitation details button](media/invite-details.png "Survey invitation details button")

The details are displayed in a panel on the right side of the page.

![Survey invitation details displayed in a panel](media/total-invites.png "Survey invitation details displayed in a panel")

## Export invitation details

You can export invitation details to a CSV file either from the statistic tile or the invitation details panel.

**To export invitation details from the statistic tile**

1. In the statistic tile, select the vertical ellipsis ![ellipsis](media/project-options.png "ellipsis"), and then select **Export**.

    ![Survey invitation export button](media/export-invites-tile.png "Survey invitation export button")

2. In the confirmation dialog box, select **Export**.

**To export invitation details from the invitation details panel**

1. In the invitation details panel, select **Export**.

    ![Survey invitation export from the invitation details panel](media/export-invites-panel.png "Survey invitation export from the invitation details panel")

2. In the confirmation dialog box, select **Export**.

## Delete a survey invitation

You can delete a survey invitation that you don't need anymore. To delete a survey invitation, go to the invitation details panel, hover over the invitation, and then select **Delete**. Select **Delete** in the confirmation message.

![Delete a survey invitation from the invitation details panel](media/delete-invite.png "Delete a survey invitation from the invitation details panel")

### See also

[Send a survey to get responses](send-survey.md)<br>
[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using the built-in email composer](send-survey-email.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
