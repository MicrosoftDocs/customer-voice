---
title: "Email delivery status"
description: "This topic explains how to view the survey email delivery status and helps you to understand the reason if the status is shown as failed."
ms.date: 09/30/2022
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# View email delivery status

A survey invitation record is created for each survey email that's sent, either through built-in email editor or with Power Automate. The survey invitations associated with a survey are available on the **Send** tab. The [survey invitations report](view-survey-invite.md) allows you to view statistics associated with survey invitations sent through the built-in email editor or Power Automate.

The [survey invitations report](view-survey-invite.md) also allows you to view invitation details. Invitation details display the following data in a tabular format:

- **Recipient**: Name and email address of the recipient of survey invitation.
- **Status**: Status whether the email is queued, failed, or sent successfully.
- **Created on**: Date on which the survey invitation was sent.

If the status of an email is shown as **Failed**, hover over the status to see the following details:

- **Failure reason**: Displays one of following reasons for failure:
    - Spam complaint
    - Soft bounced
    - Hard bounced
    - Block bounced
    - Invalid email address
    - Invalid recipient address
    - Invalid sender address
    - Invalid reply to address
    - Email activity expired
    - Cache block bounced
    - Cache hard bounced
    - Email blocked by suppression
    - Email failed due to unknown error
- **Bounce category**: Displays the bounce category of the email. For information about email bounce categories, see [Email bounce categories](/dynamics365/marketing/email-bounce-categories).
- **Bounce details**: Displays the error message as received from the destination email server.

This helps you to understand the actual reason for the survey not reaching the intended recipients. This information enables you to create effective survey reports and come up with a relevant plan for scheduling reminders and follow-ups.

For example, in the following image, the survey invitation failed due to the inactive mailbox.

:::image type="content" source="media/email-status.png" alt-text="Screenshot showing the reason for failed status":::

### See also
[View a survey invitations report](view-survey-invite.md)


