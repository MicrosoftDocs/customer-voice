---
title: Dynamics 365 Customer Voice privacy compliance
description: Learn how Dynamics 365 Customer Voice complies with privacy laws and regulations.
ms.date: 11/21/2025
ms.topic: concept-article
author: sbmjais
ms.author: shjais
---

# Dynamics 365 Customer Voice privacy compliance

[!INCLUDE [gdpr-intro](~/../shared-content/shared/privacy-includes/gdpr-intro.md)]

Dynamics 365 Customer Voice includes features to [discover](#discover), [access](#access), [export](#export), and [delete](#delete) a user's personal data.

[!INCLUDE [gdpr-dsr-delete-export-note](~/../shared-content/shared/privacy-includes/gdpr-dsr-delete-export-note.md)]

## Discover

Sign in to [Customer Voice](https://customervoice.microsoft.com) and select **All Projects**. Search the list to determine which Customer Voice project owners sent a survey to the user. Ask them to share the response page link with you. Review the response page and determine whether it's relevant to the user's request.

## Access

For each relevant survey, [view the responses](survey-report.md). To review them in Microsoft Excel, select **Export all** in the upper-left corner of the report. Before you share the worksheet with the user, delete or redact irrelevant data. 

## Delete

To delete a project, go to the **All projects** tab, select the menu button (**&hellip;**) next to the project, and then select **Delete**. When a project is deleted, all its surveys and their questions, invitations, and responses are deleted permanently. To delete a survey, open the project, select the menu button (**&hellip;**) next to the survey,  and then select **Delete**. When a survey is deleted, all its questions, invitations, and responses are deleted permanently. 

## Export

Survey questions, invitations, and responses can be exported to an Excel file.

To export survey questions, open the survey, select **Customization** > **Languages**, add a language, and then select **Download an Excel template here**.

To export invitations, go to the **Send** tab, select **Details** on the **Total invites** tile, and then select **Export**.

To export responses, go to the survey report, and select **Export all** in the upper-left corner of the report.

## Frequently asked questions

### Where is the data stored for Dynamics 365 Customer Voice?

Dynamics 365 Customer Voice has two data stores. The primary data store is on servers in the United States, except in the case of tenants based in Europe. The data for European-based tenants is stored on servers in Europe. The secondary data store is in the respective Power Platform environment location.

### Is the data stored for Dynamics 365 Customer Voice protected with Customer Lockbox?

The data stored in the Power Platform environment is protected with Power Platform Customer Lockbox. [Learn more about securely accessing customer data using Customer Lockbox in Power Platform](/power-platform/admin/about-lockbox).

### How do I restrict access to Dynamics 365 Customer Voice?

Microsoft 365 administrators can turn off Dynamics 365 Customer Voice USL in **User Management** in the Microsoft 365 admin center. [Disable Dynamics 365 Customer Voice for a user with enterprise licenses](purchase.md#disable-dynamics-365-customer-voice-for-a-user).
 
### The original owner of a survey is no longer with the organization and/or their Dynamics 365 Customer Voice license has been removed. What happens to the data that is associated with the surveys they created?

All the customer content data captured by Dynamics 365 Customer Voice, as well as account-related data, is deleted 30 days after a user's account is closed or deactivated. As long as the user accounts are active in the organization's online service agreement, there is no limit to the data, the number of users retained, or the amount of data stored in user accounts.

### How do I use the in-app functionality in Dynamics 365 Customer Voice to find, access, export, and delete personal data?

Content search does not have the ability to find data in Dynamics 365 Customer Voice. To find data, the owner of the survey must use in-product functionality or features to find data that may be relevant to a user's request. Product and service usage data follows a controlled lifecycle designed to comply with such requests.
