---
title: "Save survey progress | MicrosoftDocs"
description: "This topic explains how to save a survey's progress and enable a user to complete a survey in multiple sittings."
ms.date: 09/21/2022
ms.topic: article
author: sbmjais
ms.author: shjais
---

# Save a survey in progress

When a respondent starts a survey, they can either complete it in one go or in multiple sittings. When respondents complete a survey in multiple sittings, they begin the survey and then close it. Their responses are saved, so when they reopen the survey, those responses are retrieved and the survey starts again from where they left off. The responses that are saved temporarily until the survey is submitted are known as *paused responses*.

Paused responses are available for 28 days from the date when a respondent opens the survey. A respondent can return to the survey and submit the responses within 28 days. Paused responses are available across web browsers and devices. This means that a respondent can open a survey on their computer's web browser and later complete it from the browser on their mobile device. The most recent data is retrieved and shown to the respondent. After a response is submitted, it can't be edited.

> [!NOTE]
> - The survey progress is saved only for the surveys sent through personalized links. More information: [Work with personalized links](distribution-settings.md#work-with-personalized-links)
> - Paused responses aren't available in Dynamics 365 Customer Voice until they're submitted. They'll be available in reports only after a respondent submits the survey.
> - Paused responses are deleted if the survey author changes the structure of the survey after the invitation is sent, for example by adding or deleting questions, or changing their order.
> - The capability to save a survey in progress is not available for surveys that are migrated from Microsoft Forms Pro to Dynamics 365 Customer Voice.

## Survey author experience

By default, this feature is turned off and a survey in progress isn't saved. As a survey author, you can turn on the **Save survey progress** toggle in the **Participants** section on the **Distribution** panel to turn on this feature. Respondents can answer a few questions, close the survey, and then return later to complete it and submit their responses. When you turn off this feature after it has been turned on, existing paused responses are deleted, if there are any. More information: [Work with survey distribution settings](distribution-settings.md#participants)

## Survey respondent experience

You've sent a product feedback survey through a personalized link to your customer named Henry. The survey contains four questions. Let's understand Henry's experience through the following scenarios:

**Scenario 1**: Henry opens the survey in a computer's web browser, answers the first two questions, and then closes the survey without submitting it. A few days later, Henry opens the survey on a mobile device. The survey starts from where Henry left off. Henry modifies the response to the earlier questions, answers the remaining questions, and then submits the survey. Responses are sent to Dynamics 365 Customer Voice.

**Scenario 2**: Henry opens the survey, answers all the questions, and then submits the survey. Henry reopens the survey from the invitation link. One of the following occurs:

- If **One response per person** is turned off, Henry can submit another response for the same survey.
- If **One response per person** is turned on, Henry sees a message that a response has already been submitted.

### See also

[Work with survey distribution settings](distribution-settings.md)<br>
[Send a survey by using the built-in email composer](send-survey-email.md)<br>
[Send a survey by using Power Automate](send-survey-flow.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
