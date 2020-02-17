---
title: "Plan a survey | MicrosoftDocs"
description: "Instructions for planning a survey with Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 02/17/2020
ms.service: forms-pro
ms.topic: article
ms.assetid: FD23CE2B-B022-4708-BAE8-5CAC8BC75092
ms.custom: 
search.appverid:
  - FPR160
---

# Plan to create a survey

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

## Decide on the types of questions to ask<a name="decide-the-question-type"></a>

Deciding which types of questions you'll ask will help you organize your survey and maintain a good flow from one question to the next. The types of questions available in Forms Pro are Choice, Text, Rating, Date, Ranking, Net Promoter Score, and Likert.

### Choice
<!--from editor: For accessibility reasons I think you need to have text under each heading, not just a graphic. I rearranged the paragraphs because I believe the radio buttons and drop-down format are both ways to present a question that has a single answer. I thought it was confusing to say a Choice question could have single or multiple answers ~or~ be a drop-down, when I don't think drop-down is actually a type of Choice question, just a different way to display a single-answer question. If I'm wrong, please excuse!-->
A Choice type question gives respondents a list of answers to choose from. You can decide whether to accept a single answer or multiple answers to the question. 
<!--from editor: Suggest making the alt text more descriptive, since the graphics are conveying real information here.-->
**Single-answer question**
<!--from editor: In the following graphic, recommend changing the question to "How knowledgeable was your customer service representative?". The third option should be "Needs to learn about the product."-->

By default, a choice question accepts a single answer. Respondents choose one answer from the list by selecting a radio button.

![A single-answer question, showing a list of choices with one radio button selected](media/ques-radio-button.png "A single-answer question, showing a list of choices with one radio button selected")

In single-answer questions, you can also display the list of answers in a drop-down list rather than radio buttons. Select **More settings for question** (...), and then select **Drop-down**.
<!--from editor: Question should be "How knowledgeable was your customer service representative?" -->
![A drop-down question, showing a single answer selected in the drop-down list box](media/ques-drop-down.png "A drop-down question, showing a single answer selected in the drop-down list box") 

**Multiple-answer question**

You can accept multiple answers for your question by turning on the **Multiple answers** toggle. Respondents choose one or more answers from the list by selecting one or more check boxes.
<!--from editor: In the following graphic, recommend changing the question to "What do you like about our product?" and including "None of the above" as one of the choices. As a survey respondent, I'd want to have that option - especially if the survey won't progress to the next question unless I give at least one answer. Which makes me curious: Can the respondent leave this type of question blank? If not, it seems that "None of the above" must be one of the choices.-->
![A multiple-answer question, showing a list of choices with check boxes](media/ques-check-box.png "A multiple-answer question, showing a list of choices with check boxes")

### Text

A Text type question can accept a short (one-line) answer or a long (multiple-line) answer. 

**Short-answer question**

By default, a text question accepts a short answer. <!--from editor: Can the reader decide what text (if any) appears here by default?-->

![A short-answer question displays a one-line text box](media/ques-short-answer.png "A short-answer question displays a one-line text box")

**Long-answer question**

You can accept multiple lines of text for your question by turning on the **Long answer** toggle. <!--from editor: Is there anything you can say here about the maximum number of characters for a long answer? Is there any way for the reader to define what text appears by default in the text box, or does it have to be "Enter your answer"?-->

!["A long-answer question displays a multiple-line text box"](media/ques-long-answer.png "A long-answer question displays a multiple-line text box")

### Rating

A Rating type question asks respondents to rate their answer by using stars, numbers, or sentiment icons that range from frowning to smiley faces<!--If "Smiley" is the tooltip for the symbol, or you use "smiley" elsewhere in the UI, maybe this is a good way to make the association? -->. 

By default, the star symbol is selected. To change the symbol, select it from the **Symbol** list. You can also change the number of levels <!--edit okay?--> by selecting a value from the **Levels** list. For number and star, up to <!--edit okay?-->10 levels are supported. For smiley (sentiment icons), up to five levels are supported.
  
Star and sentiment icon ratings with five levels are shown in the following images. 

![Example of a star rating question with five stars selected](media/ques-rating-star.png "Example of a star rating question with five stars selected") 

![Example of a sentiment icon rating with the happiest face selected](media/ques-rating-smiley.png "Example of a sentiment icon rating with the happiest face selected") 

For ratings questions that use numbers or stars, you can add labels for the numbers or stars by selecting **More settings for question** (...), and then selecting **Label**. A number rating question with labels is shown in the following image.

![Example of a number rating question with labels](media/ques-rating-number.png "Example of a number rating question with labels")

### Date

A Date type question displays a calendar and asks the respondent to select a date.
<!--from editor: I suppose it's okay the person who answered this question is three years old? :) -->
![Example of a date question with a date selected](media/ques-date.png "Example of a date question with a date selected")

### Ranking

A Ranking type question asks a respondent to rank items by arranging them in the order of the respondent's preference.
<!--from editor: Suggest that the question read "Arrange the following items in the order of your preference, starting with the one you like best."-->
![Example of a ranking question](media/ques-ranking.png "Example of a ranking question")

### Net Promoter Score

A Net Promoter Score type question asks a respondent to rate the likelihood of their recommending a product or service to a friend.

![A Net Promoter Score question asks how likely the respondent is to give their recommendation](media/ques-nps.png "A Net Promoter Score question asks how likely the respondent is to give their recommendation")

### Likert

A Likert type question displays a list of single-answer questions and a rating scale for the answers, so a respondent can select a value from the scale to answer each question.

![An example Likert question that asks a respondent how satisfied they are with various aspects of a support call](media/ques-likert.png "An example Likert question that asks a respondent how satisfied they are with various aspects of a support call")

### See also

[Create a survey](create-survey.md)<br>
[Send a survey to get responses](send-survey.md) <br>
[Collaborate on a survey](collaborate-survey.md) <br>
[Analyze responses and invitations](analyze-responses-invites.md) <br>
[Work with environments](choose-environment.md)<br>
[Troubleshoot Forms Pro](troubleshoot.md)