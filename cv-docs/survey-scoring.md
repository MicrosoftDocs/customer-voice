---
title: "Add scoring to a survey | MicrosoftDocs"
description: "Survey scoring allows you to assign a point value to individual answer options. This topic explains how to add scoring to a survey."
ms.date: 11/21/2025
ms.topic: how-to
author: sbmjais
ms.author: shjais
---

# Survey scoring

Survey scoring allows you to assign a point value to individual answer options. Point values are added to generate a survey-level score for each survey response. A survey with point values assigned to answer options is known as a scored survey. You can use scored surveys to measure your respondent's overall satisfaction level. A scored survey can help you get a better picture of customer service, agent performance, and so on.

For example, as a service provider company, you have created a survey to measure the performance of your customer service agents. The survey consists of five questions with the following answer options:

- Very dissatisfied 
- Dissatisfied 
- Neutral 
- Satisfied 
- Very satisfied 

A point value is attached to each answer option as follows: 

- Very dissatisfied = 1
- Dissatisfied = 2
- Neutral = 3
- Satisfied = 4
- Very satisfied = 5

From this survey, the total score is calculated as weighted average of the normalized question level values.

A survey's score is calculated with the help of the following components:

- **Base score**: This is the number of points the survey is scored from. Each question will be normalized to fit within this score. You can select a base of 5, 10, or 100.

  By default, the base score of a survey is set to 10.

- **Weight**: Weight allows you to measure the importance of a particular question higher or lower than other questions. For more important questions, you should provide a higher value. The final score will be a weighted average of the questions in the score. For example, let's say you have a survey asking for customer feedback regarding the food delivery service. There are three questions that ask about the timeliness of the service, packaging of the food, and quality of the food. In this example, the quality of food is more important than the packaging of food. Therefore, a higher weight should be assigned to the question about quality, giving a more accurate and relevant result.

  By default, the value of weight for all questions is 1.

- **Point**: Point is the value assigned to individual answer options. The maximum point you can assign to an answer option is 100.

  By default, the point values are assigned in the ascending order of the answer options.

The score of a question response is calculated by multiplying weight with the normalized point value. All the question response scores are added to generate a survey-level score.

For information on how a survey score is calculated, see [Survey score calculation](#survey-score-calculation).

Dynamics 365 Customer Voice allows you to apply survey scoring logic to the following question types:

- **Net Promoter Score (NPS)**: You can add weight and update the point values, if required. The normalized point value of the selected response will be multiplied by the weight to generate the question score.

- **Rating (Number, Star, and Smiley)**: You can add weight and update the point values, if required. The normalized point value of the selected response will be multiplied by the weight to generate the question score.

- **Single choice question (radio button and drop down)**: You can add weight and define the scoring order (ascending or descending). The point value for each answer option depends on the order of the answer option in the survey. For example, if there are five answer options and they are in ascending order, option 1 will have point value of 1, option 2 will have point value of 2, and so on. If the answer options are in descending order, option 1 will have point value of 5, option 2 will have point value of 4, and so on. The normalized point value of the selected response will be multiplied by the weight to generate the question score. 

- **Likert**: You can add weight to each of the statements in a question of type Likert. The scoring order and point values are defined in the same way as in the single choice question. The point value of the selected response will be multiplied by the weight to generate the question score.

You can select questions in a survey for which the score needs to be calculated. The **Custom score** satisfaction metric holds the value of the survey score. After you've received responses to your survey, you can [view the satisfaction metrics report](satisfaction-metrics-report.md) to see the survey score showcasing the average score and trend over a period of time.

![Custom score report.](media/custom-score-report.png "Custom score report")

## Add scoring to a survey

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Satisfaction metrics**.

    ![Satisfaction metrics menu item.](media/satisfaction-metrics-button.png "Satisfaction metrics menu item")

3. In the **Satisfaction metrics** panel, select **Add metrics**, and then select **Custom Score**.

    ![Add Custom Score satisfaction metric.](media/custom-score-metric.png "Add Custom Score satisfaction metric")
  
4. Enter the following information:

    - **Name**: Name of the satisfaction metric.

    - **Add description**: Expand the section, and add an optional description for the satisfaction metric.

    - **<survey_name> question**: Choose the questions you want to map to the satisfaction metric.

      ![Add Custom Score satisfaction metric details.](media/custom-score-metric-fields.png "Add Custom Score satisfaction metric details")

5. Select **Edit Score**.

6. In the **Edit Score** panel, select a base score for the survey, assign weight for each question, and assign point values for each answer option.

   ![Add base score, weights, and point values.](media/custom-score-metric-values.png "Add base score, weights, and point values")

7. Select the back arrow at the upper left of the **Edit Score** panel.

8. In the **Satisfaction metrics** panel, select **Save**.

## Edit scoring of a survey

After you've created a **Custom Score** satisfaction metric, you can edit its details. You can change the questions used in calculating the survey score, the base score for the survey, the weight for each question, and the point values for each answer option. You can also delete the ones that you don't need.

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Satisfaction metrics**.

3. Expand the **Custom Score** metric and then update the name and description as required.

4. If required, change the questions used in calculating the survey score.

5. Select **Edit Score** and change the survey scoring logic as required.

6. Select the back arrow at the upper left of the **Edit Score** panel.

7. In the **Satisfaction metrics** panel, select **Save**.

## Survey score calculation

The score of a survey is calculated with the help of following components: base score, weight, and point values. Using these components, the score of a question response is calculated as follows:

1. Normalized point value is calculated as follows: `Normalized value = ((ResponseValue - MinValue.) * 100) / (Max Value – Min Value)`

    where
    - `ResponseValue` is the point value of the response received for the question
    - `Min Value` is the minimum point value of the question and 
    - `Max Value` is the maximum point value of the question


1. Using the normalized point value, score of a question response is calculated as follows: `Question score = Normalized value * Weight of the question`

1. Using the `Normalized value` and `Question score`, final value of custom score is calculated as follows: `Final value = (Sum of question scores) / (Sum of weights assigned to questions)`

    The final value in Dataverse is referred as the custom score for a particular Customer Voice survey response.

1. Using the `Final value`, the `Aggregated score` is calculated as follows: `Aggregated score = Sum (Final value of responses) / Count of responses`

1. Using the `Aggregated score` and `Base score`, the survey level custom score is calculated as follows: `Scaled value = (Aggregated score / 100) * Scale Max` 

    where
    - `Scale Max` is the value of the base score
    - `Aggregated value` is the value obtained from the previous step.

    The `Scaled value` is scaled between 0 and value of the base score. By default, the value of base score is 10.  

    > [!NOTE]
    > The `Scaled value` is the value that is displayed in the satisfaction metrics report. The range of the score depends on the value of base score that further scales the Aggregated score between 0 and the value of base score. The scaled value is rounded to one decimal place.

Let's understand the survey level score calculation with the help of following examples:

### Example 1

You've created a survey containing one rating question with 10 stars. A user has responded to the survey with 4 stars. The custom score configuration is as follows:

:::image type="content" source="media/custom-score-example1.png" alt-text="Custom score example with one question.":::

From the above configuration and the response of the user, values of the components are as follows:

- Weight = 4
- Response value = 4
- MinValue = 1
- MaxValue = 10

The score of the question response is calculated as follows:

- Normalized value = ((4 – 1)*100) / (10 – 1) = 33.3
- Question score = 33.3 * 4 = 133.3
- Final value = 133.3 / 4 = 33.3

Therefore, score of the Customer Voice survey response is 33.3.

:::image type="content" source="media/custom-score-result1.png" alt-text="Custom score result with one question.":::

The aggregated score and scaled value are calculated as follows:
- Aggregated score = 33.3/1 = 33.3
- Scaled value = (33.3 / 100) * 10 = 3.33

Therefore, survey level score is 3.33.

### Example 2

You've created a survey containing one rating question with 5 stars and one single-choice question with 5 options. A user has responded to the survey with 4 stars and option 2. The custom score configuration is as follows: 

:::image type="content" source="media/custom-score-example2.png" alt-text="Custom score example with two questions.":::

From the above configuration and the response of the user, values of the components are as follows:

**Question 1: Rating question**

- Weight = 4
- Response value = 4
- MinValue = 1
- MaxValue = 5
- Base score = 5
 
**Question 2: Single choice question**

- Weight = 3
- Response value = 2
- MinValue = 1
- MaxValue = 2

Scores of the question responses are calculated as follows:

**Question 1: Rating question**

- Normalized value = ((4 – 1)*100) / (5 – 1) = 75
- Question score (q1) = 75 * 4 = 300

**Question 2: Single choice question**

- Normalized value = ((2 – 1)*100) / (2 – 1) = 100
- Question score (q2) = 100 * 3 = 300


Final value = (300 + 300) / (4 + 3) = 85.7

Therefore, score of the Customer Voice survey response is 85.7.

:::image type="content" source="media/custom-score-result2.png" alt-text="Custom score result with two questions.":::

The aggregated score and scaled value are calculated as follows:
- Aggregated score = 85.7/1 = 85.7
- Scaled value = (85.7 / 100) * 5 = 4.3

Therefore, survey level score is 4.3.

### Example 3

You've created a survey containing one NPS question. Two users have responded to the survey with 5 and 10 respectively. The custom score configuration is as follows:

:::image type="content" source="media/custom-score-example3.png" alt-text="Custom score example with NPS question.":::

From the above configuration and the response of the users, values of the components are as follows:

**Response 1**

- Weight = 1 
- Response value = 5   
- MinValue = 0 
- MaxValue = 10 
- Base Score = 100 

**Response 2**

- Weight = 1
- Response value = 10
- MinValue = 0
- MaxValue = 10
- Base Score = 100

Scores of the question responses are calculated as follows:

**Response 1**

- Normalized value = ((5 – 0)*100) / (10 – 0) = 50
- Question score (q1) = 50 * 1 = 50
- Final value = 50 / 1 = 50

**Response 2**

- Normalized value = ((10 – 0)*100) / (10 – 0) = 100
- Question score (q2) = 100 * 1 = 100
- Final value = 100 / 1 = 100

:::image type="content" source="media/custom-score-result3.png" alt-text="Custom score result with two responses to NPS question.":::

The aggregated score and scaled value are calculated as follows:

- Aggregated score = (50 + 100) / 2 = 75
- Scaled value = (75 / 100) * 100 = 75

Therefore, survey level score is 75.

From the above three custom score examples, the satisfaction metrics report displays the scaled value as 3.33, 4.3, and 75 respectively. 

:::image type="content" source="media/custom-score-examples-report.png" alt-text="Scaled value in satisfaction metrics report.":::


### See also

[Add and configure satisfaction metrics](satisfaction-metrics.md)<br>
[View satisfaction metrics report](satisfaction-metrics-report.md)
