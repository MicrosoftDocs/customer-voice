---
title: "Create a new survey"
description: "Instructions to create a new survey with Forms Pro, avoid phishing protection, restrict content allowed in answers, and mark questions for sentiment analysis"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 01/16/2020
ms.service: forms-pro
ms.topic: article
ms.assetid: EA713CA9-6B0B-45A3-A700-22C164465411
ms.custom: 
search.appverid:
  - FPR160
---

# Create a new survey

When you create a survey, you define the types of questions you want to ask to gauge a reader's response. In addition to formulating questions, you need to keep in mind additional considerations covered in this topic, such as how to avoid having your survey blocked by phishing prevention in Microsoft Forms Pro, how to get the responses you want by restricting the type of answers you allow in text-based questions, and whether you want to mark answers for sentiment analysis.

## Create a new survey with Forms Pro

1.	Sign in to Forms Pro with your Office 365 credentials.

2.	Under **My Forms**, select **New Pro Survey**.

    > [!div class=mx-imgBorder]
    > ![New survey](media/new-survey-button.png "New survey")

3.	Select the default survey title, and then enter a title for your survey. You can also enter an optional description for it.

    > [!div class=mx-imgBorder]
    > ![Add survey title and description](media/survey-title.png "Add survey title and description") 

4.	Select **Add new** to view question types that can be added to your survey. You can choose from **Choice**, **Text**, **Rating**, or **Date** questions. You can also select **More** (...), and choose **Ranking**, **Likert**, or **Net Promoter Score** questions.

    > [!div class=mx-imgBorder]
    > ![Question types](media/ques-types.png "Question types")

5.	Select the question types you want to add.

6.	Enter the question text and its answer options. The survey is saved automatically.

    > [!div class=mx-imgBorder]
    > ![Survey](media/survey.png "Example of a survey with different question types")

7. To change the order of questions in the survey, select a question, and then select the up or down arrow on the right side of each question to move it up or down.

8. To hide a question from being displayed in the survey, move the **Visible** toggle to the Off position. By default, this toggle is turned on. You can show the question to the responder based on a branching rule. More information: [Create a branching rule](create-branching-rule.md)

    > [!div class=mx-imgBorder]
    > ![Set question visibility](media/visibility-option.png "Set the visibility of a question")

> [!NOTE]
> - You can personalize your survey by adding custom data to the questions. More information: [Personalize a survey](personalize-survey.md)
> - You can apply formatting to the survey elements, such as survey title, survey description, question text, and question subtitle. More information: [Format text in a survey](survey-text-format.md)
> - You can customize the look of your survey by applying your own formatting to survey elements such as the title, description, questions, and question subtitles. More information: [Format text in a survey](survey-text-format.md)
> - You can create a classic form within Forms Pro. More information: [Create a classic form](create-classic-form.md)
> - You can also create quizzes within Forms Pro to get real-time feedback. More information: [Create a quiz with Microsoft Forms](https://support.office.com/article/create-a-quiz-with-microsoft-forms-a082a018-24a1-48c1-b176-4b3616cdc83d)

<a name="proactive-phishing-prevention"></a>

## Avoid having your survey blocked by Forms Pro phishing prevention

*Phishing attacks* attempt to steal sensitive information through emails, websites, text messages, or other forms of electronic communication that appear to be official communication from legitimate companies or individuals. Phishers often attempt to steal passwords or other credentials.

In Forms Pro, we've enabled automated machine reviews to proactively detect malicious password collection in surveys.

### Survey designer experience

If you've designed a survey that includes questions that require a respondent to provide their password, account information, or other security information, the survey will be automatically blocked and can't be distributed. The administrator will receive a notification and an option to unblock the survey. If you want to distribute the survey, you must contact your administrator to unblock it.

### Administrator experience

When a survey is blocked automatically, the administrator receives a daily notification in **Message center** with an option to unblock the survey. More information: [Review and unblock forms detected and blocked for potential phishing](https://support.office.com/article/review-and-unblock-forms-detected-and-blocked-for-potential-phishing-879a90d7-6ef9-4145-933a-fb53a430bced)

## Add restrictions in text-based questions

When you create a text-based question (that is, a question of type Text), you can add restrictions to the kind of answers you'll accept from your respondents. For example, you can restrict their answers to be a number, an email address, or a string in a predefined format (based on a [regular expression](https://docs.microsoft.com/dotnet/standard/base-types/regular-expression-language-quick-reference)) such as a booking ID.

1. In the text-based question, select **More settings for question** (...), and then select **Restrictions**.
2. Select one of the following options from the **Restrictions** list:
    - **Number**: Only accept input in number format. You can select from various options such as **Only number**, **Greater than**, **Less than**, **Between**, and others.
    - **Email**: Only accept input that's a valid email address.
    - **Custom**: Define a regular expression, and only accept input that matches the defined expression. You can also add an optional description to the regular expression suggesting user the format in which the text input is expected. Let's say you want to define a character limit for the text input field that allows entering up to 200 English characters. You'll enter the regular expression as `\b[A-Za-z0-9]{200}\b`.

## Calculate sentiments from responses to text-based questions

You can use sentiment analysis to determine whether user responses for a survey are positive, neutral, or negative. Sentiments are calculated from responses to the text-based questions you've selected. To select text-based questions for sentiment analysis, go to the text-based question, and move the **Sentiment** toggle to the On position. By default, this toggle is turned off. If you don't select any text-based question for sentiment analysis, sentiment data won't be generated.

### See also

[Apply a theme to a survey](apply-theme.md)<br>
[Preview and test a survey](preview-test-survey.md)<br>
[Create a branching rule](create-branching-rule.md)<br>
[Personalize a survey](personalize-survey.md)<br>
[Format text in a survey](survey-text-format.md)<br>
[Create a classic form](create-classic-form.md)<br>
[Create a multilingual survey](create-multilingual-survey.md)<br>
[Create a multiple-page survey](create-multipage-survey.md)
