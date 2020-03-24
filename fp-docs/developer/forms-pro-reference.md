---
title: "Entity Reference for Microsoft Forms Pro | MicrosoftDocs"
description: "Reference documentation for the entities of Microsoft Forms Pro."
keywords: 
author: "susikka"
ms.author: "susikka"
manager: "shujoshi"
applies_to: 
ms.date: 03/24/2020
ms.service: "forms-pro"
ms.topic: "reference"
ms.assetid: 0CCDE7D8-E6D8-4892-B293-A4F39DEE4B06
ms.custom: 
search.audienceType: 
  - developer
search.app: 
  - PowerApps
  - D365CE
search.appverid:
  - FPR160
---

# Entity Reference for Microsoft Forms Pro

Use this reference to understand the available operations that can be performed on specific entities, the default attributes of each entity and the relationship between entities.

Following is a simplified version of the entity relationship diagram of Forms Pro entities. You can generate a detailed entity relationship diagram of Forms Pro entities using the [Metadata Diagram tool](https://code.msdn.microsoft.com/Sample-of-generating-a0ba0e47). To do this, you will just have to mention the entity logical names as parameters while executing the sample. More information: [Use metadata to generate entity diagrams](https://docs.microsoft.com/dynamics365/customer-engagement/developer/use-metadata-generate-entity-diagrams).

> [!div class=mx-imgBorder]
> ![Simplified entity relationship diagram](../media/er-diagram.png "Simplified entity relationship diagram")

## Entities

|Entity name|Description|
|------|------|
|[msfp_emailtemplate](reference/entities/msfp_emailtemplate.md)|Template for an email message that contains the survey invitation link.|
|[msfp_question](reference/entities/msfp_question.md)|Question in a survey to collect feedback.|
|[msfp_questionresponse](reference/entities/msfp_questionresponse.md)|Response to a question in a survey.|
|[msfp_survey](reference/entities/msfp_survey.md)|Set of questions to collect feedback.|
|[msfp_surveyinvite](reference/entities/msfp_surveyinvite.md)|Activity that tracks a survey invitation sent to a person.|
|[msfp_surveyresponse](reference/entities/msfp_surveyresponse.md)|Response to a survey.|
|[msfp_unsubscribedrecipient](reference/entities/msfp_unsubscribedrecipient.md)|Email address of an unsubscribed respondent.|

### See also

[Developer guide for Forms Pro](developer-guide.md)<br />
[Entity reference for Microsoft Dynamics 365](/dynamics365/customer-engagement/developer/about-entity-reference)
