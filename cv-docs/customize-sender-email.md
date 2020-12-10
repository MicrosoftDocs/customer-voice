---
title: "Customize the From address of the email | MicrosoftDocs"
description: "Instructions for customizing the From address of survey emails."
ms.date: 12/09/2020
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Customize the sender's email address

[!INCLUDE[cc-data-platform-banner](includes/cc-data-platform-banner.md)]

By default, surveys are sent from the `surveys@email.customervoice.microsoft.com` email address. The email customization feature helps you create a custom email address based on your organization's domain. You can use then use this custom email address to send survey invitations to your customers.

Let's say your company is Contoso Suites, and the company's website is `www.contososuites.com`. You could create two custom email addresses based on your company's domain, such as `noreply@contososuites.com` and `support@contososuites.com`.

## Add custom email addresses

Take the following steps to add custom email addresses:<!-- Edit note: Generally, updating "email" with "email address" because "email" usually refers to an email message instead of an address. Perhaps you could call it an account and not an address in some cases. -->

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.
 
4.	In the **Dynamics 365 Customer Voice** panel, select **Add custom email**.
 
5.	On the **Add domain** page, enter the domain name of the email domain you want to create, and then select **Next**.
 
6.	Create DNS records in your domain by using the values available under the **Create DNS record** section on the **Verify you own this domain** page.
 
7.	After creating DNS records, select **Verify**.<!-- Edit note: What if there is an error with verification. -->

8.	On the **User emails** page, enter the following information:

    - **Email**: Email address to use for sending survey invitation.
    - **Display name**: Display name for the email user.
    - **Add users**: Users who can use custom email addresses when sending survey invitations.

9.	To add more email addresses, select **Add more emails**, and then provide the required information.
 
10.	After adding the required email addresses, select **Next**.

11.	On the **Review custom email and finish** page, review the information, and then select **Create policy**.
 
12.	On the **New custom email created** page, a confirmation message is displayed that the custom email address is created.

    > [!NOTE]
    > In any of the above steps, you can select **Save and close** to save your current changes. You can come back later and continue from the saved step.
 
13.	Select **Done**.

The custom email address is displayed in the **Dynamics 365 Customer Voice** panel.
  
## Edit custom email addresses

After creating a custom email address, you can edit it to change its address, display name, and modify the users allowed to use the email.

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.

4.	In the **Dynamics 365 Customer Voice** panel, hover over the email address you want to edit, select the ellipsis button, and then select **Edit custom email**.
 
5.	In the **Edit custom email** panel, edit the required information, and then select **Save**.
 
## Delete custom email addresses

You can delete custom email addresses that are no longer required.

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.

4.	In the **Dynamics 365 Customer Voice** panel, hover over the email address that you want to delete, select the ellipsis button, and then select **Delete custom email**.
 
5.	In the confirmation dialog box, select **Remove**.

## Example DNS records

### TXT record<!-- Edit note: Perhaps we can add more detail about what we are presenting here. Is this to show the format. -->

`TXT name: @`
`TXT value: msfpkey=abc123abc123abc123abc123`

### CNAME record

`Host name or Alias: fpeurkey1.\_domainkey`
`Points to address: fpeurkey1contosocom.d01.formspro.dynamics.com`

## Frequently asked questions

### Should the email account be a functioning account, or can it be a dummy account?

The email account need not be a functioning account to send emails; however, a mailbox must be configured if the account is expected to receive replies. In most cases, the email address from which survey emails are sent is an unmonitored email account and need not receive emails.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)
