---
title: "Transition from Forms Pro | MicrosoftDocs"
description: "Learn what data is migrated when you transition from Forms Pro to Dynamics 365 Customer Voice."
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Transition from Forms Pro to Dynamics 365 Customer Voice

With the release of Dynamics 365 Customer Voice on July 21, 2020, all your surveys from Forms Pro will be moved to Dynamics 365 Customer Voice and you'll be able to perform all the actions in Dynamics 365 Customer Voice that you performed<!--Suggested.--> in Forms Pro. The transition period will last 45 days.

## How will the data be migrated?
<!--Suggest using bullets for this section because these paragraphs all "stand alone," they don't really tell a story. Also, I tried to make the verb tenses parallel (that is, present/past tense -> future tense).-->
- All your surveys from Forms Pro will be migrated as individual projects in Dynamics 365 Customer Voice. This means that each project will contain one survey. You'll be able to see all your projects on the **All projects** tab.

- If you created a shared survey in Forms Pro, a shared project will be created and the survey will be shared between them.<!--Edit okay? I didn't quite understand what "with the survey shared" meant.-->

- If you created a flow for your surveys in Forms Pro, it will be available at the survey level in Dynamics 365 Customer Voice.

- If you added a Net Promoter Score (NPS) question or tagged a text question for sentiment analysis, the corresponding NPS and sentiment metrics will be created in Dynamics 365 Customer Voice. A dashboard will be automatically created for each set of metrics, showcasing recent scores and trends. The dashboard will be available on the **Reports** tab.

- If you created a bookmark for a Forms Pro survey, you'll be redirected to the corresponding project in Dynamics 365 Customer Voice.

- If you're currently<!--Edit okay?--> a trial user in Forms Pro, your data won't be migrated to Dynamics 365 Customer Voice.

- If you created a survey in the default environment, the data will be migrated to the currently available default environment.

## Experience for users based on their license

The transition experience differs based on the product license you have. This section provides details.

**Experience for users with only a Forms Pro license**

If you have only a Forms Pro license and try to sign in to Forms Pro, the following message will be displayed with a link to go to Dynamics 365 Customer Voice.

`image`

**Experience for users with both Forms and Forms Pro licenses**

If you have licenses for both Forms and Forms Pro, and have created surveys in Forms Pro, the following message is displayed where you can choose<!--Suggested.--> to go to Dynamics 365 Customer Voice or stay in Forms.

![Forms Pro move message](media/forms-pro-move-message.png "Forms Pro move message") 

If you choose to stay in Forms, the following message is displayed at the top of the page, stating that your Forms Pro surveys are available in Dynamics 365 Customer Voice and won't be available through Forms after the transition period is over.<!-- Suggested, so the graphic won't contain information that the text doesn't contain.-->

![Forms Pro move message bar](media/forms-pro-move-message-bar.png "Forms Pro move message bar") 

If you select a survey tile, you're redirected to the corresponding project in Dynamics 365 Customer Voice.

**Experience for users with only a Forms license**

If you have a Forms-only license and try to sign in to Forms Pro, the Forms home page is displayed.

**Experience for a new user**

If you're a new user and try to sign in to Forms Pro, an error is displayed. You must sign in to Dynamics 365 Customer Voice to create surveys.
