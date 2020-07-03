---
title: "Manage existing surveys | MicrosoftDocs"
description: "Instructions for managing existing surveys with Customer Voice"
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Manage existing surveys

Once you've created the required survey or multiple surveys within a project, you can perform the following actions:

- **Copy**: Create a copy your survey in the same or different project in the same environment.
- **Move**: Move a survey to a different project in the same environment.
- **Rename**: Rename your survey.
- **Delete**: Delete the survey that is not required anymore.
- **Share**: Share your survey with other people for collaboration.

## Copy a survey

You can create a copy of your survey in the same or a different project in the same environment. Customer Voice gives the new survey the same name as the existing survey and appends `Copy` to it. You can rename the survey, if you want.

`image of existing and copied survey names`

**What is copied to the new survey?**

Survey, along with its customizations, is copied as a new survey. 

**What is not copied to the new survey?**

The following are not copied to the new survey:

- Satisfaction metrics and their data
- Power Automate flows
- Email templates
- Survey response data

**To copy a survey**

1. Open the project in which a survey needs to be copied.

2. Hover over the survey to be copied, select the ellipsis button `image`, and select **Copy**.

    The **Copy to** screen is displayed.

3. To copy your survey in the same project you are currently working in, select the project listed under the **Current project** section.

4. To copy your survey to a different project, expand **All Projects**, and select a project.

5. After selecting the project, select **Copy**. A notification is displayed at the top-right corner when the project is copied successfully.

## Move a survey

You can move a survey to a different project in the same environment. This helps you move similar surveys under one project. 

## Rename a survey

1. Open the project in which a survey needs to be renamed.

2. Hover over the survey to be renamed, select the ellipsis button `image`, and select **Rename**.

3. In the **Rename your survey** dialog box, enter a new name, and select **Rename**.

## Delete a survey

You can delete a survey that is not required anymore. Deleting a survey removes its associated satisfaction metrics, email templates, survey response data, and satisfaction metrics data. The Power Automate flows associated with the surveys are deactivated. The deletion of a survey is permanent and cannot be reverted.

If a project has only one survey, deleting a survey will also delete the project. If a project has multiple surveys, only the survey is deleted.

If a satisfaction metric is mapped to the questions of the survey being deleted, the satisfaction metric is also deleted. If a satisfaction metric is mapped to the questions of multiple surveys, the data of the survey being deleted is not included for further calculation.

**To delete a survey**

1. Open the project from which a survey needs to be deleted.

2. Hover over the survey to be deleted, select the ellipsis button `image`, and select **Delete**.

3. In the confirmation dialog box, select **Delete**.

## Share a survey

You can share your survey with multiple people in your organization so they can collaborate on the structure and layout of  the survey. 