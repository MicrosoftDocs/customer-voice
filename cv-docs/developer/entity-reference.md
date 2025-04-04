---
title: "Entity Reference for Dynamics 365 Customer Voice | MicrosoftDocs"
description: "Reference documentation for the entities of Microsoft Dynamics 365 Customer Voice."
ms.date: 10/12/2021
ms.topic: "reference"
author: "sbmjais"
ms.author: "shjais"
search.audienceType: 
  - developer
---

# Entity Reference for Dynamics 365 Customer Voice

Use this reference to understand the available operations that can be performed on specific entities, the default attributes of each entity, and the relationship between entities.

Following is a simplified version of the entity relationship diagram of Dynamics 365 Customer Voice entities. You can generate a detailed entity relationship diagram of  Dynamics 365 Customer Voice entities using the [Metadata Diagram tool](https://code.msdn.microsoft.com/Sample-of-generating-a0ba0e47). To do this, you will just have to mention the entity logical names as parameters while executing the sample. More information: [Use metadata to generate entity diagrams](/dynamics365/customer-engagement/developer/use-metadata-generate-entity-diagrams).

> [!div class=mx-imgBorder]
> ![Simplified entity relationship diagram.](../media/er-diagram.png "Simplified entity relationship diagram")

## Entities

|Entity name|Description|
|------|------|
|[msfp_alert](entities/msfp_alert.md)|Alerts created in Customer Voice.|
|[msfp_alertrule](entities/msfp_alertrule.md)|Rule for creating alerts in Customer Voice.|
|[msfp_emailtemplate](entities/msfp_emailtemplate.md)|Template for an email message that contains the survey invitation link.|
|[msfp_localizedemailtemplate](entities/msfp_localizedemailtemplate.md)|Stores localized data for email templates.|
|[msfp_question](entities/msfp_question.md)|Question in a survey to collect feedback.|
|[msfp_questionresponse](entities/msfp_questionresponse.md)|Response to a question in a survey.|
|[msfp_survey](entities/msfp_survey.md)|Set of questions to collect feedback.|
|[msfp_surveyinvite](entities/msfp_surveyinvite.md)|Activity that tracks a survey invitation sent to a person.|
|[msfp_surveyreminder](entities/msfp_surveyreminder.md)|Email reminders for surveys created in Customer Voice.|
|[msfp_surveyresponse](entities/msfp_surveyresponse.md)|Response to a survey.|
|[msfp_project](entities/msfp_project.md)|Set of surveys to collect feedback.|
|[msfp_unsubscribedrecipient](entities/msfp_unsubscribedrecipient.md)|Email address of an unsubscribed respondent.|
|[msfp_satisfactionmetric](entities/msfp_satisfactionmetric.md)|Satisfaction metric defined for a project.|


[!INCLUDE[footer-include](../includes/footer-banner.md)]
