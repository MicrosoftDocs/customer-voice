---
title: "Frequently asked questions | MicrosoftDocs"
description: "Use this article to know about the frequently asked questions and their answers in Dynamics 365 Customer Voice."
ms.date: 01/05/2026
ms.topic: faq
author: sbmjais
ms.author: shjais
ms.custom: sfi-image-nochange
---

# Dynamics 365 Customer Voice FAQ

We've compiled a list of frequently asked questions and provided brief answers to help you get to your information quickly.

## I created a guest user in Microsoft Entra ID, but the user is unable to access Dynamics 365 Customer Voice.

Guest user access isn't supported in Dynamics 365 Customer Voice. You must create a new user in your tenant and then provide access to the new user.

## How is the owner of a survey response determined?

A response owner is determined by the following logic:

- For responses to a survey invitation, the invitation owner is set as the response owner.
- If the survey invitation owner doesn't have sufficient privileges to own responses, or if the response is anonymous, the survey owner is set as the response owner.
- If the account of a survey owner has been disabled or the survey owner is unable to access the application due to licensing issues, the application user is set as the response owner.

## What has changed in the short URL domain for surveys?

Starting from May 1, 2024, the short URL domain has changed from `https://<region>.microsoft.com` to `https://<region>.dcv.ms`.

**What will happen to the existing short URLs?**

This change only impacts the short URLs generated after May 1, 2024; existing short URLs with `https://<region>.microsoft.com` domain, created before May 1, will continue to work.

**What do I need to do if I'm using short URLs in my surveys?**

Reach out to your IT team and check if your network firewall or email security systems requires you to allow new URLs. If yes, you need to add the new domain `dcv.ms` to your allow list immediately. If you do not have any such restrictions, you don't have to take any action. You can continue to create and send survey links as usual. 

**What will NOT be impacted by this short url change?**

The following services will not be impacted by this change:

- The main link customervoice.microsoft.com 
- The default domains for sending emails (surveys@email.formspro.microsoft.com) 
- The custom domains for sending emails
- Old Short URLs
- Old QR codes 

## I deleted data from Microsoft Dataverse but it's visible in reports.

It's recommended not to delete data directly from Microsoft Dataverse. If you delete any data directly from Microsoft Dataverse, it isn't synchronized with Customer Voice services. If you want to delete any data, you must delete using the Dynamics 365 Customer Voice interface.

## Why does the application user require the System Administrator role?

The application user requires the System Administrator role to associate survey invites and responses to any of the entities, including custom entities.

## What happens if the project owner leaves the organization?

If the project owner leaves the organization, the project is deleted once the user is removed from the organization. If the project was shared by the user before leaving the organization, the existing user, with whom the project is shared, must create a [copy of the project](manage-projects.md#copy-a-project) before user leaves the organization and use the copied project.

When a user is deleted, it is considered as a soft delete for 30 days. After 30 days, the user is hard deleted. This activity takes place in Microsoft Entra ID. Once the account of the survey owner is hard deleted, the survey is deleted automatically from Dynamics 365 Customer Voice but the data is retained in Microsoft Dataverse till the retention policy is met. If the user is only deactivated, the survey is not deleted but operations will fail. If a project has surveys with owners who are active, the project appears in the list of projects on the Dynamics 365 Customer Voice interface.

## The original owner of a survey is no longer with the organization and/or their Customer Voice license has been removed. What happens to the data associated with the survey?

All account-related data is deleted 30 days after the account is deleted from Microsoft Entra ID.

## What languages are supported for sentiment analysis?

Dynamics 365 Customer Voice supports the following languages for sentiment analysis:

|     Language                 |     Language code    |
|------------------------------|------------------------|
|     Chinese                  |     zh                 |
|     Chinese-Simplified       |     zh-hans            |
|     Chinese-Traditional      |     zh-hant            |
|     Dutch                    |     nl                 |
|     English                  |     en                 |
|     French                   |     fr                 |
|     German                   |     de                 |
|     Hindi                    |     hi                 |
|     Italian                  |     it                 |
|     Japanese                 |     ja                 |
|     Korean                   |     ko                 |
|     Norwegian (Bokmål)       |     no                 |
|     Portuguese (Brazil)      |     pt-BR              |
|     Portuguese (Portugal)    |     pt-PT              |
|     Portuguese               |     pt                 |
|     Spanish                  |     es                 |
|     Turkish                  |     tr                 |
|||

Survey responses received in languages other than the ones specified above are considered as English and sent to the cognitive services for further processing. In this case, the accuracy would be impacted.

## How can I change the ownership of satisfaction metrics and alerts from owner to a team?

### Assign the satisfaction metric record from owner to a team

1. Sign in to [Power Apps](https://make.powerapps.com/) with a user that has access to Dynamics 365 records.

2. Select **Settings** > **Advanced settings**.

    :::image type="content" source="media/advanced-settings-pa.png" alt-text="Go to advanced settings in Power Apps":::

3. Select **Advanced Find** on the command bar at the top.

    :::image type="content" source="media/advanced-find.png" alt-text="Go to advanced find":::

4. In the **Look for** list, select **Customer Voice satisfaction metric**.

5. In the **Select** list, select **Project**.

6. Select **Enter value**, then browser and select the name of the project.

    :::image type="content" source="media/advanced-find-window-sm.png" alt-text="Advanced find filter values for satisfaction metrics":::

7. Select **Results**. A list of all satisfaction metrics associated to the project is displayed.

8. Select the records whose ownership needs to be changed, and then select **Assign Customer Voice Satisfaction metric**.
 
    :::image type="content" source="media/advanced-find-results-sm.png" alt-text="Advanced find result for satisfaction metrics":::

9. In the **Assign Customer Voice satisfaction metric** window, select the **Assign to** field to change its value to **User or team**.

10. In the **User or team** field, browse and select the team to which ownership needs to be transferred.

    :::image type="content" source="media/assign-window-sm.png" alt-text="Assign the selected satisfaction metrics to a team":::

    > [!NOTE]   
    > To know how to find a team, see [How to find a team?](#how-to-find-a-team).

11. Select **Assign**.

### Assign the alert record from owner to a team

1. Sign in to [Power Apps](https://make.powerapps.com/) with a user that has access to Dynamics 365 records.

2. Select **Settings** > **Advanced settings**.

    :::image type="content" source="media/advanced-settings-pa.png" alt-text="Go to advanced settings in Power Apps":::

3. Select **Advanced Find** on the command bar at the top.

    :::image type="content" source="media/advanced-find.png" alt-text="Go to advanced find":::

4. In the **Look for** list, select **Customer Voice alert**.

5. In the **Select** list, select **Project**.

6. Select **Enter value**, then browser and select the name of the project.

7. Add the **Owner** column.

    :::image type="content" source="media/advanced-find-window-alert.png" alt-text="Advanced find filter values for alerts":::

8. Select **Results**. A list of all alerts associated to the project is displayed.

9. Select the records whose ownership needs to be changed, and then select **Assign Customer Voice alert**.

    :::image type="content" source="media/advanced-find-results-alert.png" alt-text="Advanced find result for alerts":::

10. In the **Assign to Team or User** window, select the **Assign to** field to change its value to **User or team**.

11. In the **User or team** field, browse and select the team to which ownership needs to be transferred.

    :::image type="content" source="media/assign-window-alert.png" alt-text="Assign the selected alerts to a team":::

12. Select **Assign**.
 
### How to find a team?

1. In the **Assign to Team or User** window, select the **Assign to** field to change its value to **User or team**.

2. Hover over the **User or team** field, and select the **Select a value** icon.
 
    :::image type="content" source="media/find-team.png" alt-text="Find a team":::

3. In the list, select **Look Up More Records**.

    :::image type="content" source="media/find-team-lookup.png" alt-text="Lookup more records":::

4. In the **Lookup Record** window, enter or select the following values:
    - **Look for**: Team
    - **Look in**: All AAD office Group Teams
    - **Search**: Name of the team.
    - Select the **Search** icon next to this field.

    :::image type="content" source="media/find-team-lookup-record-window.png" alt-text="Lookup Record window":::

5. From the search results, select a team, and then select **Add**.

## I deleted the old surveys and survey responses, and want to update values in the satisfaction metrics report accordingly.

This is an unsupported scenario. Deleting old surveys and survey responses won't update values in the satisfaction metrics report.

## I want to delete multiple responses from the Dynamics 365 Customer Voice interface.

Deleting multiple responses from the Dynamics 365 Customer Voice interface isn't supported.

## I restored Microsoft Dataverse and want Dynamics 365 Customer Voice and survey responses to work with it.

This is an unsupported scenario.

## I migrated my Microsoft Dataverse environment from one tenant to another, but I don't see my existing projects when I sign in to Dynamics 365 Customer Voice in the new tenant.

Tenant to tenant migration isn't supported for Dynamics 365 Customer Voice.

## Should I use Microsoft Forms connector for Customer Voice surveys in Power Automate flow?

It isn't recommended to use [Microsoft forms connector](/connectors/microsoftforms/) for Customer Voice surveys. The flow might not run properly. You must only use [Customer Voice connectors](/connectors/microsoftformspro/) and [Dataverse connectors](/power-automate/dataverse/overview) while creating flows for Customer Voice surveys.

## I added unicode character while designing a survey but it isn't rendered properly.

Manually adding unicode character isn't supported in Dynamics 365 Customer Voice. For example, if you add unicode character in a question and survey title, it will not be rendered properly.

## Why projects aren't visible while creating a flow in Power Automate?

If you've created projects in Dynamics 365 Customer Voice and shared all the projects with other users, the projects won't be visible while creating a flow in Power Automate. You must create at least one project that isn't shared with other users. After the new project is created, all the projects (user owned and shared) will be visible while creating a flow in Power Automate. It takes 5 minutes for the projects to be visible in Power Automate.

## Can I see responses submitted through the Report abuse link?

The responses submitted through the **Report abuse** link can only be seen by Microsoft. Neither the respondent nor the survey owner can see them. The responses help Microsoft to identify if someone is misusing a survey for phishing or any illegal activities.

## Can I remove the Report abuse link from a survey?

No, the **Report abuse** link can't be removed from a survey.

## Why a flow retries to send a survey invitation?

A flow retries to send a survey invitation after the original request times out or fails. The retry policy works with HTTP action and handles the following status codes: 408, 429, and 5xx. The flow retries for the specified number of times and interval. 

## How can I customize the privacy statement?

Privacy statement can be customized by administrators from the Azure portal. In the Azure portal, open Microsoft Entra ID, and then select the **Properties** tab. In the **Properties** tab, enter the link to the privacy statement in the **Privacy statement URL** field. 

:::image type="content" source="media/customize-privacy-statement.png" alt-text="Screenshot showing customized privacy statement URL.":::

## Can I transfer the ownership of a project from a user who has left the organization or will leave soon?

No, transferring the ownership of a project is not supported currently. You must create a copy of the project and share it with other users. Ensure that the newly copied project is used going forward.

## Can I restore a deleted project?

No, restoring a deleted project is not supported currently. 

## How are satisfaction metrics values aggregated in a report?

Satisfaction metrics values are aggregated based on the time filter selected in the report. The values are aggregated as follows:

- By six hours, if the value selected in the filter is less than or equal to two days.
- By 24 hours, if the value selected in the filter is less that or equal to seven days (Last 7 days).
- By week, if the value selected in the filter is more than two days but less than 30 days (All days or Last 28 days).
- By month, if the value selected in the filter is more than 30 days (Last 90 days).

## Why can't I create alerts for custom score satisfaction metrics?

Alerts can't be created for custom score satisfaction metrics. It's the limitation of the product.

## What P99 or average latency for data synchronization between Dynamics 365 Customer Voice and Microsoft Dataverse?

There's no official latency for data synchronization. Data is synchronized from Dynamics 365 Customer Voice to Microsoft Dataverse in an asynchronous manner. 

## Why the Forms connector shows warm data lock error?

When responses for a form reach 65,000, the form gets locked for archiving data to cold storage and the Forms connector shows a warm data lock error. It is recommended to use [Dataverse connectors](/power-automate/dataverse/overview) instead of the Forms connector.

## Is there any impact on the performance of Customer Voice when moving the organization to a different datacenter?

There's no impact on the performance of Customer Voice when moving the organization to a different datacenter as long as the organization ID and organization name remain the same.

## In which business unit is team created after sharing a project?

When a project is shared with a team, the team is created in the root business unit (BU). We recommend not to change anything manually in the organization directly.

## Why can't I see personalization variables in Create an Invitation and Send a Survey Power Automate connectors?

[Perosnalization variables](personalize-survey.md) are not available in non-Open API Power Automate flows. It is recommended to create a new flow that is based on Open API by default. To check if your flow is non-Open API, see if there's Peek code on an action and if you see the API Connection value instead of Open API Connection in Kind field, it's a non-Open API flow.


## Why do invite counts differ between the Send tab and exported data?

The invite count shown on the [**Total invites** card](view-survey-invite.md) in the **Send** tab may differ from the count in [exported data](view-survey-invite.md#export-invitation-details) because they use different data sources:

- **Exported data**: Generated directly from Microsoft Dataverse and reflects the actual invite records created. This data is accurate and complete, and you can verify it through exports or Advanced Find.
- **Send tab**: Displays a summarized dashboard view for quick reference. During periods of high activity or when sending a large number of invites simultaneously, this view may not fully align with historical data.

As a result, you may notice differences between the invite count shown on the [**Total invites** card](view-survey-invite.md) in the **Send** tab and the [exported](view-survey-invite.md#export-invitation-details) counts across multiple projects or surveys. However, the exported Dataverse data is always accurate and complete.

## How can I share new feature requirements or ideas?

You can share your new feature requirements or ideas on the [Customer Voice Ideas](https://aka.ms/customervoiceideas) page.


[!INCLUDE[footer-include](includes/footer-banner.md)]
