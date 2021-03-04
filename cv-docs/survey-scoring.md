---
title: "Add scoring to a survey | MicrosoftDocs"
description: "Instructions for adding scoring to a survey created with Dynamics 365 Customer Voice."
ms.date: 03/10/2021
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Survey scoring

Survey scoring allows you to assign a point value to individual answer options. Point values are added to generate a survey-level score for each survey response. A survey with point values assigned to answer options is known as a scored survey. You can use scored surveys to measure your respondent's overall satisfaction level. For example, a scored survey can help you get a better picture on customer service, agent's performance, and so on.

For example, as an healthcare provider, you have created a survey to measure the psychological distress of your patients by using Kessler 5 Distress Scale. The survey consists of five questions with the following answer options:

- None of the time 
- A little of the time 
- Some of the time 
- Most of the time 
- All of the time 

A point value is attached to each answer option as follows: 

- None of the time = 1
- A little of the time = 2
- Some of the time = 3
- Most of the time = 4
- All of the time = 5

From this survey, a total score out of 25 can be calculated. A score of 5 through 11 indicates that a person is well or  experiencing only mild distress. A score of 12 through 25 indicates that a person is experiencing moderate to high distress. 

A survey's score is calculated with the help of following components:

- **Base score**: Base score is the number of points the survey is scored from. Each question will be normalized to fit within this score. You can select a base of 5, 10, or 100.

- **Weight**: Weight allows you to measure the importance of a particular question higher or lower than the other question. For example, let's say you have a survey asking for customer's feedback regarding the food delivery service. There are three questions that ask about the timeliness of the service, packaging of the food, and quality of the food. In this example, the quality of food is more important than the packaging of food. Therefore, a higher weight will be assigned to the question about quality, thereby giving a more accurate and relevant result.

- **Point**: Point is the value assigned to individual answer options.The maximum point you can assign to an answer option is 100.

The score of a question response is calculated by multiplying weight with the point value. All the scores are added to generate a survey-level score.

You can apply survey scoring logic to the following question types:

- Net Promoter Score (NPS): 
- Rating (Number, Star, and Smiley): 
- Single choice question (radio button and drop down): 
- Likert: 

Dynamics 365 Customer Voice allows you to select questions in a survey for which the score needs to be calculated. The **Custom score** satisfaction metric holds the value of survey score. After you've received responses to your survey, you can [view the satisfaction metrics report](satisfaction-metrics-report.md) to see the survey score showcasing the average score and trend over a period of time.



