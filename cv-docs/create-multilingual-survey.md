---
title: "Create a multilingual survey | MicrosoftDocs"
description: "Instructions for creating a multilingual survey with Dynamics 365 Customer Voice"
ms.date: 07/21/2020
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

![Select a language for the survey](media/select-survey-lang.png "Select a language for the survey") 

**To create a multilingual survey**

1.	[Add survey language](#step-1-add-survey-language)
2.	[Add translations](#step-2-add-translations)

## Step 1: Add survey language

1.	Open the survey.

2.	On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

    ![Languages menu item](media/languages-menu-button.png "Languages menu item") 

3.	In the **Languages** panel, select **Add language**.

    ![Multilingual pane](media/languages-pane.png "Multilingual pane")

4.	From the list of languages, browse to and select the language you want.

    ![Browse to and select the required language](media/lang-list.png "Browse to and select the required language") 

5.	If required, select **Add language** to add more languages. The added languages are displayed in the pane.

    ![Languages added for the survey](media/lang-added.png "Languages added for the survey")

> [!NOTE]
> You can add up to 23 languages to your survey.

## Step 2: Add translations

You can choose from two options for adding translations:

1. [Translate all languages in bulk](#option-1-translate-all-languages-in-bulk)
2. [Translate individual languages](#option-2-translate-individual-languages)

### Option 1: Translate all languages in bulk

1. In the **Languages** panel, select **download an Excel template here** to download an Excel file containing strings in the primary language and columns for each of the selected languages. For example, **es** for Spanish or **fr** for French.

    ![Download an Excel file to edit all languages](media/download-excel.png "Download an Excel file to edit all languages")

3. Open the Excel file and add translations for each language in its respective column.

4. After adding translations for all languages in the Excel file, go to the **Languages** panel, and then select **Upload**.

    ![Upload the Excel file containing translations for all languages](media/upload-excel.png "Upload the Excel file containing translations for all languages") 

5. Browse to and select the Excel file in which you have added translations.

After uploading the Excel file, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

![Translated survey](media/translated-survey.png "Translated survey")

> [!NOTE]
> - The first column in the Excel file contains strings in the primary language and isn't editable.
> - You must ensure that a translation for each string is provided in the Excel file.
> - We recommend that you download the latest Excel file every time you add or edit the translations. This ensures that the latest strings and languages are available.
> - We recommend that you _not_ make a copy of the Excel file and add strings to it, or change the file name extension. These actions might result in upload failure.

### Option 2: Translate individual languages

1.	In the **Languages** panel, hover over the language for which you want to add translations, and then select the **Edit** icon.

    ![Edit the language added for the survey](media/edit-lang.png "Edit the language added for the survey")

2.	Select the survey element, and then enter the translated text. Repeat this step for all survey elements.

    ![Translated text added in the survey](media/translation-added.png "Translated text added in the survey") 

3.	After you've added translated text for all elements in the survey, select **Back** in the upper-left corner of the page to go back to the **Languages** panel.

4.	Repeat steps 1 through 3 to add translations for other languages.

After adding translations for all languages, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

![Translated survey](media/translated-survey.png "Translated survey") 

## Manage translations  

After adding translations for the required languages in your survey, you can edit the existing translation or delete a language.

1.	Open the multilingual survey.

2.	On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

    ![Languages menu item](media/languages-menu-button.png "Languages menu item")

3.	To edit the translations, hover over the language for which you want to edit translations, and then select the **Edit** icon.

    ![Edit the language added for the survey](media/edit-lang.png "Edit the language added for the survey")

    > [!NOTE]
    > To edit all languages together, follow the steps in [Option 1: Translate all languages in bulk](#option-1-translate-all-languages-in-bulk).

4.	Edit the translations as required.

5.	To delete a language, hover over the language to be deleted, and then select the **Delete** icon.

    ![Delete a language](media/delete-lang.png "Delete a language") 


## Locale codes to use in survey variable

When you create a multilingual survey, you can use the **locale** survey variable to set the default language for displaying the survey. You must use the language codes as provided in the following table:

|     Language code           |     Language                                   |
|---------------------------|------------------------------------------------|
|         af                |      Afrikaans                                 |
|           am-et           |      አማርኛ (ኢትዮጵያ)                        |
|           ar              |      العربية                                   |
|           as-in           |      অসমীয়া (ভাৰত)                       |
|           az-latn-az      |      azərbaycan (Azərbaycan)             |
|           be              |      Беларуская                                |
|           bg              |      български                                 |
|           bn-bd           |      বাংলা (বাংলাদেশ)                    |
|           bn-in           |      বাংলা (ভারত)                        |
|           bs-latn-ba      |      bosanski (Bosna i   Hercegovina)    |
|         ca                |      català                                    |
|         ca-es-valencia    |      valencià   (Espanya)                |
|         cs                |      čeština                                   |
|         cy-gb             |      Cymraeg (Y Deyrnas   Unedig)        |
|         da                |      dansk                                     |
|         de                |      Deutsch                                   |
|           el              |      Ελληνικά                                  |
|           en-gb           |      English (United   Kingdom)          |
|         en-us             |      English (United   States)           |
|         es                |      español                                   |
|           es-mx           |      español (México)                    |
|           et              |      eesti                                     |
|           eu              |      euskara                                   |
|           fa              |      فارسی                                     |
|           fi              |      suomi                                     |
|           fil-ph          |      Filipino   (Pilipinas)              |
|         fr                |      français                                  |
|         fr-ca             |      français   (Canada)                 |
|         ga-ie             |      Gaeilge (Éire)                      |
|           gd              |      Gàidhlig                                  |
|           gl              |      galego                                    |
|           gu              |      ગુજરાતી                                    |
|           ha-latn-ng      |      Hausa   (Najeriya)                  |
|         he                |      עברית                                     |
|         hi                |      हिन्दी                                     |
|         hr                |      hrvatski                                  |
|         hu                |      magyar                                    |
|         hy                |      Հայերեն                                   |
|         id                |      Indonesia                                 |
|         is                |      íslenska                                  |
|         it                |      italiano                                  |
|           ja              |      日本語                                    |
|           ka              |      ქართული                                   |
|           kk              |      қазақ тілі                                |
|           km-kh           |      ភាសាខ្មែរ (កម្ពុជា)                    |
|           kn              |      ಕನ್ನಡ                                      |
|           ko              |      한국어                                    |
|           kok             |      कोंकणी                                     |
|           ky              |      Кыргыз                                    |
|           lb-lu           |      Lëtzebuergesch (Lëtzebuerg)         |
|           lo              |      ລາວ                                       |
|           lt              |      lietuvių                                  |
|           lv              |      latviešu                                  |
|           mi-nz           |      te reo Māori (Aotearoa)             |
|           mk              |      македонски                                |
|           ml              |      മലയാളം                                    |
|           mn              |      монгол                                    |
|           mr              |      मराठी                                     |
|           ms              |      Melayu                                    |
|           mt-mt           |      Malti (Malta)                       |
|           nb-no           |      norsk bokmål (Norge)                |
|           ne-np           |      नेपाली (नेपाल)                        |
|           nl              |      Nederlands                                |
|           nn-no           |      nynorsk (Noreg)                     |
|           or-in           |      ଓଡ଼ିଆ (ଭାରତ)                          |
|           pa              |      ਪੰਜਾਬੀ                                     |
|           pl              |      polski                                    |
|           prs-af          |      درى (افغانستان)\u200F                     |
|           pt-br           |      português (Brasil)                  |
|           pt-pt           |      português (Portugal)                |
|           quz-pe          |      Runasimi (Perú)                     |
|           ro              |      română                                    |
|           ru              |      русский                                   |
|           sd-arab-pk      |      سنڌي (پاکستان)\u200F                      |
|           si-lk           |      සිංහල (ශ්‍රී   ලංකාව)                   |
|           sk              |      slovenčina                                |
|           sl              |      slovenščina                               |
|           sq              |      shqip                                     |
|           sr-cyrl-ba      |      српски (Босна и Херцеговина)        |
|           sr-cyrl-rs      |      српски (Србија)                     |
|           sr-latn-rs      |      srpski (Srbija)                     |
|           sv              |      svenska                                   |
|           sw              |      Kiswahili                                 |
|           ta              |      தமிழ்                                      |
|           te              |      తెలుగు                                     |
|           th              |      ไทย                                       |
|           tk-tm           |      Türkmen dili (Türkmenistan)         |
|           tr              |      Türkçe                                    |
|           tt              |      Татар                                     |
|           ug              |      ئۇيغۇرچە                                  |
|           uk              |      українська                                |
|           ur              |      اُردو                                      |
|           uz-latn-uz      |      o‘zbek (Oʻzbekiston)                |
|           vi              |      Tiếng Việt                                |
|           zh-cn           |      中文（中国）                        |
|           zh-hk           |      中文（香港特別行政區）              |
|           zh-tw           |      中文（台灣）                        |
|||


### See also

[Create a new survey](create-new-survey.md)<br>
[Preview and test a survey](preview-test-survey.md)<br>
[Create a branching rule](create-branching-rule.md)<br>
[Personalize a survey](personalize-survey.md)<br>
[Format text in a survey](survey-text-format.md)<br>
[Create a multiple-page survey](create-multipage-survey.md)
