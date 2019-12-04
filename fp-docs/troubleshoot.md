---
title: "Troubleshoot | MicrosoftDocs"
description: "Learn how to troubleshoot issues in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 08/19/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 97526FE3-7523-48B0-A8F4-7C369AF78DB4
ms.custom: 
search.appverid:
  - FPR160
---

# Troubleshoot issues in Forms Pro

This article provides information about troubleshooting issues in the Microsoft Forms Pro solution.

## Environment provisioning failure

If you receive an error stating that your environment provisioning has failed, you must check the version of Common Data Service you are using. Forms Pro doesn't work with the previous version. If your default environment is created with the previous version of Common Data Service, your environment will not be provisioned and an error message is displayed. You must upgrade the previous version of Common Data Service to the newer version. For more information on Common Data Service, see [What is Common Data Service](https://docs.microsoft.com/common-data-service/upgradecds/introduction-upgrade-cds).

To delete or upgrade your Common Data Service from a previous version to the newer version, contact your global administrator. 

If your environment provisioning has failed, the provisioning will be retried periodically. If you want to prioritize or submit any other requests, please contact Microsoft Support.

If you have upgraded Common Data Service and your environment creation still has issues, please contact Microsoft Support.

## Environment permission failure

If you receive an error stating that you don't have permission to access the environment, you must contact your administrator to verify the following:

- Microsoft Forms Pro solution is installed.
- An application user with the name Microsoft Forms Pro is created.
    - The application user has the Survey Services Administrator and System Administrator security roles assigned.
    - The Survey Services Administrator security role has the Organization privileges on the survey entities as specified in [Survey Services Administrator security role privileges](#survey-services-administrator-security-role-privileges).
- You have the Survey Owner security role assigned.
    - The Survey Owner security role has the User privileges on the survey entities as specified in [Survey Owner security role privileges](#survey-owner-security-role-privileges).

### Survey Services Administrator security role privileges

|Entity|Create|Read|Write|Delete|Append|Append To|Assign|Share|
|------|------|----|-----|------|------|---------|------|-----|
|Survey|x|x|x|x|x|x|x|x|
|Survey email template|x|x|x|x|x|x|x|x|
|Survey question|x|x|x|x|x|x|x|x|
|Survey question response|x|x|x|x|x|x|x|x|
|Unsubscribed recipient|x|x|x|x|x|x|x|x|
||||||||||

### Survey Owner security role privileges

|Entity|Create|Read|Write|Delete|Append|Append To|Assign|Share|
|------|------|----|-----|------|------|---------|------|-----|
|Survey|x|x|x|x|x|x|x|x|
|Survey email template|x|x|x|x|x|x|x|x|
|Survey question|x|x|x|x|x|x|x|x|
|Survey question response|x|x|x|x|x|x|x|x|
||||||||||

## Invalid connection error in Flow

If you receive an error stating that your connection is invalid or there is a problem with the flow's trigger, you must:

1. Open Power Automate.

2. In the left pane, select **Data** > **Connections**.

3. Search for the **Microsoft Forms Pro** connection and delete it.

    > [!NOTE]
    > If you have created multiple connections for Microsoft Forms Pro, you must delete all of them.

4. Select **New connection** to create a new connection.

5. From the list of connections, search for **Microsoft Forms Pro** and select it.

6. In the confirmation window, select **Create**, and then enter your credentials.

7. Open the flow in which the error occurred.

8. Go to the action causing the error. The connection you created is displayed.

9. Select the connection from the list. The error will be resolved after selecting the connection and flow will work fine.

## Error while setting up a user in default environment

When you sign in to Microsoft Forms Pro in the default environment, security roles are assigned to you. If any error occurs during the role assignment, see if you fall under any of the following categories and resolve the error accordingly:

|Error|Resolution|
|-----|----------|
|User does not have a license|Assign an appropriate license to the user in Active Directory.|
|User is not part of the security group|Add the user to the instance's security group.|
|User is not created in Active Directory|Create the user in Active Directory.|
|User is not enabled in Active Directory|Enable the user in Active Directory.|
|Instance not found|Instance details are incorrect or instance is deleted.|
|Instance is not enabled|Instance is disabled. Enable the instance and try again.|
|||

> [!NOTE]
> The above errors are displayed only in the default environment. If you are working in an environment other than the default environment, contact your administrator to assign the roles accordingly. More information: [Work with environments](choose-environment.md)

If you are not able to resolve the error, please contact Microsoft Support.

## Azure Active Directory disabled error

If you receive an error stating that Azure Active Directory is disabled, you must verify whether:

- The Dynamics CRM Online app is disabled on the tenant.
- A new app is created with an "https://admin.service.crm4.dynamics.com" audience, which is disabled and Azure Active Directory is giving preference over to that app, instead of Microsoft's first-party app.

If a new app is created, you must remove the app or change the audience. If this is not the case, you must contact your tenant administrator to run the following script, which will re-enable the Dynamics CRM Online app in the tenant and should resolve the error. 

1. Download the AzureAD Module from [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0).

2. Run the following commands in a PowerShell window (run PowerShell as an administrator). When prompted, sign in with the tenant administrator credentials.
    ```
    Install-Module AzureAD
    Connect-AzureAD
    $sp = Get-AzureADServicePrincipal -Filter "AppId eq '00000007-0000-0000-c000-000000000000'"
    Set-AzureADServicePrincipal -ObjectId $sp.ObjectId -AccountEnabled $True
    ```

3. If the error does not resolve after running the above commands or the above commands throw an error, run the following commands to completely reset the principal on the tenant to make sure it's in a proper state.
    ```
    $appId = "00000007-0000-0000-c000-000000000000"
    Get-AzureADServicePrincipal -Filter "AppId eq '00000007-0000-0000-c000-000000000000'" | Remove-AzureADServicePrincipal
    New-AzureADServicePrincipal -AppId $appId
    ```


