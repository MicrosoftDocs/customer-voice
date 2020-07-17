---
title: "Connect Dynamics 365 Customer Voice with your environment | MicrosoftDocs"
description: "Learn about connecting Dynamics 365 Customer Voice with your environment"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Connect Dynamics 365 Customer Voice with your environment

An environment is a space to store, manage, and share your organization's business data, apps, and flows. It also serves as a container to separate apps that might have different roles, security requirements, or target audiences. More information: [Environments overview](https://docs.microsoft.com/power-platform/admin/environments-overview)

You can create environments for different purposes such as survey development, testing, and production. After developing and testing the survey, you can copy the survey or the project to the production environment.

When you sign in to Dynamics 365 Customer Voice, only the projects that are available in the selected environment are displayed. When you create a project, the project is connected to the selected environment and isn't available in other environments. The invitations and responses are stored in the same environment in which the project was created.

You select an environment while [creating a project](create-project.md). You can also copy a project from one environment to another. More information: [Manage projects](manage-projects.md)

To work with projects in an environment, install the [Customer Voice app from Microsoft AppSource](linkhere), and assign the Project Owner role to users. If you select an environment that doesn't have the Customer Voice app, an error message is displayed.

When you install the Customer Voice app, an application user named Customer Voice is created automatically. This user is created to allow Customer Voice Azure service to authenticate with Common Data Service using Server-to-Server (S2S) authentication, and is primarily used for pushing survey data. The user is a non-interactive and non-login user. It is assigned Survey Services Administrator and System Administrator roles. More information on S2S authentication: [Build web applications using Server-to-Server (S2S) authentication](https://docs.microsoft.com/powerapps/developer/common-data-service/build-web-applications-server-server-s2s-authentication)

> [!NOTE]
> - If you have organizations for Dynamics 365 Sales, Customer Service, Marketing, and Talent, Customer Voice entities are already installed in these organizations.
> - A default environment is based on Common Data Service. Before planning a large scale deployment, see [service protection API limits](https://docs.microsoft.com/powerapps/developer/common-data-service/api-limits). To learn more about the default environment, see [default environment](https://docs.microsoft.com/power-platform/admin/environments-overview#the-default-environment).

## Privileges required

- Ensure that you've assigned the Project Owner role to users.
- If you've created any custom entities that you want Customer Voice to interact with, assign the **Append To** privilege of the entities to the user.

### Minimum privileges for a custom role

If you've created a custom security role and want to use it as a project owner, ensure that the custom role has User permission on the entities used by Customer Voice. The following table shows the required and optional privileges for the entities.

A required privilege is denoted by ![Required](media/required-icon.png "Required").

An optional privilege is denoted by ![Optional](media/optional-icon.png "Optional").

If you provide the optional privileges, additional actions can be performed by the user who is assigned the custom role. For example, the Read privilege is required for the Contact entity and is used to associate invitations with a specific contact. Other privileges, such as Create and Write, are optional. If you provide Create and Write privileges, a user can perform these operations on a contact. If you provide only the Read privilege, and you want a particular user to perform create and write operations also on a contact, you can provide Create and Write privileges to the user through other security roles.

|Entity                            |Create   |Read     |Write    |Delete   |Append   |Append To|Assign |Share   |
|----------------------------------|---------|---------|---------|---------|---------|--------|--------|--------|
|Customer Voice survey                  |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Customer Voice survey email template   |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Customer Voice Survey question         |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Customer Voice Survey question response|![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Customer Voice unsubscribed recipient  |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional") |![Optional](media/optional-icon.png "Optional") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Activity                          |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
|Contact                           |![Optional](media/optional-icon.png "Optional") |![Required](media/required-icon.png "Required") |![Optional](media/optional-icon.png "Optional") |![Optional](media/optional-icon.png "Optional") |![Optional](media/optional-icon.png "Optional") |![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|![Optional](media/optional-icon.png "Optional")|
||||||||||

### See also

[Create a project](create-project.md)<br>
[Manage projects](manage-projects.md)<br>
