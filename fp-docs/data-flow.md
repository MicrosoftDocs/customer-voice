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
<!--I'm a bit leery of using "data flow" because of its specific meaning in Power BI, but I can't find any good alternative.-->
The following data flow diagram provides a visual representation of the flow of information (data) across Forms Pro services and Common Data Service. It also provides visual information about inputs and outputs of entities and processes. The data in the Forms Pro services area is stored in Microsoft managed storage in North America or Europe, and is encrypted by using Microsoft-managed keys<!--I base this edit on usage in https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption, which please see. I haven't seen "managed keys" used as a standalone term.-->. The data in the Common Data Service area is stored in users' Common Data Service organizations in the local datacenter.<!--I like this diagram! It's very clear. -->

![Data flow diagram for Forms Pro](media/dfd.png "Data flow diagram for Forms Pro")

The following processes are shown in the data flow diagram:

- **Create survey**: When a survey owner creates a survey, its data is stored in Forms Pro services and Common Data Service.

- **Distribute survey**: When a survey distributor sends a survey, the survey invitations are stored in Forms Pro services and Common Data Service. The survey invitation emails are sent to the recipients by using Dynamics 365 Marketing Email service internally.

  > [!NOTE]
  > You don't need an explicit subscription to Dynamics 365 Marketing to send emails.

- **Respond to survey**: When a respondent responds to a survey, the survey response is first stored in Forms Pro services and then sent to Azure Cognitive Services and the Forms Pro analytics engine for further processing. After responses are processed by Cognitive Services, they're stored in Common Data Service.

- **Analyze results**: After data is processed by the Forms Pro analytics engine, it's ready for analysis by viewing the information in charts in Forms Pro.