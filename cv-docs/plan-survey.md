---
title: "Plan a survey | MicrosoftDocs"
description: "Instructions for planning a survey with Customer Voice"
ms.date: 08/31/2020
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Plan to create a survey

It's important to have a plan for creating your surveys. Here are a few things to think about when you're creating surveys:

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

A few best practices enable you to create an effective high-volume survey using Customer Voice:

- Make sure that you create the project in a non-default environment. Dynamics 365 Customer Voice (Default) uses the version of Common Data Service that has fixed service protection limits. More information: [Service Protection API Limits](https://docs.microsoft.com/powerapps/developer/common-data-service/api-limits)

  **Recommendation**: [Create a project](create-project.md) in your existing production Common Data Service environment, or [create a new production environment](https://docs.microsoft.com/power-platform/admin/create-environment) from the [Power Platform admin center](https://admin.powerplatform.microsoft.com/).

- When you're sending a non-anonymous survey, avoid sending a large number of invitations through Power Automate at the same time. Sending more than eight individual survey invitations per minute might result in processing delays.

  **Recommendations:**
  - To send a large batch of invitations at once, use email. More information: [Send a survey by using email](send-survey-email.md) 
  - Customize the sender's email address to help recipients identify the survey with your company and improve the survey response rate. More information: [Customize sender email address](customize-sender-email.md)

- When using Power Automate to automate survey response processing or follow-up, be sure to create the workflow by using the account that has the capacity to run the projected workflow volume.

  **Recommendation**: Set up the Power Automate workflow by using an account that has an appropriate Power Automate plan. More information: [Power Apps and Power Automate licensing FAQs](https://docs.microsoft.com/power-platform/admin/powerapps-flow-licensing-faq)

For any questions or assistance, please contact Microsoft support.

## Survey, question, response, and character limits

Dynamics 365 Customer Voice has a limit on the number of surveys you can create, number of questions you can add per survey, and number of responses a survey can receive. The limits are:

- Number of surveys that can be created by a user: 200 (including forms and quizzes if you have Microsoft Forms license)
- Number of questions allowed per survey: 100
- Number of responses a survey can receive: 500,000
- Number of characters allowed per response for a single question: 4,000
- Number of characters allowed for total responses per survey: 16,000

> [!NOTE]
> - For the **Likert** question type, each option counts as a single question.
> - A response is defined as a response to an entire survey, and not to the individual questions within the survey. When a respondent completes a survey and submits it, it is counted as one response. For example, if a survey contains 10 questions and all of the questions are answered by five respondents, the survey will count as having five responses.

### See also

[Create a project](create-project.md)<br>
[Send a survey to get responses](send-survey.md) <br>
[Connect Dynamics 365 Customer Voice with your environment](connect-environment.md)<br>
