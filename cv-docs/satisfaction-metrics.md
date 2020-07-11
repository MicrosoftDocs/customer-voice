---
title: "Work with satisfaction metrics"
description: "Instructions for working with satisfaction metrics"
ms.date: 07/21/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Add and configure satisfaction metrics

Organizations use various metrics to determine the effectiveness of the experiences they provide to their customers. They track a subset of these metrics daily, and this forms the basis for measuring their performance. These metrics, called *satisfaction metrics*, are measurement systems you can use to measure your customer experience. This ensures that the data you collect through surveys can be analyzed successfully, and you can make decisions accordingly.<!--All edits this paragraph: Suggested.-->

Dynamics 365 Customer Voice includes support for adding the following standardized satisfaction metrics and mapping them to survey questions:

- **Net Promoter Score<!--I see that the trademark "bug" is used in the UI, but unless required by a mandate from CELA, we don't use trademark bugs for anything on docs. Please see https://microsoft.sharepoint.com/sites/celaweb-copyrights-trademarks-and-patents/sitepages/trademarks-trademark-list-and-usage.aspx--> (NPS)**: NPS is a metric used to measure customer loyalty. The score is calculated from the NPS-type question by using a scale from 0 through 10.<!--Writing Style Guide wants us to use "from x through y" to indicate a range.--> The respondents are grouped as follows:
  - **Detractors** are those who respond with a score from 0 through 6.
  - **Passives** are those who respond with a score of 7 or 8.<!--Edit okay? I assume you can't choose 7.5 (for example).-->
  - **Promoters** are those who respond with a score of 9 or 10.<!--Edit okay? -->

  NPS is calculated by subtracting the percentage of detractors from the percentage of promoters. The score is a number that can range from &ndash;100 to 100.

- **Sentiment**: Sentiment is a metric used to identify customer sentiment<!--Suggested.--> toward<!--Via Writing Style Guide.--> a product or a service. Sentiment groups the responses to a text-based question<!--Suggested.--> as positive, negative, or neutral.

- **Customer Satisfaction (CSAT)**: CSAT is a metric used to measure the level of satisfaction customers have with a product or a service. CSAT is measured by responses to rating-type questions.  

Satisfaction metrics are defined at the project level. If you create a project from one of the ready-to-use project templates in Dynamics 365 Customer Voice<!--Suggested, just to emphasize that these are new.-->, satisfaction metrics are already created and mapped to survey questions. However, you can add more metrics as needed. If you create a project from the **Blank** project template, you need to add satisfaction metrics and map them to the questions.

After you've received responses to your survey, a dashboard is created automatically for each set of metrics, showcasing recent scores and trends. The dashboard is available on the **Reports** tab in the left pane<!--Via Writing Style Guide.-->.

**To add satisfaction metrics**
<!--Took the H2 away to be parallel with other topics. Also, please note that all these graphics are much bigger than they need to be.-->
1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Satisfaction metrics**.

    ![Satisfaction metrics menu item](media/satisfaction-metrics-button.png "Satisfaction metrics menu item")

3. In the **Satisfaction metrics** panel, select **Add metrics**, and then select the type of metric you want to add.

    ![Add satisfaction metrics](media/add-metrics.png "Add satisfaction metrics")

4. Enter the following information:

    - **Name**: Name of the satisfaction metric.

    - **Add description**: Expand the section, and add an optional description for the satisfaction metric.

    - **<survey_name> question**: Choose the question you want to map to the satisfaction metric.

      ![Add satisfaction metrics details](media/metric-fields.png "Add satisfaction metrics details")

5. To see questions from other surveys in the project that are also<!--Edit okay? I wasn't sure what this meant.--> mapped to the metric, expand the **Other questions using this metric** section.

6. Select **Save**.

7. To add more metrics, repeat steps 3 through 6.

**To edit satisfaction metrics**

After you've created the satisfaction metrics you need, you can edit their details or delete the ones that you don't need.<!--Suggested.-->

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Satisfaction metrics**.

3. To edit a metric, expand it, and then update the name and description as required. If you change the question that's mapped to the metric, a confirmation message appears. Select **Change** in the confirmation message to continue.

4. Select **Save**.

5. To delete a metric, hover over the metric, and then select **Delete**.

6. In the confirmation message that appears, select **Delete** to continue with the deletion.
