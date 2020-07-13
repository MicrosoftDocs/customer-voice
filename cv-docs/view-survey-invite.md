---
title: "View survey invitations report"
description: "Instructions for viewing survey invitations report"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# View survey invitations report

A survey invitation record is created for each survey email that's sent, either manually or with Microsoft Power Automate. The survey invitations associated with a survey are available on the **Send** tab.

The following survey invitation statistics are displayed in the upper part of the page and an **Invites tracking** chart is displayed below the statistics.

- **Total invites**: Displays the total number of survey invitations sent.

- **Responses**: Displays the total number of recipients who responded to the survey invitations.

- **Not responded**: Displays the total number of recipients who have not responded to the survey invitations. A distribution of survey invitations by status is displayed in a pie chart. The following statuses are displayed:

    - **Unread**: The survey invitation email is not read.

    - **Read**: The survey invitation email is read or opened.

    - **Opened**: The survey is opened but is not completed yet.

- **Unsubscribed**: Displays the total number of recipients who have unsubscribed from receiving the survey-related emails.

- **Failed**: Displays the total number of survey invitations that were not delivered to the recipients due to an incorrect email address or any other error.

![Survey invitation report](media/invite-report.png "Survey invitation report")

## View invitation details

You can view details of an invite statistic by selecting **Details** in the upper-right corner of the statistic tile. For example, if you want to see details of total invites, select **Details** on the **Total invites** tile.

![Survey invitation details button](media/invite-details.png "Survey invitation details button")

The details are displayed in a panel on the right-side of the page.

![Survey invitation details displayed in a panel](media/total-invites.png "Survey invitation details displayed in a panel")

## Export invitation details

You can export invitation details to a CSV file either from the statistic file of the invitation details panel. 

**To export invitation details from the statistic tile**

1. In the statistic tile, select the ellipsis button, and then select **Export**.

    ![Survey invitation export button](media/export-invites-tile.png "Survey invitation export button")

2. Select **Export** in the confirmation dialog box.

**To export invitation details from the invite details panel**

1. Select **Export** in the invite details panel.

    ![Survey invitation export from invite details panel](media/export-invites-panel.png "Survey invitation export from invite details panel")

2. Select **Export** in the confirmation dialog box.