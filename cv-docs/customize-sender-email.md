---
title: "Customize the From address of the email"
description: "Instructions for customizing the From address of the email"
ms.date: 07/29/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Customize the sender's email address

By default, surveys are sent from the `surveys@email.customervoice.microsoft.com` email address. The email customization feature helps you select an email address consisting of your company's domain. You can use the custom email address to send survey invitations to your respondents. 

Let's say you're an owner of a company named Contoso Suites. The company's website is `www.contososuites.com`. You can create two custom email addresses (for example, `noreply@contososuites.com` and `support@contososuites.com`) consisting of your company's domain.

**To customize the sender's email address**

1. Sign in to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/support) with your admin credentials.

2. Select **Help + support** > **New support request**. The support request form is displayed in the right pane.

3. Specify the product details as follows:

    - **Product**: **Dynamics 365 Customer Engagement**
    - **Problem type**: **Forms Pro**<!--Is this accurate?-->
    - **Environment**: Enter or select your Common Data Service environment

4. Select **See solutions**.

5. Select **Create a support request**, and specify details as follows:

    - **Issue title**: Customize the From email address to send survey invitations
    - **Issue description**: Enter your issue description, and provide the domain you want to configure for sending emails. For example, if the website is `www.contososuites.com`, you must provide `contososuites.com` as the domain.
    - **How severe is this issue?**: Select the severity of the issue.

6. Select **Next**.

7. Enter your contact information, and then select **Submit**. A ticket is created with the Microsoft support team, which will contact you with the following DNS records:

    - **Ownership authentication key**: Proves that your organization owns the domain.

    - **Email authentication keys for DKIM**: Prove that Dynamics 365 Customer Voice is authorized to send messages that show your organization's domain name in the from-address.

8.	After record creation, contact Microsoft support, and provide the following information:

    - A list of email addresses you want to create, such as  noreply@contososuites.com and support@contososuites.com.
    - A list of users who will be sending the survey invitations by using the custom email.

    Based on the information provided, Microsoft support will then verify the records and create the DKIM keys for signing the emails. You'll get a confirmation from Microsoft support that the record verification is complete.

    > [!NOTE]
    > The SLA for creating DKIM keys is minimum three to four days.

10.	Sign in to Dynamics 365 Customer Voice, and open the **Distribution** panel. Expand the **Email** section, and select the custom email address that you want to use for sending email.
    
    Use the custom email while sending the survey invitation.

    > [!NOTE]
    > In Power Automate, the custom email address is picked from the survey distribution settings.

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

### How long does it take for setup to be completed?

It will take a minimum of three to four days for setup to be completed. After Microsoft support confirms the domain is active, you can start sending survey invitations by using the custom email.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)<br>
[Embed a survey in a webpage](embed-web-page.md)<br>
[Send a survey link to others](send-survey-link.md)<br>
[Send a survey QR code](send-survey-qrcode.md)<br>
[Embed a survey in Power Apps](embed-survey-powerapps.md)
