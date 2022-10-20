---
title: Email delivery status
description: Learn how to view the survey email delivery status and understand the reason if the delivery failed.
ms.date: 10/19/2022
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# View email delivery status

A survey invitation record is created for each survey email you send either through the built-in email editor or with Power Automate. You can view the invitations that are associated with a survey on the **Send** tab. The [survey invitations report](view-survey-invite.md) shows statistics and details about the invitations, including:

- **Recipient**: The name and email address of the recipient
- **Status**: The status of the invitation email, either queued, failed, or sent
- **Created on**: The date on which the invitation was sent

If the status of an invitation email is **Failed**, hover over the status to view the following information:

- **Failure reason**: The reason the email failed to send

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

- **Bounce category**: The email's [bounce category](/dynamics365/marketing/email-bounce-categories)

- **Bounce details**: The error message received from the destination email server

In the following example, the survey invitation failed because the mailbox isn't accepting email:

:::image type="content" source="media/email-status.png" alt-text="Screenshot of the survey invitations report, showing that an invitation failed because the mailbox is inactive.":::

This information helps you to understand the reason the survey didn't reach the intended recipients. With it, you can create effective survey reports and schedule reminders and follow-ups.

### See also

[View a survey invitations report](view-survey-invite.md)
