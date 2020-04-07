---
title: "Personalize a survey | MicrosoftDocs"
description: "Instructions for personalizing a survey with Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/15/2020
ms.service: forms-pro
ms.topic: article
ms.assetid: 1AECC69F-B68A-4776-884A-C59770FC5C96
ms.custom: 
search.appverid:
  - FPR160
---

# Personalize a survey

You can automatically insert custom information into your survey by using survey variables. For example, you can use a survey variable to automatically insert a customer's first name and product name into a question to personalize it.

By default, the following survey variables are available:

- **First Name**: Inserts the first name of the recipient.

- **Last Name**: Inserts the last name of the recipient.

- **locale**: Specifies the locale of the survey while embedding it in the email. More information: [Embed a survey in an email](send-survey-email.md#embed-a-survey-in-an-email)

**To create a new survey variable**

1.	Open the survey in which you want to use survey variables.

2.	Select the ellipsis button **(…)** from the toolbar at the top of the page, and then select **Survey variables**.

    > [!div class=mx-imgBorder]
    > ![Survey variables button](media/custom-data-button.png "Survey variables button")

3.	Select **New variable**.

5.	Enter a name and default value for the survey variable.

    > [!div class=mx-imgBorder]
    > ![New survey variable created](media/custom-data-button.png "New survey variable created")

> [!NOTE]
> - After you create a variable, you'll not be able to rename it.
> - You can also personalize survey invitations by using survey variables. More information: [Personalize an email](send-survey-email.md#personalize-an-email)
> - Don't use survey variables if you plan to send a survey anonymously. The variables won't be replaced with actual data in an anonymous survey.
> - Survey variables are replaced with the specified default values when sending a survey invitation.
> - You can define a maximum of 15 variables in a survey.

## Add survey variables to a question

After creating the required survey variables, you need to add them to the question. 

1.	Open the survey in which you want to add survey variables.

2.	On the **Questions** tab, select the question text to which you want to add a survey variable. The formatting toolbar appears.

3.	Place the cursor at the location where you want to add the survey variable.

4.	From the **Variables** list in the formatting toolbar, select the survey variable you want to add.

    > [!div class=mx-imgBorder]
    > ![Add survey variables](media/add-pipe-data.png "Add survey variables")

For example, let's say that you've created a survey variable named **Product Name** and that you want to display the customer's first name and the product name in a question. Select **First Name** and **Product Name** from the **Variables** list. *{{First Name}}* and *{{Product Name}}* are inserted at the cursor location.

Let's say the question is:
*{{First Name}}*, overall, how would you rate your experience with customer service for *{{Product Name}}*?

That question will look like this when a customer named Bert Hair takes the survey for a product named Contoso Sales:

&nbsp;&nbsp;&nbsp;&nbsp;Bert, overall, how would you rate your experience with customer service for Contoso Sales?

## Specify values for survey variables

You must specify default values for survey variables while you create them. If you don't specify default values, nothing will be displayed for the survey variables. You can also specify the values for survey variables:

- When sending email invitations.
- When configuring a flow.

### Specify values when sending email invitations

If you've created survey variables but didn't specify default values for them, a warning message is displayed at the top of the page when you send the survey. Select **Define survey variables** to open the **Survey variables** pane, and then specify the default values.

### Specify values in a flow

To specify values for survey variables in a flow:

1.	While configuring a flow, select **Edit in advanced mode**.

    > [!div class=mx-imgBorder]
    > ![Edit a flow in advanced mode](media/flow-advanced-mode.png "Edit a flow in advanced mode")

2.	Go to the step that sends the survey, and expand it.

3.	Select **Show advanced options**.

    ![Show advanced options for a step in a flow](media/flow-step-advanced-options-button.png "Show advanced options for a step in a flow")

4.	Specify the values for survey variables.

    ![Specify values for survey variables](media/flow-step-advanced-options.png "Specify values for survey variables")

5.	Save the changes.

### See also

[Create a new survey](create-new-survey.md)<br>
[Apply a theme to a survey](apply-theme.md)<br>
[Preview and test a survey](preview-test-survey.md)<br>
[Create a branching rule](create-branching-rule.md)<br>
[Format text in a survey](survey-text-format.md)<br>
[Create a classic form](create-classic-form.md)<br>
[Create a multilingual survey](create-multilingual-survey.md)<br>
[Create a multiple-page survey](create-multipage-survey.md)
