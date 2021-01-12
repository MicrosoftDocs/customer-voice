---
title: "Save survey progress | MicrosoftDocs"
description: "Instructions for saving a survey's progress in Dynamics 365 Customer Voice."
ms.date: 01/15/2021
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Save survey progress

When a respondent starts a survey, they can either complete it in one go or in multiple sittings. Respondents who complete a survey in multiple sittings, their responses are saved and then retrieved when they reopen the survey. The survey starts from where they left off earlier. The responses that are saved temporarily until a survey is submitted are known as paused responses.

Paused responses are available for 28 days from the date when a respondent opens the survey. A respondent can return to the survey and submit the responses within 28 days. Paused responses are available across web browsers and devices. This means, a respondent can open a survey on their computer's web browser and later complete it from their mobile's web browser. The most recent data is retrieved and shown to the respondent. Once a response is submitted, it cannot be edited.

> [!NOTE]
> - The survey progress would be saved only for the surveys sent through personalized links. To know more about personalized links, see [Work with personalized links](distribution-settings.md#work-with-personalized-links).
> - Paused responses are not available in Dynamics 365 Customer Voice until they are submitted. They will be available in reports only after a respondent submits the survey.
> - Paused responses are deleted if the survey author changes the structure of the survey after the invitation is sent, for example, adding new questions, deleting the existing ones, or changing the question order.

## Survey author experience

By default, this feature is turned off and a survey's progress is not saved. As a survey author, you can turn on the **Save survey progress** toggle under the **Participants** section in the **Distribution** panel to turn on this feature. Respondents can answer a few questions, close the survey, and then return later to complete and submit the responses. When you turn off this feature after it's turned on, the existing paused responses are deleted, if available. More information: [Work with survey distribution settings](distribution-settings.md#participants)

## Survey respondent experience

You've sent a product feedback survey though personalized links to your customers named Henry. The survey contains four questions. Let's understand Henry's experience through the following scenarios:

**Scenario 1**: Henry opens the survey in his computer's web browser, answers the first two questions, and then closes the survey without submitting it. A few days later, he opens the survey in his mobile device. The survey starts from where he left off. Henry  modifies the response to earlier questions, answers the remaining questions, and then submits the survey. Responses are now sent to Dynamics 365 Customer Voice.

**Scenario 2**: Henry opens the survey, answers all the questions, and then submits the survey. He reopens the survey from the invitation link. The following are the possibilities:
- If **One response per person** is turned off, Henry can submit another response for the same survey.
- If **One response per person** is turned on,  message is displayed that a response is already submitted.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using email](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)