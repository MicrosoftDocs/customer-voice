---
title: "Manage projects | MicrosoftDocs"
description: "Instructions for managing projects with Dynamics 365 Customer Voice"
ms.date: 07/29/2020
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Manage projects

After you've created the projects you need, they're available on the **All projects** tab. The following information is displayed:

- **Name**: The name of the project.
- **Modified date**: The date on which the project was modified.
- **Surveys**: The number of surveys in the project.
- **Responses**: The total number of responses received across all surveys in the project.
- **Environment**: The environment in which the project was created.

You can perform the following actions:

- **Rename**: Rename your project title.
- **Copy**: Create a copy of your project in the same or different environment.
- **Share**: Share your project with other people for collaboration.
- **Delete**: Delete a project that you don't need anymore.

## Rename a project

1. Sign in to Dynamics 365 Customer Voice.

2. On the **All projects** tab, hover over the project you want to rename, select vertical ellipsis ![Project options](media/project-options.png "Project options"), and then select **Rename**.

3. In the **Rename Project** dialog box, enter a new name, and then select **Rename**.

    ![Rename a project](media/rename-project.png "Rename a project")

## Copy a project

You can create a copy of your project in the same environment or a different environment. Dynamics 365 Customer Voice gives the new project the same name as the existing project and appends `- copy` to it. You can rename the project if you want.

**What's copied to the new project?**

- **Surveys**: Surveys, along with their customizations, are copied as a new instance to the new project.
- **Satisfaction metrics**: All satisfaction metrics that were configured for their respective questions are copied to the new project. The satisfaction metrics retain their mappings with the questions in the newly created surveys. 
- **Power Automate flows**: All the Power Automate flows configured for the project are copied to the new project.
- **Email templates**: All email templates configured for the surveys are copied to the new project.

**What isn't copied to the new project?**

Survey response data and satisfaction metrics data aren't copied to the new project.

**To copy a project**

1. Sign in to Dynamics 365 Customer Voice.

2. On the **All projects** tab, hover over the project you want to copy, select ![Project options](media/project-options.png "Project options"), and then select **Copy**.

    The **Copy project to** screen is displayed.

3. Do one of the following:

   - To copy your project in the same environment you're currently working in, select the environment listed under **Current location**.

      ![Copy your project in the same environment](media/copy-project-current.png "Copy your project in the same environment")

   - To copy your project to a different environment, expand **All locations**, and then select an environment.

      ![Copy your project to a different environment](media/copy-project-other.png "Copy your project to a different environment")

5. After selecting an environment, select **Copy**. A notification is displayed in the upper-right corner when the project is copied to the selected location.

## Share a project

You can share your project with multiple people in your organization so they can collaborate on the structure and layout of  surveys within the project. The people with whom the project is shared become the co-owners of the shared project. The projects that are shared with you are available on the **All projects** tab. 

**What can a co-owner do?**

A project co-owner has the same level of permissions as the project owner. This means a co-owner can create, edit, update, delete, and share the project.

**What can't a co-owner do?**

- A co-owner cannot remove the project creator from a shared project.

- A co-owner can't delete a survey that was created by another user. The survey can be deleted only by the user who created it. If a co-owner tries to delete a project that contains a survey created by another user, an error is displayed.

- A co-owner can't move a survey that was created by another user. The survey can be moved only by the user who created it. If a co-owner tries to move a survey that is created by another user, an error is displayed.

**How are the responses shared?**

If a project contains responses, a co-owner can see all responses under **Reports** in the left pane. In the Customer Voice survey responses entity, only those responses that are received after the project was shared will be shared with co-owners.

**To share a project**

1. Sign in to Dynamics 365 Customer Voice.

2. On the **All projects** tab, hover over the project you want to share, select ![Project options](media/project-options.png "Project options"), and then select **Share**.

3. In the **Share** panel, on the **Share** tab, select the name of the user from the **Share with** list. You can select multiple users.

    ![Share a project](media/share-project.png "Share a project")

   (Optional: Include a message to send the co-owners.)

4. Select **Share**. 

    The co-owners are displayed on the **Access** tab.

    ![Owners of a project](media/project-owners.png "Owners of a project")

**To remove a co-owner from a project**

1. Sign in to Dynamics 365 Customer Voice.

2. On the **All projects** tab, hover over the project from which you want to remove a co-owner, select ![Project options](media/project-options.png "Project options"), and then select **Share**.

3. In the **Share** panel, go to the **Access** tab, and then select **Remove access** for the user you want to remove.

    ![Remove project access](media/project-owners.png "Remove project access")

## Delete a project

You can delete a project that you don't need anymore. Deleting a project removes its surveys, satisfaction metrics, email templates, survey response data, and satisfaction metrics data. The Power Automate flows associated with the surveys are deactivated. The deletion of a project is permanent and can't be reverted.

**To delete a project**

1. Sign in to Dynamics 365 Customer Voice.

2. On the **All projects** tab, hover over the project you want to delete, select ![Project options](media/project-options.png "Project options"), and then select **Delete**.

3. In the confirmation dialog box, select **Delete**.

### See also

[Create a project](create-project.md)<br>
[Create a survey](create-survey.md)<br>
[Manage surveys](manage-surveys.md)