---
title: "Customer Satisfaction app | MicrosoftDocs"
description: "Instructions for working with Forms Pro Customer Satisfaction app"
keywords: ""
author: sbmjais
ms.author: shjais
manager: shujoshi
applies_to: 
ms.date: 10/01/2019
ms.service: forms-pro
ms.topic: article
ms.assetid: 7771F115-DD60-4084-A8C3-A0DDBC2128A3
ms.custom: 
search.appverid:
  - FPR160
---

# Monitor customer satisfaction

Use the Forms Pro Customer Satisfaction app to get insights report that link customer feedback with the cases when you use Microsoft Forms Pro to send survey after case resolution in Dynamics 365 Customer Service. You can view average Net Promoter Score (NPS) as well as your agent's and customer's individual NPS. This app provides you the capability to filter the report by case priority, location, product, and more parameters. Survey metrics such as number of survey invitations sent, number of survey responses received, NPS, sentiment, and key phrases are also displayed in the report. You can also edit the reports and build customized reports as per your requirement.

## Install the Forms Pro Customer Satisfaction app

The Forms Pro Customer Satisfaction app is a template app built using Power BI. This app helps you to know your customers' satisfaction and your agents' performance. You can connect your Dynamics 365 Customer Service instance to view insights based on your data. This app comes with sample data for you to navigate and explore the app. It also gives you the capability to edit and customize the workspace as per your requirement.

For more information on template apps, see [What are Power BI template apps?](https://docs.microsoft.com/en-us/power-bi/service-template-apps-overview).

For steps to install a template app and get started, see [Install and distribute template apps](https://docs.microsoft.com/en-us/power-bi/service-template-apps-install-distribute).

## Report

The Forms Pro Customer Satisfaction app displays insights in a report with the following pages:

- [Overview](#overview)
- [Agent Performance](#agent-performance)
- [Customer Satisfaction](#customer-satisfaction)

You can filter the data using the **Date** filter at the top of the report. The data is filtered based on the survey invitations sent during the selected time period. Let's say, you've sent 100 survey invitations during the selected time period. You received 60 responses within the time period and 20 responses after the time period. The 20 responses will also be included in the report.

If you would like to select a different survey for displaying insights, you can do it from the **Filters** pane on the right-side of the report. Open the pane and select a survey from the **Survey Name** filter under **Filters on all pages**. 

For more information on working with filters in Power BI reports, see [The new filter experience in Power BI reports](https://docs.microsoft.com/en-us/power-bi/power-bi-report-filter).

For more information on working with reports, see [Reports in Power BI](https://docs.microsoft.com/en-us/power-bi/consumer/end-user-reports).

### Overview

The Overview page provides an overview of customer satisfaction data. The following survey metrics are displayed across the top of the report:

- **Survey invitations**: Total number of survey invitations sent.
- **Survey responses**: Number of non-anonymous survey responses received.
- **NPS**: Average NPS of the survey.
- **Sentiment**: Sentiment of respondents based on the survey responses.

The following information is displayed below the survey metrics:

- **Net Promoter Score**: The trend of average NPS over a period of time. The x-axis displays the time period and y-axis displays the average NPS. You can filter the NPS chart using the following filters to view NPS variations and take effective decisions accordingly:

  - **Trend**: Average NPS trend over a period of time is displayed by default. 
  - **Location**: Displays the NPS trend by location. This helps you to view the locations from where the maximum responses are coming and take decisions accordingly. For example, you received NPS from three locations: Loc1, Loc2, and Loc3. Insights showed that Loc3 has a better NPS then other two locations. You might take the decision to focus on Loc1 and Loc2 and find out the ways to improve NPS. 
  - **Case priority**: Displays the NPS trend by case priorities, such as high, medium, and so on.
  - **Case origin**: Displays the NPS trend by the origin of the case, such as Facebook, phone, twitter, and so on.
  - **Case type**: Displays the NPS trend by the type of a case, such as problem, request, question, and so on.
  - **Product**: Displays the NPS trend by products.

- **Key Phrases**: Displays a word cloud of the key phrases used in sentiment analysis. You can filter to see only the positive or negative key phrases or all key phrases.

### Agent Performance

The Agent Performance page provides the agent centric view of the satisfaction data. This page will help customer service managers to analyze an agent's performance based on the survey responses. The following information is displayed:

- **NPS**: Average NPS of the survey.
- A bubble chart at the top of the report displaying NPS distribution according to the number of agents.
- An NPS chart is displaying the trend of average NPS over a period of time.
- A grid containing top 10 agents' names and their corresponding NPS. You can select an agent's name to see the agent specific data in all other charts.
- **Key Phrases**: Displays a word cloud of the key phrases used in sentiment analysis. You can filter to see only the positive or negative key phrases or all key phrases.

### Customer Satisfaction

The Customer Satisfaction page provides the customer centric view of the satisfaction data. This page will help customer service managers to analyze a customer's satisfaction based on the survey responses. The following information is displayed:

- **NPS**: Average NPS of the survey.
- A bubble chart at the top of the report displaying NPS distribution according to the number of customers.
- An NPS chart is displaying the trend of average NPS over a period of time.
- A grid containing top 10 satisfied customers and their corresponding NPS. You can select a customer's name to see the customer specific data in all other charts.
- **Key Phrases**: Displays a word cloud of the key phrases used in sentiment analysis. You can filter to see only the positive or negative key phrases or all key phrases.