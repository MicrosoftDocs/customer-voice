---
title: "Create a multilingual survey | MicrosoftDocs"
description: "Instructions for creating a multilingual survey with Customer Voice"
ms.date: 07/01/2020
ms.service:
  - "dynamics-365-sales"
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Create a multilingual survey

You can create a multilingual survey by adding multiple languages to a single survey. You can then add translations for each language. This helps you increase your customer base and allows respondents to take the survey in their preferred language.

When you create a multilingual survey, respondents can choose their preferred language from the language selector at the upper-right corner of the survey.

> [!div class=mx-imgBorder]
> ![Select a language for the survey](media/lang-select.png "Select a language for the survey") 

**To create a multilingual survey**

1.	[Add survey language](#step-1-add-survey-language)
2.	[Add translations](#step-2-add-translations)

## Step 1: Add survey language

1.	Open the survey in which you want to enable multiple languages.

2.	Select **Customization** at the right-side of the page, and then select **Languages**.

    > [!div class=mx-imgBorder]
    > ![Multilingual button](media/multilingual-button.png "Multilingual button") 

3.	In the **Languages** pane, select **Add language**.

    > [!div class=mx-imgBorder]
    > ![Multilingual pane](media/multilingual-pane.png "Multilingual pane")

4.	From the list of languages, browse to and select the required language.

    > [!div class=mx-imgBorder]
    > ![Browse and select the required language](media/lang-list.png "Browse to and select the required language") 

5.	If required, select **Add language** to add more languages. The added languages are displayed in the pane.

    > [!div class=mx-imgBorder]
    > ![Languages added for the survey](media/lang-added.png "Languages added for the survey")

> [!NOTE]
> You can add up to 20 languages to your survey.

## Step 2: Add translations

You can choose from two options for adding translations:

1. [Translate all languages in bulk](#option-1-translate-all-languages-in-bulk)
2. [Translate individual languages](#option-2-translate-individual-languages)

### Option 1: Translate all languages in bulk

1. In the **Languages** pane, select **Download an Excel template here** to download an Excel file containing strings in the primary language and columns for each of the selected languages. For example, **es** for Spanish or **fr** for French.

    > [!div class=mx-imgBorder]
    > ![Download Excel file to edit all languages](media/download-excel.png "Download an Excel file to edit all languages")

3. Open the Excel file and add translations for each language in its respective column.

4. After adding translations for all languages in the Excel file, go to the **Languages** pane, and then select **Upload**.

    > [!div class=mx-imgBorder]
    > ![Upload Excel file containing translations for all languages](media/upload-excel.png "Upload the Excel file containing translations for all languages") 

5. Browse to and select the Excel file in which you have added translations.

After uploading the Excel file, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

> [!div class=mx-imgBorder]
> ![Translated survey](media/translated-survey.png "Translated survey")

> [!NOTE]
> - The first column in the Excel file contains strings in the primary language and isn't editable.
> - You must ensure that a translation for each string is provided in the Excel file.
> - We recommend that you download the latest Excel file every time you add or edit the translations. This ensures that the latest strings and languages are available.
> - We recommend that you _not_ make a copy of the Excel file and add strings to it, or change the file name extension. These actions might result in upload failure.

### Option 2: Translate individual languages

1.	In the **Languages** pane, hover over the language for which you want to add translations, and then select the **Edit** icon.

    > [!div class=mx-imgBorder]
    > ![Edit the language added for the survey](media/edit-lang.png "Edit the language added for the survey")

2.	Select the survey title, description, and questions with their corresponding options, and then enter translated text for all survey elements.

    > [!div class=mx-imgBorder]
    > ![Translated text added in the survey](media/translation-added.png "Translated text added in the survey") 

3.	After you've added translated text for all elements in the survey, select **Back** in the upper-left corner of the page to go back to the survey editor.

4.	Repeat steps 2 through 3 to add translations for other languages.

After adding translations for all languages, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

> [!div class=mx-imgBorder]
> ![Translated survey](media/translated-survey.png "Translated survey") 

## Manage translations  

After adding translations for the required languages in your survey, you can either edit the existing translation or delete a language.

1.	Open the multilingual survey in which you want to manage translations.

2.	Select **Customization** at the right-side of the page, and then select **Languages**.

    > [!div class=mx-imgBorder]
    > ![Multilingual button](media/multilingual-button.png "Multilingual button")

3.	To edit the translations, hover over the language for which you want to edit translations, and then select the **Edit** icon.

    > [!div class=mx-imgBorder]
    > ![Edit the language added for the survey](media/edit-lang.png "Edit the language added for the survey")

    > [!NOTE]
    > To edit all languages together, select **Edit all** and follow the steps in [Option 1: Translate all languages in bulk](#option-1-translate-all-languages-in-bulk).

4.	Edit the translations as required.

5.	To delete a language, hover over the language to be deleted, and then select the **Delete** icon.

    > [!div class=mx-imgBorder]
    > ![Delete the language](media/delete-lang.png "Delete the language") 

### See also

[Create a new survey](create-new-survey.md)<br>
[Apply a theme to a survey](apply-theme.md)<br>
[Preview and test a survey](preview-test-survey.md)<br>
[Create a branching rule](create-branching-rule.md)<br>
[Personalize a survey](personalize-survey.md)<br>
[Format text in a survey](survey-text-format.md)<br>
[Create a classic form](create-classic-form.md)<br>
[Create a multiple-page survey](create-multipage-survey.md)
