---
title: "Manage existing projects | MicrosoftDocs"
description: "Instructions for managing existing projects with Customer Voice"
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Manage existing projects

Once you've created the required projects, they are available under the **All projects** tab. The following information is displayed about the projects:

- **Name**: Name of the project.
- **Modified date**: Date on which the project is modified.
- **Surveys**: Number of surveys created in the project.
- **Responses**: Total number of responses received across all surveys in the project.
- **Environment**: Environment in which the project is created.

You can also perform the following actions:

- **Rename**: Rename your project.
- **Copy**: Create a copy your project in the same or different environment.
- **Share**: Share your project with other people for collaboration.
- **Delete**: Delete the project that is not required anymore.

## Rename a project

1. Sign in to Customer Voice.

2. On the **All projects** tab, hover over the project to be renamed, select the ellipsis button `image`, and select **Rename**.

3. In the **Rename Project** dialog box, enter a new name, and select **Rename**.

    ![Rename a project](media/rename-project.png "Rename a project")

## Copy a project

You can create a copy of your project in the same environment or in different environment. Customer Voice gives the new project the same name as the existing project and appends `- copy` to it. You can rename the project, if you want.

`image of existing and copied project names`

**What is copied to the new project?**

The following are copied to the new project:

- **Surveys**: Surveys, along with their customizations, are copied as a new instance to the new project. 
- **Satisfaction metrics**: All satisfaction metrics that are configured for respective questions are copied to the new project. The satisfaction metrics retain their mappings with the questions in the newly created surveys in the new project. 
- **Power Automate flows**: All the Power Automate flows configured for the project are copied to the new project.
- **Email templates**: Email templates configured for the surveys are copied to the new project.

**What is not copied to the new project?**

Survey response data and satisfaction metrics data are not copied to the new project. 

**To copy a project**

1. Sign in to Customer Voice.

2. On the **All projects** tab, hover over the project to be copied, select the ellipsis button `image`, and select **Copy**.

    The **Copy project to** screen is displayed.

3. To copy your project in the same environment you are currently working in, select the environment listed under the **Current location** section.

4. To copy your project to a different environment, expand **All locations**, and select an environment.

5. After selecting an environment, select **Copy**. A notification is displayed at the top-right corner when the project is copied to the selected location.

## Share a project

You can share your project with multiple people in your organization so they can collaborate on the structure and layout of  surveys within the shared project. The people with whom the project is shared become the co-owners of the shared project. The projects that are shared with you are available under the **All projects** tab. 

**What a co-owner can do?**

A project co-owner has the same level of permissions as the project owner. This means a co-owner can create, edit, update, delete, and share the project. A co-owner can also remove the project owner from a shared project.

**What a co-owner cannot do?**

A project co-owner cannot delete a survey that is created by another user. The survey can be deleted only by the user who created it. If a co-owner tries to delete a project that contains a survey created by another user, an error is displayed. If a co-owner removes the project owner from a shared project that contains a survey created by the project owner, then the project cannot be deleted by the co-owner.

**How are the responses shared?**

If a project contains responses, only those responses will be shared with the co-owners that are received after the project is shared.

**To share a project**

1. Sign in to Customer Voice.

2. On the **All projects** tab, hover over the project to be shared, select the ellipsis button `image`, and select **Share**.

    `image`

3. In the **Collaborate on this project** panel, under the **Collaborate** tab, browse and select the name of user from the **Share project with** list. You can browse and select multiple users.

    `image`

4. Include an optional message, and then select **Collaborate**.

    The co-owners are displayed under the **Access** tab.

    `image`

**To remove a co-owner from the a project**

1. Sign in to Customer Voice.

2. On the **All projects** tab, hover over the project from which a co-owner needs to be removed, select the ellipsis button `image`, and select **Share**.

    `image`

3. In the **Collaborate on this project** panel, go to the **Access** tab, and select **Remove** `image` for the user to be removed.

    `image`

## Delete a project

You can delete a project that is not required anymore. Deleting a project removes its surveys, satisfaction metrics, email templates, survey response data, and satisfaction metrics data. The Power Automate flows associated with the surveys are deactivated. The deletion of a project is permanent and cannot be reverted.

**To delete a project**

1. Sign in to Customer Voice.

2. On the **All projects** tab, hover over the project to be deleted, select the ellipsis button `image`, and select **Delete**.

3. In the confirmation dialog box, select **Delete**.