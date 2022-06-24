---
title: "Dynamics 365 Customer Voice GDPR compliance | MicrosoftDocs"
description: "Use this topic to know how Dynamics 365 Customer Voice complies with General Data Protection Regulation (GDPR)."
ms.date: 06/24/2022
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Dynamics 365 Customer Voice GDPR compliance

The European Union (EU) General Data Protection Regulation (GDPR) gives rights to people (known in the regulation as data subjects) to manage the personal data that's been collected by a corporation or other types organizations, including employers (known as the data controller or just controller). Personal data is defined broadly under the GDPR as any data that relates to an identified or identifiable natural person. Microsoft is committed to helping business customers to be GDPR compliant and Dynamics 365 Customer Voice is GDPR compliant.

Dynamics 365 Customer Voice allows licensed users to capture feedback swiftly across different channels with personalized surveys. It also helps to track customer metrics that are important. The survey questions, invitations, satisfaction metrics defined, responses from end users are all in the direct control of administrators and end users. Microsoft processes data on behalf of customers to provide the requested service as set forth in our [Online Services Terms](https://go.microsoft.com/fwlink/?LinkID=734008). Administrators can set policies that control this information independent of the user account lifecycle for which Dynamics 365 Customer Voice license is associated with.

The in-app functionality in Dynamics 365 Customer Voice enables to [discover](#discover), [access](#access), [export](#export), and [delete](#delete) personal data.

## Discover

Licensed users of Dynamics 365 Customer Voice must sign in to https://customervoice.microsoft.com and select **All Projects** to see the list of all projects that they have created or have collaborated with other users within the tenant. To determine whether Dynamics 365 Customer Voice has personal data for the Data Subject Request (DSR), you can ask the Data Subject to search his list to determine which users ("Customer Voice Project Owners") have sent the survey to the Data Subject. You can then ask the project owners to share the response page link so that you can view it and further determine whether it is relevant to your DSR.

## Access

After the relevant surveys are found, you can access the responses of the survey by selecting it under the **Reports** section. Learn more about how to [check your survey results](survey-report.md). To review response results in Excel, select **Export all** in the upper-left corner of the report. If you would like to send the Data Subject a copy of the survey, you can either take screenshots of the relevant questions and answers by selecting the Data Subject in the **Respondents** panel in rich text format or send the Data Subject a copy of Excel sheet containing the results. If you are using Excel and would like to share with the Data Subject only portions of the survey result, you can delete certain rows or columns or redact the remaining sections before sharing the results. 

## Delete

A project or survey can be permanently deleted by its owner. To honor the "forget me" request by a DSR and to delete a survey in its entirety, go to the **All projects** tab, hover over the project you want to delete, select the ellipsis button, and then select **Delete**. Once a project is deleted, all surveys and their questions, invitations, and responses are deleted permanently. If a project consists of more than one survey, open the project, hover over the survey to be deleted, select the ellipsis button, and then select **Delete**. Once a survey is deleted, all the survey questions,  invitations, and responses for the survey are deleted permanently. 

## Export

Survey questions, invitations, and responses can be exported to an Excel file.

To export survey questions, open the survey, select **Customization** > **Languages**, add a language, and then select **Download an Excel template here**.

To export invitations, go to the **Send** tab, select **Details** on the **Total invites** tile, and then select **Export**.

To export responses, go to the survey report, and select **Export all** in the upper-left corner of the report.

## Frequently asked questions

### Where is the data stored for Dynamics 365 Customer Voice?

Dynamics 365 Customer Voice has two data stores, the primary data store is on servers in the United States, with the exception of data for European-based tenants. The data for European-based tenants is stored on servers in Europe. The secondary data store is in the respective Power Platform environment location. For more information about Dataverse, see [Resources to manage GDPR Compliance](/power-platform/admin/wp-compliance-data-privacy#resources-to-manage-gdpr-compliance).

### Is the data stored for Dynamics 365 Customer Voice protected with Customer Lockbox?

The data stored in the Power Platform environment is protected with Power Platform Customer Lockbox. For more information about Customer Lockbox, see [Securely access customer data using Customer Lockbox in Power Platform](https://docs.microsoft.com/power-platform/admin/about-lockbox).

### How do I restrict access to Dynamics 365 Customer Voice?

Microsoft 365 administrators can turn off Dynamics 365 Customer Voice USL for users by going to **User Management** in Microsoft 365 Admin Center. For information about disabling Dynamics 365 Customer Voice for a user with enterprise licenses, see [Disable Dynamics 365 Customer Voice for a user with enterprise licenses](purchase.md#disable-dynamics-365-customer-voice-for-a-user). For information about disabling Dynamics 365 Customer Voice for a user without enterprise licenses [Disable Dynamics 365 Customer Voice for a user without enterprise licenses](purchase.md#disable-dynamics-365-customer-voice-for-a-user-1). 
 
### The original owner of a survey is no longer with the organization and/or their Dynamics 365 Customer Voice license has been removed. What happens to the data that is associated with the surveys they created?

All the customer content data captured by Dynamics 365 Customer Voice, as well as account related data will be deleted in 30 days after a user's account is closed or deactivated. As long as the user accounts are active within the organization's online service agreement, currently there is no limit to the data or the number of users to be retained. There is also no limit to the amount of data stored on user accounts.

### How do I use the in-app functionality in Dynamics 365 Customer Voice to find, access, export, and delete personal data?

Currently, content search does not have the ability to find data in Dynamics 365 Customer Voice. To find data, the owner of the survey must use in-product functionality or features to find data that may be relevant to a DSR. Product and service usage data follows a controlled lifecycle designed to comply with GDPR data subject requests.



