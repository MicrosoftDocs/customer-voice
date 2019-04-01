---
title: "Troubleshoot | MicrosoftDocs"
description: "Learn how to troubleshoot issues in Microsoft Forms Pro"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 04/01/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 97526FE3-7523-48B0-A8F4-7C369AF78DB4
ms.custom: 
---

# Troubleshoot issues in Forms pro

This article provides information about troubleshooting issues in the Forms Pro solution.

## Environment provisioning failure

If you receive an error stating that your environment provisioning has failed, you must check the version of Common Data Service (CDS) you are using. Forms Pro doesn't work with the legacy version of CDS. If your default environment is created with legacy CDS, your environment will not be provisioned and an error message is displayed. You must upgrade the legacy CDS to use the newer version of CDS for Apps. For more information on upgrading to CDS for Apps, see [Upgrade to Common Data Service for Apps](https://docs.microsoft.com/en-us/common-data-service/upgradecds/introduction-upgrade-cds).

To delete or upgrade your CDS from previous version to the newer version, contact your Global administrator. 

If your environment provisioning has failed, the provisioning will be retried periodically. If want to prioritize or submit any other request, please contact support.

If you have upgraded the CDS and your environment creation is still having issues, please contact support.

> [!NOTE]
> Ensure that you upgrade the CDS in your default environment only.

## Environment permission failure

If you receive an error stating that you don't have permission to access the environment, you must contact your administrator to verify the following:

- Forms Pro solution is installed.
- An application user is created.
    - The application user is having the Survey Services Administrator security role assigned.
    - The Survey Services Administrator security role has the Organization privileges on all the Survey, Survey email template, Survey question, Survey question response, and Unsubscribed recipient entities.
- The system user is having the Survey Owner security role assigned.
    - The Survey Owner security role has the User privileges on the  Survey, Survey email template, Survey question, and Survey question response entities.


