---
title: "Data flow | MicrosoftDocs"
description: "Learn about data flow in Forms Pro."
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/20/2020
ms.service: forms-pro
ms.topic: article
ms.custom: 
search.appverid:
  - FPR160
---

# Data flow in Forms Pro

> [!NOTE]
> Microsoft Forms Pro has evolved into Dynamics 365 Customer Voice, providing you with additional survey capabilities and business benefits. The change is being introduced in phases and will be available in all geographical regions in the next few weeks, except for US Government Community Cloud customers. Dynamics 365 Customer Voice will be available on US Government Community Cloud by October 2020. For more information, see the [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p/?linkid=2128357) documentation.

The following data flow diagram provides a visual representation of the flow of information (data) across Forms Pro services and Common Data Service. It also provides visual information about inputs and outputs of entities and processes. The data in the Forms Pro services area is stored in Microsoft managed storage in North America or Europe, and is encrypted by using Microsoft-managed keys. The data in the Common Data Service area is stored in users' Common Data Service organizations in the local datacenter.

![Data flow diagram for Forms Pro](media/dfd.png "Data flow diagram for Forms Pro")

The following processes are shown in the data flow diagram:

- **Create survey**: When a survey owner creates a survey, its data is stored in Forms Pro services and Common Data Service.

- **Distribute survey**: When a survey distributor sends a survey, the survey invitations are stored in Forms Pro services and Common Data Service. The survey invitation emails are sent to the recipients by using Dynamics 365 Marketing Email service internally.

  > [!NOTE]
  > You don't need an explicit subscription to Dynamics 365 Marketing to send emails.

- **Respond to survey**: When a respondent responds to a survey, the survey response is first stored in Forms Pro services and then sent to Azure Cognitive Services and the Forms Pro analytics engine for further processing. After responses are processed by Cognitive Services, they're stored in Common Data Service.

- **Analyze results**: After data is processed by the Forms Pro analytics engine, it's ready for analysis by viewing the information in charts in Forms Pro.
