---
title: "Add formatting to a survey | MicrosoftDocs"
description: "Instructions for adding formatting to a survey created with Dynamics 365 Customer Voice."
ms.date: 07/29/2020
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Add formatting to a survey

Formatting controls the general look and feel of your survey. This includes showing or hiding a progress bar, showing or hiding question numbers, and shuffling questions in a survey. 

**To add formatting to a survey**

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Formatting**.

    ![Formatting menu item](media/formatting-button.png "Formatting menu item")

    The **Formatting** panel is displayed.

    ![Formatting panel](media/formatting-panel.png "Formatting panel")

3. Update the formatting options as described in the following sections.

## Progress bar

A progress bar shows your respondents the percentage of pages that they've navigated to or viewed so far. It gives them an idea of how far they've come and how far they have to go. The progress bar takes into account all pages in the survey. If pages have been skipped due to a branching rule, the progress bar shows the adjusted completion percentage. The progress bar is displayed only if there are two or more pages in the survey.

By default, this setting is turned on for multiple-page surveys and the progress bar is displayed. For a single-page survey, this setting is turned off.

When turned on, the progress bar is displayed to the right side of the buttons on the survey.

![Progress bar on a survey](media/progress-bar.png "Progress bar on a survey")

## Question number

Specify whether the question numbers should be displayed in a survey. By default, this setting is turned on. If you want to hide question numbers in a survey, turn off this setting.

## Shuffle questions

Specify whether the questions in a survey should be shuffled. By default, this setting is turned off. If you want to enable question shuffling in a survey, turn on this setting. This setting is disabled when a branching rule is created in a survey.

### See also

[Add and configure satisfaction metrics](satisfaction-metrics.md)<br>
[Add logic by creating branching rules](create-branching-rule.md)<br>
[Personalize your survey by adding variables](personalize-survey.md)<br>
[Create multilingual survey](create-multilingual-survey.md)<br>
[Add branding to your survey](survey-branding.md)<br>
[Add formatting to survey elements](survey-text-format.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]