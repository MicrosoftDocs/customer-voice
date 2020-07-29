---
title: "Plan a survey | MicrosoftDocs"
description: "Instructions for planning a survey with Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 06/12/2020
ms.service: forms-pro
ms.topic: article
ms.assetid: FD23CE2B-B022-4708-BAE8-5CAC8BC75092
ms.custom: 
search.appverid:
  - FPR160
---

# Plan to create a survey

> [!NOTE]
> Microsoft Forms Pro has evolved into Dynamics 365 Customer Voice, providing you with additional survey capabilities and business benefits. The change is being introduced in phases and will be available in all geographical regions in the next few weeks, except for US Government Community Cloud customers. Dynamics 365 Customer Voice will be available on US Government Community Cloud by October 2020. For more information, see the [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p/?linkid=2128357) documentation.

It's important to have a plan for creating your surveys. Here are a few things to think about when you're creating surveys:

-   How do you want to collaborate? For example, do you want to share the survey as a template or invite other people to collaborate?

-   What's the purpose of your survey? For example, you might want to interact with your customers, promote new products or services, or measure customer satisfaction. If your goal is to measure something, what and how do you want to measure it?

-   How long do you want the survey to be? Keep in mind that longer surveys tend to have higher abandon rates. A good rule of thumb is to keep surveys shorter than five minutes, or no longer than 10 questions (depending on the type of questions you ask).

-   How many mandatory questions will you include in the survey? We recommend that you ask as few mandatory questions as possible.

-   How do you want to distribute your survey? For example, do you want to distribute it through individual email, QR code, or do you want to automate?

## Best practices for creating a survey

A few best practices enable you to create a meaningful survey and gather good responses from your customers. You can then analyze those responses and act on them in a way that best suits your organization. Some of the best practices for creating a survey are:

- **Define an objective**: Having an objective allows you to properly plan for your survey. It also allows you to identify what results you expect from your customers. Knowing how you'll use the responses helps you pick the right questions for your survey.

- **Keep the survey short**: If you create a survey that takes a long time to complete, you might reduce your response rate.

- **Create a logical flow of questions**: Ensure that your survey has a logical flow of questions to keep respondents interested.

- **Organize the survey**: Group related questions together.

- **Preview the survey**: After creating your survey, always preview it to check the overall flow of the survey and to catch any mistakes.

- **Mention expectations in the survey invitation**: In the survey invitation, be sure to mention the estimated time to complete it and give a brief overview. This will help respondents submit their input within the expected time frame.

## Best practices for creating a high-volume survey

A few best practices enable you to create an effective high-volume survey using Forms Pro:

- Make sure that you create the survey in a non-default environment. Microsoft Forms Pro (Default) uses the version of Common Data Service that has fixed service protection limits. More information: [Service Protection API Limits](https://docs.microsoft.com/powerapps/developer/common-data-service/api-limits)

  **Recommendation**: [Switch the environment](https://docs.microsoft.com/forms-pro/change-environment) to your existing production Common Data Service environment, or [create a new production environment](https://docs.microsoft.com/power-platform/admin/create-environment) from the [Power Platform admin center](https://admin.powerplatform.microsoft.com/).

- When you're sending a non-anonymous survey, avoid sending a large number of invitations through Power Automate at the same time. Sending more than eight individual survey invitations per minute might result in processing delays.

  **Recommendations:**
  - To send a large batch of invitations at once, use email. More information: [Send a survey by using email](https://docs.microsoft.com/forms-pro/send-survey-email) 
  - Customize the sender's email address to help recipients identify the survey with your company and improve the survey response rate. More information: [Customize sender email address](https://docs.microsoft.com/forms-pro/send-survey-email#customize-sender-email-address)

- When using Power Automate to automate survey response processing or follow-up, be sure to create the workflow by using the account that has the capacity to run the projected workflow volume.

  **Recommendation**: Set up the Power Automate workflow by using an account that has an appropriate Power Automate plan. More information: [Power Apps and Power Automate licensing FAQs](https://docs.microsoft.com/power-platform/admin/powerapps-flow-licensing-faq)

For any questions or assistance, please contact Microsoft support.

## Decide on the types of questions to ask<a name="decide-the-question-type"></a>

Deciding which types of questions you'll ask will help you organize your survey and maintain a good flow from one question to the next. The types of questions available in Forms Pro are Choice, Text, Rating, Date, Ranking, Net Promoter Score, and Likert.

### Choice

A Choice type question gives respondents a list of answers to choose from. You can decide whether to accept a single answer or multiple answers to the question. 

**Single-answer question**

By default, a choice question accepts a single answer. Respondents choose one answer from the list by selecting a radio button.

> [!div class=mx-imgBorder]
> ![A single-answer question, showing a list of choices with one radio button selected](media/ques-radio-button.png "A single-answer question, showing a list of choices with one radio button selected")

In single-answer questions, you can also display the list of answers in a drop-down list rather than radio buttons. Select **More settings for question** (...), and then select **Drop-down**.

> [!div class=mx-imgBorder]
> ![A drop-down question, showing a single answer selected in the drop-down list box](media/ques-drop-down.png "A drop-down question, showing a single answer selected in the drop-down list box") 

**Multiple-answer question**

You can accept multiple answers for your question by turning on the **Multiple answers** toggle. Respondents choose one or more answers from the list by selecting one or more check boxes.

> [!div class=mx-imgBorder]
> ![A multiple-answer question, showing a list of choices with check boxes](media/ques-check-box.png "A multiple-answer question, showing a list of choices with check boxes")

### Text

A Text type question can accept a short (one-line) answer or a long (multiple-line) answer. 

**Short-answer question**

By default, a text question accepts a short answer.

> [!div class=mx-imgBorder]
> ![A short-answer question displays a one-line text box](media/ques-short-answer.png "A short-answer question displays a one-line text box")

**Long-answer question**

You can accept multiple lines of text for your question by turning on the **Long answer** toggle.

> [!div class=mx-imgBorder]
> !["A long-answer question displays a multiple-line text box"](media/ques-long-answer.png "A long-answer question displays a multiple-line text box")

### Rating

A Rating type question asks respondents to rate their answer by using stars, numbers, or smiley symbols. 

By default, the star symbol is selected. To change the symbol, select it from the **Symbol** list. You can also change the number of levels by selecting a value from the **Levels** list. For number and star, up to 10 levels are supported. For smiley symbol, up to five levels are supported.

> [!NOTE]
> If you change the number of levels after sending the survey, the previously received responses won't be adjusted in accordance with the new level. For example, you sent a survey with a star rating question that had five levels, and received five responses with a three-star rating. Later, if you change the number of levels to 10, the previously received responses that have a three-star rating won't be adjusted to the 10-level scale.
  
Star and smiley rating questions with five levels are shown in the following images. 

> [!div class=mx-imgBorder]
> ![Example of a star rating question with five stars selected](media/ques-rating-star.png "Example of a star rating question with five stars selected") 

> [!div class=mx-imgBorder]
> ![Example of a smiley rating with the happiest face selected](media/ques-rating-smiley.png "Example of a smiley rating with the happiest face selected") 

For ratings questions that use numbers or stars, you can add labels for the numbers or stars by selecting **More settings for question** (...), and then selecting **Label**. A number rating question with labels is shown in the following image.

> [!div class=mx-imgBorder]
> ![Example of a number rating question with labels](media/ques-rating-number.png "Example of a number rating question with labels")

### Date

A Date type question displays a calendar and asks the respondent to select a date.

> [!div class=mx-imgBorder]
> ![Example of a date question with a date selected](media/ques-date.png "Example of a date question with a date selected")

### Ranking

A Ranking type question asks a respondent to rank items by arranging them in the order of the respondent's preference.

> [!div class=mx-imgBorder]
> ![Example of a ranking question](media/ques-ranking.png "Example of a ranking question")

### Net Promoter Score

A Net Promoter Score type question asks a respondent to rate the likelihood of their recommending a product or service to a friend.

> [!div class=mx-imgBorder]
> ![A Net Promoter Score question asks how likely the respondent is to give their recommendation](media/ques-nps.png "A Net Promoter Score question asks how likely the respondent is to give their recommendation")

### Likert

A Likert type question displays a list of single-answer questions and a rating scale for the answers, so a respondent can select a value from the scale to answer each question.

> [!div class=mx-imgBorder]
> ![An example Likert question that asks a respondent how satisfied they are with various aspects of a support call](media/ques-likert.png "An example Likert question that asks a respondent how satisfied they are with various aspects of a support call")

## Survey, question, response, and character limits

Forms Pro limits the number of surveys you can create, the number of questions you can add per survey, and the number of responses a survey can receive. The limits are:

- Surveys that can be created by a user: 200
- Questions allowed per survey: 100
- Responses a survey can receive: 500,000
- Characters allowed per response to a single question: 4,000
- Characters allowed for total responses per survey: 16,000

> [!NOTE]
> - For the **Likert** question type, each option counts as a single question.
> - A *response* is defined as a response to an entire survey, and not to the individual questions within the survey. When a respondent completes a survey and submits it, that survey is counted as having one response. For example, if a survey contains 10 questions and all the questions are answered by five respondents, the survey is counted as having five responses.

### See also

[Create a survey](create-survey.md)<br>
[Send a survey to get responses](send-survey.md) <br>
[Collaborate on a survey](collaborate-survey.md) <br>
[Analyze responses and invitations](analyze-responses-invites.md) <br>
[Work with environments](choose-environment.md)<br>
[Troubleshoot Forms Pro](troubleshoot.md)
