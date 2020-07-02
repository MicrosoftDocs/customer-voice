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

- **Copy**: Create a copy your survey in the same or another project in the same or another environment.
- **Move**: Move a survey to another project in the same or another environment.
- **Rename**: Rename your survey.
- **Delete**: Delete the survey that is not required anymore.
- **Share**: Share your survey with other people for collaboration.

## Copy a survey

You can create a copy of your survey in the same or another project in the same or another environment. When you copy a project, surveys, customizations, satisfaction metrics, Power Automate flows, and email templates are also copied to the new project. The satisfaction metrics retain their mappings with the questions in the newly created survey in the new project. However, survey response data and satisfaction metrics data are not carried over to the new project. Customer Voice gives the new project the same name as the existing project and appends `- copy` to it. You can rename the project, if you want.

`image of existing and copied survey names`

## Move a survey

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