---
title: "Connect Dynamics 365 Customer Voice with your environment | MicrosoftDocs"
description: "Learn about connecting Dynamics 365 Customer Voice with your environment"
ms.date: 03/23/2021
ms.service: 
  - dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Connect Dynamics 365 Customer Voice with your environment

[!INCLUDE[cc-data-platform-banner](includes/cc-data-platform-banner.md)]

An environment is a space to store, manage, and share your organization's business data, apps, and flows. It also serves as a container to separate apps that might have different roles, security requirements, or target audiences. More information: [Environments overview](https://docs.microsoft.com/power-platform/admin/environments-overview)

In Dynamics 365 Customer Voice, all projects created by you or shared with you across environments are displayed in the **All Projects** tab. When you create a project, the project is connected to the selected environment. The survey data including invitations and responses are stored in the same environment in which the project is created. You select an environment during [project creation](create-project.md). You can copy a project within same or across environments. More information: [Manage projects](manage-projects.md)

To work with projects in an environment, install the [Dynamics 365 Customer Voice app](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.shimla?tab=Overview) (formerly called Microsoft Forms Pro) from Microsoft AppSource, and assign the Project Owner role to users in Dynamics 365. If you select an environment that doesn't have the Customer Voice app, an error message is displayed during project creation.

When you install the Customer Voice app, an application user named Customer Voice is created automatically. The email address of application user is `enterprisesurveyappuser@contoso.com`. This user is created to allow Customer Voice Azure service to authenticate with Microsoft Dataverse using Server-to-Server (S2S) authentication, and is primarily used for saving survey data in the environment. The user is a non-interactive and non-login system user. The user is assigned Survey Services Administrator and System Administrator roles. More information on S2S authentication: [Build web applications using Server-to-Server (S2S) authentication](https://docs.microsoft.com/powerapps/developer/common-data-service/build-web-applications-server-server-s2s-authentication)

> [!NOTE]
> - If you have organizations for Dynamics 365 Sales, Customer Service, Marketing, and Talent, Customer Voice entities are already installed in these organizations.
> - A default environment is based on Dataverse. Before planning a large scale deployment, see [service protection API limits](https://docs.microsoft.com/powerapps/developer/common-data-service/api-limits). To learn more about the default environment, see [default environment](https://docs.microsoft.com/power-platform/admin/environments-overview#the-default-environment).
> - You must not delete Customer Voice data directly from Dataverse. If you delete any data directly from Dataverse, it is not synchronized with Customer Voice services.

## Privileges required

- Ensure that you've assigned the Project Owner role to users in Dynamics 365.
- If you've created any custom entities that you want Customer Voice to interact with, assign the **Append To** privilege of the entities to the user.

### Minimum privileges for a custom role

If you've created a custom security role and want to use it as a project owner, ensure that the custom role has User permission on the entities used by Customer Voice. The following table shows the required and optional privileges for the entities.

A required privilege is denoted by ![Required](media/required-icon.png "Required").

If you provide the optional privileges, additional actions can be performed by the user who is assigned the custom role. For example, the Read privilege is required for the Contact entity and is used to associate invitations with a specific contact. Other privileges, such as Create and Write, are optional. If you provide Create and Write privileges, a user can perform these operations on a contact. If you provide only the Read privilege, and you want a particular user to perform create and write operations also on a contact, you can provide Create and Write privileges to the user through other security roles.

|Entity                            |Create   |Read     |Write    |Delete   |Append   |Append To|
|----------------------------------|---------|---------|---------|---------|---------|---------|
|Customer Voice project      |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice satisfaction metric    |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice localized survey email template     |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice survey                  |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice survey email template   |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice survey question         |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") | |
|Customer Voice survey question response|![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |  |
|Customer Voice unsubscribed recipient  |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |  | 
|Activity                          |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |![Required](media/required-icon.png "Required") |  |![Required](media/required-icon.png "Required") | ![Required](media/required-icon.png "Required")| 
|Contact                           |  |![Required](media/required-icon.png "Required") |  |
|||||||

### See also

[Create a project](create-project.md)<br>
[Manage projects](manage-projects.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]