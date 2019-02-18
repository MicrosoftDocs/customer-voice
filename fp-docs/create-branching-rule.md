---
title: "Create branching rule for a survey with Microsoft Forms Pro | MicrosoftDocs"
description: "Instructions for creating branching rule for a survey with Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/07/2019
ms.service: 
ms.topic: article
ms.assetid: 72B81F9F-952B-4A58-83C7-9F68A5EF9B5C
ms.custom: 
---

[!include[cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

# Create a branching rule

When you want to ask additional questions based on responses in a survey, create one or more branching rules for the response you want more information about. Branching rules make your surveys interactive and ensures that only the relevant questions are displayed to the responders. You can also choose to navigate to another question, survey, or even open a website based on the response of a question.

For example, for the question **How likely is it that you would recommend us to a friend?**, you can create a branching rule to ask the reason if someone responds **Not likely**.

1.	Open the survey in which you want to add a branching rule.

2.	On the **Create Questions** tab, select the ellipsis button (…) from the toolbar at the top of the page, and then select **Branching rules**. 

    ![Branching rules button](media/branching-rules-button.png "Branching rules button")
    
    If you don't have any rules created yet, the following page is displayed. Select **Create rule**. 

    ![Create new rule button](media/create-rule-button.png "Create new rule button") 

    If you have at least one rule created, a list of rules is displayed in a grid. Select **New rule**. 
 
    ![New rule button](media/branch-new-rule-button.png "New rule button")

4.	In the **Rule name** field, enter a name of the branching rule.

5.	In the **Define conditions** area, select **Add condition** to add a response condition.

6.	In the **Select question** list, choose the question for which you want to create a rule.

7.	Select values from the **Select operator** and **Select response** lists accordingly.

    ![Branching rules condition](media/branch-condition.png "Branching rules condition")

    You can add more conditions in the combination of And/Or operators by selecting Add condition.

    ![Branching rules multiple conditions](media/branch-multi-condition.png "Branching rules multiple conditions")

8.	Select **Add “If true”** to add the action that will trigger when the defined condition meets the criteria.

9.	Select **Add condition** to add a response action.

10.	In the **Select action** list, choose one of the following actions:

    - **Show**: Allows you to select a question to be displayed as per response to a question.
    - **Hide**: Allows you to select a question to be hidden as per response to a question.
    - **Toggle**: Allows you to toggle the state of the selected question as per response to a question.
    - **Navigate to**: Allows you to select a target to which a responder should be navigated.

11.	In the **Select target** list, choose a target for the selected action. If you select **Show**, **Hide,** or **Toggle** as the action, you can select **Question** as the target. If you select **Navigate to** as the action, you can choose one of the following targets:

    - **Question**: Allows you to skip to a question as per response to a question.
    - **End of survey**: Allows you to end the survey as per response to a question.
    - **Chain survey**: Allows you to open a different the survey as per response to a question.
    - **URL**: Allows you to open a website as per response to a question.

12.	In the **Select value** list, enter or choose a value as per the target.

    ![Branching rules true action](media/branch-true-action.png "Branching rules true action")

13.	Select **Add “If false”** to add the action that will trigger when the defined condition does not meet the criteria. Follow the steps you took while adding the true action.

    ![Branching rules false action](media/branch-false-action.png "Branching rules false action")

14. Select **Save**.

