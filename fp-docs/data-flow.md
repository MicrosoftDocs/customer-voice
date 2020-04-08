---
title: "Data flow | MicrosoftDocs"
description: "Learn about data flow in Forms Pro."
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/15/2020
ms.service: forms-pro
ms.topic: article
ms.custom: 
search.appverid:
  - FPR160
---

# Data flow in Forms Pro

The following data flow diagram provides a visual representation of the flow of information (data) across Forms Pro services and Common Data Service. It also provides visual information about inputs and outputs of entities and processes. The data under Forms Pro services area is stored within Microsoft managed storage in North America or Europe and is encrypted with Microsoft managed key. The data under Common Data Service area is stored in users' Common Data Service organization in the local data center.

![Data flow diagram of Forms Pro](media/dfd.png "Data flow diagram of Forms Pro")

Following processes are shown in the data flow diagram:

- **Create survey**: When a survey owner creates a survey, its data is stored under Forms Pro services and Common Data Service.

- **Distribute survey**: When a survey distributor sends a survey, the survey invitations are stored in Forms Pro services and Common Data Service. The survey invitation emails are sent to the recipients by using Dynamics 365 Marketing Email service internally.

  > [!NOTE]
  > You would not need an explicit subscription to Dynamics 365 Marketing to send emails.

- **Respond to survey**: When a respondent responds to a survey, the survey response is first stored in Forms Pro services and then sent to Azure Cognitive Services, and Forms Pro analytics engine for further processing. After responses are processed by Azure Cognitive Services, they are stored in Common Data Service.

- **Analyze results**: After data is processed in by Forms Pro analytics engine, it is ready for analysis in Forms Pro. It enables you to view information by using charts.