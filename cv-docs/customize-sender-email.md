---
title: "Customize the From address of the email | MicrosoftDocs"
description: "Instructions for customizing the From address of the email"
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

By default, surveys are sent from the `surveys@email.customervoice.microsoft.com` email address. . The email customization feature helps you create a custom email address consisting of your company's domain. You can use then use this custom email address to send survey invitations to your customers.

Let's say you're an owner of a company named Contoso Suites. The company's website is `www.contososuites.com`. You can create two custom email addresses (for example, `noreply@contososuites.com` and `support@contososuites.com`) consisting of your company's domain.

## Add custom email

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.
 
4.	In the **Dynamics 365 Customer Voice** panel, select **Add custom email**.
 
5.	On the **Add domain** page, enter the domain name of the email you want to create, and then select **Next**.
 
6.	Create DNS records in your domain by using the values available under the **Create DNS record** section on the **Verify you own this domain** page.
 
7.	After creating DNS records, select **Verify**.

8.	On the **User emails** page, enter the following information:

    - **Email**: Email address to use for sending survey invitation.
    - **Display name**: Display name for the email user.
    - **Add users**: Users who can use custom email for sending survey invitation.

9.	To add more email addresses, select **Add more emails**, and provide the required information.
 
10.	After adding the required email addresses, select **Next**.

11.	On the **Review custom email and finish** page, review the information, and select **Create policy**.
 
12.	On the **New custom email created** page, a confirmation message is displayed that the custom email is created.

    > [!NOTE]
    > In any of the above steps, you can select Save and close to save your current changes. You can come later and continue from the saved step.
 
13.	Select **Done**.

The custom email is displayed in the **Dynamics 365 Customer Voice** panel.
  
## Edit custom email

After creating a custom email, you can edit it to change its address, display name, and modify the users allowed to use the email.

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.

4.	In the **Dynamics 365 Customer Voice** panel, hover over the email address you want to edit, select the ellipsis button, and then select **Edit custom email**.
 
5.	In the **Edit custom email** panel, edit the required information, and then select **Save**.
 
## Delete custom email

You can delete the email that is no longer required.

1.	Sign in to [Microsoft 365 admin center](https://admin.microsoft.com/) with your work or school account.

2.	Select **Settings** > **Org settings**.

3.	On the **Org settings** page, under the **Services** tab, select **Dynamics 365 Customer Voice**.

4.	In the **Dynamics 365 Customer Voice** panel, hover over the email address you want to delete, select the ellipsis button, and then select **Delete custom email**.
 
5.	In the confirmation pop-up, select **Remove**.

## Example DNS records

### TXT record

`TXT name: @`
`TXT value: msfpkey=abc123abc123abc123abc123`

### CNAME record

`Host name or Alias: fpeurkey1.\_domainkey`
`Points to address: fpeurkey1contosocom.d01.formspro.dynamics.com`

## Frequently asked questions

### Should the email account be a functioning account, or can it be a dummy account?

The email account need not be a functioning account to send emails; however, a mailbox must be configured if the account is expected to receive replies. In most cases, the email address from which survey emails are sent is an unmonitored email account, and need not receive emails.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)
