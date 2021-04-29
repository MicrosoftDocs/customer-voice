---
title: "Integrate Dynamics 365 Customer Voice with Dynamics 365 Customer Service | MicrosoftDocs"
description: "Instructions for integrating Dynamics 365 Customer Voice with Dynamics 365 Customer Service"
ms.date: 04/28/2021
ms.service: dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Integrate Dynamics 365 Customer Voice with Dynamics 365 Customer Service

**Prerequisite**: You must install Dynamics 365 Customer Service in the same tenant as Dynamics 365 Customer Voice. 

You can send a survey automatically to customers as soon as a case is resolved in Dynamics 365 Customer Service. When a customer submits response to a survey, it is attached with the case. You can open the response record from the case’s timeline.

1.	[Create a project](create-project.md) using the **Support** template.

2.	Modify the survey questions and [customize the survey](create-survey.md#customize-a-survey) as required.

3.	Go to the **Send** tab and select **Automation**.

    ![Select Automation to create a flow](media/select-automation.png "Select Automation to create a flow")

4.	In the **Choose a template or create your own** screen, select **Send a survey when a case is resolved in Dynamics 365**.

    ![Select an Automation template](media/select-automation-template.png "Select an Automation template")

5.	Verify the connection details, and select **Continue**.

    ![Verify the connection details](media/verify-connection.png "Verify the connection details")

6.	Select **Create**.

    ![Create the flow](media/create-flow.png "Create the flow")

7.	Go to Dynamics 365 Customer Service and resolve a case. More information: [resolve a case](/customer-service/customer-service-hub-user-guide-resolve-cancel-reassign-a-case).

The survey is automatically sent to the contact or account linked with the case. The survey sent to the survey is visible as a record on the case's timeline.

![Survey invitation on the case's timeline](media/survey-case-timeline.png "Survey invitation on the case's timeline")

When the customer submits a response to the survey, the response record is visible as a record on the case's timeline.

![Survey response on the case's timeline](media/survey-response-case-timeline.png "Survey response on the case's timeline")

To see response details, hover over the response record in timeline, and select **Open Record**.

![See survey response details](media/response-details-timeline.png "See survey response details")

The response detail is displayed in the Customer Voice survey response entity form.

![See survey response details in Dynamics 365](media/response-record-crm.png "See survey response details in Dynamics 365")

### See also

[Create a project](create-project.md)<br>
[Manage projects](manage-projects.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
