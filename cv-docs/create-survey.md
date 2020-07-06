---
title: "Create a survey"
description: "Instructions for creating a survey in Customer Voice."
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Create a survey

A survey is created automatically when you create a project (either from out-of-the-box templates or blank). You can also create a survey within a project. After a survey is created, you can add or edit questions to it and customize it the way you want. For information on creating a project, see [Create a project](create-project.md)

## Create a survey within a project

1. Open the project in which a survey needs to be created.

2. In the left-navigation pane, select **New survey**.

3. Select the default survey title, and then enter a title for your survey. You can also enter an optional description for it.

    ![Survey header](media/survey-header.png "Survey header")

4. Proceed with adding questions to your survey.

## Add or edit questions

1. In the survey designer, select **Add new** to view question types that can be added to your survey. You can also select **More question types** (![Questions types](media/more-ques-button.png "Question types")), and choose a question type.

2. Select the question types you want to add.

3. Enter the question text and its answer options. The survey is saved automatically.

4. To change the order of questions in the survey, select a question, and then select the up arrow (![Move question up](media/move-ques-up.png "Move question up")) or down arrow (![Move question down](media/move-ques-down.png "Move question down")) on the right side of each question to move it up or down.

5. To copy a question, select a question, and then select **Copy question** (![Copy a question](media/copy-ques.png "Copy a question")).

6. To delete a question, select a question, and then select **Delete question** (![Delete a question](media/delete-ques.png "Delete a question")).

## Set visibility of a question

By default, every question in a survey is visible to respondents. You choose to hide a question in a survey by default and then show it based on a logic. The logic can be defined by creating a branching rule. To hide a question from being displayed in a survey, select the question, and then turn off the **Visible** toggle.

![Set visibility of a question](media/ques-visibility.png "Set visibility of a question")

## Mark a question as required

By default, a question is not required to be answered by respondents. If you want a question to be answered, you mark it as required. To mark a question as required, select the question, and then turn on the **Required** toggle.

![Mark a question as required](media/ques-required.png "Mark a question as required")

## Add an image to a survey header

You can add an image, such as logo, to your survey header. When you add an image to the survey header, it is displayed at the top left corner of the survey.

1. Open the survey in which you want to add an image and then select the survey header.

2. Select **Insert image** (![Insert image](media/insert-image.png "Insert image")) on the right side of the header.

3. In the **Insert logo** panel, select **Upload**.

4. Browse the image and upload it.

## Add a media to a question

You can add an image or video to a question in your survey. This helps your respondents to understand the context and respond accordingly.

1. Open the survey in which you want to add an image or video to the question, and then select the question.

2. Select **Insert media** (![Insert media](media/insert-image.png "Insert media")) on the right side of the question.

    The **Insert media** panel is displayed.

3. To add an image, select **Image**.

    1. Select **Upload**.
    
    2. Browse the image to be added and then upload it.

5. To add a video, select **Video**.

    1. Enter the URL of the video hosted on Microsoft Stream or YouTube.
    
    2. Select **Add**.

## Customize a survey

You can customize your survey in the following ways:

- [Add and configure satisfaction metrics](satisfaction-metrics.md)
- [Add logic by creating branching rules](create-branching-rule.md)
- [Personalize your survey by adding variables](personalize-survey.md)
- [Create multilingual survey](create-multilingual-survey.md)
- [Add branding to your survey](survey-branding.md)
- [Add formatting to your survey](survey-formatting.md)
- [Add formatting to survey elements](survey-text-format.md)
