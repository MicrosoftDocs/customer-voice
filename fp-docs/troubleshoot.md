---
title: "Troubleshoot | MicrosoftDocs"
description: "Learn how to troubleshoot issues in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/02/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 97526FE3-7523-48B0-A8F4-7C369AF78DB4
ms.custom: 
---

# Troubleshoot issues in Forms pro

This article provides information about troubleshooting issues in the Forms Pro solution.

## Environment provisioning failure

If you receive an error stating that your environment provisioning has failed, you must check the version of Common Data Service you are using. Forms Pro doesn't work with the previous version of Common Data Service. If your default environment is created with the previous version of Common Data Service, your environment will not be provisioned and an error message is displayed. You must upgrade the previous version of Common Data Service to the newer version of Common Data Service for Apps. For more information on upgrading to Common Data Service for Apps, see [Upgrade to Common Data Service for Apps](https://docs.microsoft.com/en-us/common-data-service/upgradecds/introduction-upgrade-cds).

To delete or upgrade your Common Data Service from previous version to the newer version, contact your Global administrator. 

If your environment provisioning has failed, the provisioning will be retried periodically. If want to prioritize or submit any other request, please contact support.

If you have upgraded the Common Data Service and your environment creation is still having issues, please contact support.

## Environment permission failure

If you receive an error stating that you don't have permission to access the environment, you must contact your administrator to verify the following:

- Microsoft Forms Pro solution is installed.
- An application user with the name Microsoft Forms Pro is created.
    - The application user has the Survey Services Administrator security role assigned.
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
