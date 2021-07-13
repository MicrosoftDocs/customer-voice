---
title: "Send a Dynamics 365 Customer Voice survey from Dynamics 365 | MicrosoftDocs"
description: "This topic explains how to send a survey to your customer from within the customer engagement application's interface."
ms.date: 02/12/2021
ms.topic: article
ms.service: dynamics-365-customervoice
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Send a survey from Dynamics 365
<!--markdownlint-disable MD036-->
**Prerequisites**

- An administrator must install the [Send Customer Voice survey from Dynamics 365](https://appsource.microsoft.com/product/dynamics-365/msfp.customervoicedistribution?tab=DetailsAndSupport) app in your environment for you to send surveys from customer engagement applications. If the option to send surveys isn't visible, contact your administrator.

- An administrator must configure the Power Automate flow to send surveys. More information: [Configure the Power Automate flow](#configure-the-power-automate-flow).

- Users must at least have the **Survey Sender** role to send the survey through Dynamics 365 apps.

You can send a survey to your customer from within the customer engagement application's interface. This helps you to send a survey at the right time in the customer's journey. Let's consider the following scenarios:

**Scenario 1**: You've created a Power Automate flow to send a survey every time a lead is qualified. But, if you want to send a survey during the process of lead qualification, you need to go to Dynamics 365 Customer Voice and send the survey. With this capability, you can send the survey while working on the lead.

**Scenario 2**: As a sales representative, you don't have access to surveys in Dynamics 365 Customer Voice. With this capability, you can send the survey from a customer engagement application without requiring access to Dynamics 365 Customer Voice.

As a salesperson, you can send a survey from the following entities:

-   Contact
-   Opportunity
-   Lead
-   Account
-   Case
-   Contract

You can only send surveys that are shared with you or created by you. If no surveys are shared with you, you can create a new survey (if you have permission to create a survey) and then send it to your customers. If you have Share privilege on the Customer Voice survey entity, you can share a survey with other users or team. More information: [Share a survey](#share-a-survey)

**To send a survey from Dynamics 365**

1.  In the site map of the customer engagement app, select the entity from which you want to send a survey.

2.  From the list of records, open a record.

3.  On the toolbar at the top of the page, select **Send Survey**.

    ![Send Survey button.](media/send-survey-button.png "Send Survey button")

    If you don't have any surveys created or shared with you, select **+ New Survey** to create a new survey. You'll be redirected to Dynamics 365 Customer Voice for the survey creation. More information: [Create a project](create-project.md)

    ![Create new survey link.](media/d365-create-new-survey.png "Create new survey link")

    If you have surveys created or shared with you, you'll be provided with a list of surveys.

    ![New survey button.](media/d365-new-survey-button.png "New survey button")

    If you don't want to send a survey from the available list of surveys, you can create a new survey by selecting **+ New Survey**. You'll be redirected to Dynamics 365 Customer Voice for the survey creation. More information: [Create a project](create-project.md)

4.  In the **Choose one survey to send** dialog box, select a survey to be sent.

    > [!NOTE]
    > You can select only one survey at a time.

5.  To preview the survey, select **Preview**.

6.  To share the survey, see [Share a survey](#share-a-survey).

    ![Choose a survey to send.](media/d365-choose-survey.png "Choose a survey to send")

7.  Select **Next**.

8.  In the **These details will show in your email or survey** dialog box, select the following information:

    - **Recipient**: By default, the name of the contact associated with the entity is populated. You can also remove and select a different recipient, if required. You can select only one recipient at a time.

    - **Email template**: Email template to be used to send the survey invitation.

    - **Locale**: Language of the email template.

    If you've used variables in your survey, they'll be displayed as fields and you can specify their values accordingly.

    ![Enter details to send the survey.](media/d365-enter-details.png "Enter details to send the survey")

9.  Select **Send**.

## Check survey invitation status

When you send a survey invitation, its status will be one of the following:

- **Sending**: The survey invitation email is being sent.

- **Sent**: The survey invitation email was sent successfully.

- **Failed**: The survey invitation email wasn't sent due to an incorrect email address or other error.

**To check survey invitation status**

1.  Go to **Advanced Find**.

2.  In the **Look for** list, select **Customer Voice Send survey history**.

3.  Add the **Status Reason** column.

4.  Select **Results**. A list of survey invitations is displayed with their corresponding status.

    ![Check survey invitation status.](media/d365-check-survey-invite-status.png "Check survey invitation status")

## Share a survey

If you have Share privilege on the Dynamics 365 Customer Voice survey entity, you can share a survey with other users or a team.

1.  In the **Choose one survey to send** dialog box, select a survey to be shared.

2.  Select **Share**.

    ![Select a survey to send.](media/d365-choose-survey.png "Select a survey to send")

    > [!NOTE]
    > If you don't have permission to share surveys, the **Share** button is not displayed.

3.  In the **Share customer voice survey** dialog box, add the users or team you want.

    ![Add users to share a survey with.](media/d365-add-users-share-survey.png "Add users to share a survey with")

4.  Select **Share**.

## Configure the Power Automate flow

The **Send survey on create of custom entity record** Power Automate flow is created automatically when the **Send survey** app is installed. This flow sends the survey when you select **Send Survey** from an entity record. An administrator must set the connection references manually and turn on the flow.

**To configure the Power Automate flow**
<!--markdownlint-enable MD036-->
1.  Go to [flow.microsoft.com](https://flow.microsoft.com/), and select **Solutions** on the left pane.

2.  Find and select the **Send Customer Voice survey from Dynamics 365** solution to open it.

3.  Find and select the **Send survey on create of custom entity record** flow to open it.

4.  Select **Edit** on the toolbar at the top. The flow editor opens.

    A warning symbol is displayed in the header of conditions and actions that have the connection error.

3.  Select the condition or action, and then select the appropriate connection.

4.  Save the changes, and turn on the flow.

### See also

[Create a project](create-project.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]