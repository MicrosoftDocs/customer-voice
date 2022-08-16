---
title: "Create a branching rule for a survey | MicrosoftDocs"
description: "Branching rules allow you to customize the flow of your survey. This topic explains how to create branching rules for a survey with Dynamics 365 Customer Voice."
ms.date: 08/16/2022
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Create a branching rule

Branching rules allow you to customize the flow of your survey. You can show or hide questions, choose to navigate to another question or survey, or even open a website based on the response to a question. Branching rules make your surveys interactive and ensure that only relevant questions are displayed to respondents.

If you have hidden a question from being displayed in a survey by using the **Visible** option, you can use the branching rule to display it based on the required response. For more information about setting the visibility for a question, see [Create a survey](create-survey.md).

For example, for the question **How likely is it that you would recommend us to a friend?**, you can create a branching rule to ask the reason if someone responds **Not likely**.

**To create a branching rule**

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Branching**.

   ![Branching menu item.](media/branching-menu.png "Branching menu item")

    If you haven't created any rules yet, the following message is displayed. Select **Customize**.

    ![Customize survey flow button.](media/customize-survey-flow-button.png "Customize survey flow button") 

    If you've created at least one rule, a list of rules is displayed in a grid. Select **New rule**.

    ![New rule button.](media/existing-rules.png "New rule button")

3. In the **Rule name** field, enter a name for the branching rule.

4. In the **Primary rule condition(s)** area, select **Add condition** to add a response condition.

    > [!NOTE]
    > You can create a maximum of 10 conditions.

5. In the first list, choose whether you want to create a rule on a question or a survey variable.

    ![Select Question or Survey variable.](media/select-ques-var.png "Select Question or Survey variable")

   - If you want to create the rule on a survey variable, select a variable from the **Select survey variable** list.

     ![Branching rules condition variable.](media/branch-condition-variable.png "Branching rules condition variable")

   - If you want to create the rule on a question, select a question from the **Select question** list.

     ![Branching rules condition question.](media/branch-condition-question.png "Branching rules condition question")

6. Select values from the **Select operator** and **Select response** lists, respectively.

   You can add more conditions by using **AND**/**OR** operator by selecting **Add condition**.

    ![Branching rules multiple conditions.](media/branch-multi-condition.png "Branching rules multiple conditions")

7. Select **Add "If true"** to add the action that will be triggered when the defined condition meets the criteria.

8. Select **Add action** to add the response action.

9. In the **Select action** list, choose one of the following actions:

    - **Show**: Select a question to be displayed based on the response to a question.
    - **Hide**: Select a question to be hidden based on the response to a question.
    - **Navigate to**: Select the target to which a respondent should be navigated.

   ![Select an action for true condition.](media/branch-true-select-action.png "Select an action for a true condition")

10. In the **Select target** list, choose a target for the selected action:

    - If you select **Show** or **Hide** as the action, you can select **Question** as the target.

    - If you select **Navigate to** as the action, you can choose one of the following targets:

      - **Question**: Skip to a question based on the response to a question. The questions between the source and target questions are hidden from the respondent.
      - **End of survey**: End the survey based on the response to a question.
      - **Chained survey**: Open a different survey, created by you, based on the response to a question.
      - **URL**: Open a website based on the response to a question. You must add `http://` to the URL for it to work properly.

11. In the **Select value** list, enter or choose a value in accordance with the target.

    ![Branching rules true action.](media/branch-true-action.png "Branching rules true action")

12. Select **Add "If false"** to add the action that's triggered when the defined condition doesn't meet the criteria. Then follow steps 8 through 11.

    ![Branching rules false action.](media/branch-false-action.png "Branching rules false action")

13. Select **Save**.

After creating a branching rule, you can preview the survey and see whether the rule is working as expected.

## Manage branching rules

After you've created a branching rule or a set of branching rules, you can edit, delete, or change the order of their execution. The branching rules are executed in the order they were created in.

1. Open the survey.

2. Select **Customization** at the right side of the page, and then select **Branching**.

    ![Branching menu item.](media/branching-menu.png "Branching menu item")

3. A list of rules is displayed in a grid.

    ![Existing branching rules.](media/existing-rules.png "Existing branching rules")

4. To edit a branching rule, select **Edit** ![Edit branching rule.](media/edit-rule.png "Edit branching rule") from the corresponding rule row.

5. To delete a branching rule, select **Delete** ![Delete branching rule.](media/delete-rule.png "Delete branching rule") from the corresponding rule row.

6. To change the order of execution of a branching rule, move a rule up or down in the grid. To move a rule up or down, select **Move up** ![Move up](media/move-up-rule.png "Move up") or **Move down** ![Move down](media/move-down-rule.png "Move down") from the corresponding rule row.

### See also

[Add and configure satisfaction metrics](satisfaction-metrics.md)<br>
[Personalize your survey by adding variables](personalize-survey.md)<br>
[Create multilingual survey](create-multilingual-survey.md)<br>
[Add branding to your survey](survey-branding.md)<br>
[Add formatting to your survey](survey-formatting.md)<br>
[Add formatting to survey elements](survey-text-format.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
