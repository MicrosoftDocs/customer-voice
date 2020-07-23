---
title: "Data flow | MicrosoftDocs"
description: "Learn about data flow in Dynamics 365 Customer Voice."
ms.date: 07/29/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Data flow in Dynamics 365 Customer Voice

The following data flow diagram provides a visual representation of the flow of information (data) across Customer Voice services and Common Data Service. It also provides visual information about inputs and outputs of entities and processes. The data in the Customer Voice services area is stored in Microsoft managed storage in North America or Europe, and is encrypted by using Microsoft-managed keys. The data in the Common Data Service area is stored in users' Common Data Service organizations in the local datacenter.

![Data flow diagram for Customer Voice](media/dfd.png "Data flow diagram for Customer Voice")

The following processes are shown in the data flow diagram:

- **Create project**: When a project owner creates a project, its data is stored in Customer Voice services and Common Data Service.

- **Distribute survey**: When a survey distributor sends a survey, the survey invitations are stored in Customer Voice services and Common Data Service. The survey invitation emails are sent to the recipients by using Dynamics 365 Marketing Email service internally.

  > [!NOTE]
  > You don't need an explicit subscription to Dynamics 365 Marketing to send emails.

- **Respond to survey**: When a respondent responds to a survey, the survey response is first stored in Customer Voice services and then sent to Azure Cognitive Services and the Customer Voice analytics engine for further processing. After responses are processed by Cognitive Services, they're stored in Common Data Service.

- **Analyze results**: After data is processed by the Customer Voice analytics engine, it's ready for analysis by viewing the information in charts in Customer Voice.