---
title: "Create a multilingual survey | MicrosoftDocs"
description: "You can add multiple languages and their translations to a survey. This topic explains how to create a multilingual survey with Dynamics 365 Customer Voice."
ms.date: 08/16/2021
ms.service: dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Create a multilingual survey

A survey created in Dynamics 365 Customer Voice can be translated to multiple languages. Once you setup the translations for the survey, a respondent can choose to take the survey in the language of their choice. This helps you increase your customer base and allows respondents to take the survey in their preferred language. A survey having translations in multiple languages is known as a multilingual survey.

To create a multilingual survey, you must first add the languages and then add translations for each of the added language. 

When you create a multilingual survey, you can also allow or restrict respondents to choose their preferred language from the language selector at the upper-right corner of the survey. More information: [Restrict respondents to change survey language](#restrict-respondents-to-change-survey-language)

![Select a language for the survey.](media/select-survey-lang.png "Select a language for the survey") 

To create a multilingual survey, you must first add a language (additional or custom) and then add translations for the corresponding strings in the survey.

> [!NOTE]
> Dynamics 365 Customer Voice supports 44 languages out-of-the-box. You can also add custom languages as per the requirement.

## Language types available in Dynamics 365 Customer Voice

### Root language

Root language is the language in which the survey is originally created. For example, if you are using the Dynamics 365 Customer Voice application in French locale, and are creating all your surveys in French locale – that is your _root language_. In short, the language you see in the designer is the root language of the survey. The root language is automatically set as the default language for the respondent. The default language can be selected from a list of languages supported in Dynamics 365. You can change it as per your requirement. More information: [Change the default language](#change-the-default-language)

> [!NOTE]
> The root language cannot be changed for the survey. For example, let's assume you have used the Dynamics 365 Customer Voice application in German locale and created your root survey in German locale. Then, you decided to use the Dynamics 365 Customer voice application in English locale. While all the other parts of the application will be displayed in English, the original survey text will continue to be in German. You cannot remove the root language of the survey unless you explicitly delete the survey.

### Additional languages

Additional languages are the languages in which a survey can be rendered in addition to the root language.There are two types of additional languages which can be setup for a survey within Customer Voice:

- **Out of the box languages**: These languages can be selected from a list of languages supported in Dynamics 365. These languages can be added, edited, and deleted from the Dynamics 365 Customer Voice interface. The system strings are translated automatically. More information: [Add additional languages](#add-additional-languages)

- **Custom languages**: These are the languages that are not included in the list of Dynamics 365 supported languages. You can define a language's display name and code. Custom languages can be added, edited, and deleted from the Dynamics 365 Customer Voice interface. The system strings are not translated automatically and are visible in the survey's default language.


## Add additional languages

Once you've completed the setup of your survey in the root language, you can add additional languages to your survey from the **Languages** panel. After adding the languages, you can add translations either in bulk for all languages or to each individual language. The system strings are translated automatically for the out of the box languages. For custom languages, the system strings are not translated automatically and are visible in the survey's default language.

### Step 1: Add additional languages

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

   The **Languages** panel is displayed with the root language selected and set as the default language for the survey.

   ![Root language for the survey ](media/root-lang.png "Root language for the survey.")

3. In the **Languages** panel, select **Add language**.

4. From the list of languages, browse to and select the out of the box languages you want. You can also search for a language and then select it.

    ![Browse to and select the required language ](media/lang-list.png "Browse to and select the required language")

    > [!NOTE]
    > You can select multiple languages by selecting the check boxes next to each language.

    If you don't find the language in the list of out of the box languages, you can add custom languages. 

5. In the **Languages** panel, select **Add language**, and then select **Add another language**.

   ![Add custom language in a survey ](media/add-custom-lang.png "Add custom language in a survey")

6. In the **Enter language name** field, enter the name of the custom language you want to add.

7. In the **Enter code** field, enter the code of the custom language. 

   Let's say, you want to add the **Spanish (Mexico)** language to your survey. You searched in the languages list and found only **Spanish (Spain, International Sort)**. In this case, you must manually add **Spanish(Mexico)** to the languages list. You'll define the display name as **Spanish(Mexico)** and the language code as **es-MX**.

   ![Custom language being added to a survey ](media/add-custom-lang-1.png "Custom language being added to a survey")

8. Select anywhere in the **Languages** panel to save the changes.

9. Repeat steps 5 through 8 to add more custom languages.

   The added languages are displayed in the panel along with their locale code. You can use this locale code in the **locale** variable while sending personalized survey invitations.

   ![Languages added for the survey ](media/lang-added.png "Languages added for the survey.")

> [!NOTE]
> - The language code you enter is validated against the existing list. You cannot have two languages defined with the same language code for the survey.
> - You can add up to 90 languages per survey.


### Step 2: Add translations

After adding the out of the box and custom languages, you can choose from two options for adding translations:

-  Translate all languages in bulk by using the Excel file

-  Translate individual languages from the Dynamics 365 Customer Voice interface

#### Option 1: Translate all languages in bulk

1. In the **Languages** panel, expand **Advanced options**, and then select **Download template** to download an Excel file containing strings in the primary language and columns for each of the selected languages. For example, **de** for German or **fr-FR** for French.

    ![Download an Excel file to edit all languages](media/download-excel.png "Download an Excel file to edit all languages.")

2. Open the Excel file and add translations for each language in its respective column.

3. After adding translations for all languages in the Excel file, go to the **Languages** panel, expand **Advanced options**, and then select **Upload**.

4. Browse to and select the Excel file in which you have added translations.

After uploading the Excel file, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

![Translated survey.](media/translated-survey.png "Translated survey")

> [!NOTE]
> - The first column in the Excel file contains strings in the primary language and isn't editable.
> - You must ensure that a translation for each string is provided in the Excel file.
> - We recommend that you download the latest Excel file every time you add or edit the translations. This ensures that the latest strings and languages are available.
> - We recommend that you _not_ make a copy of the Excel file and add strings to it, or change the file name extension. These actions might result in upload failure.

#### Option 2: Translate individual languages

1. In the **Languages** panel, select the language for which you want to add translations.

   Alternately, you can also hover over a language, select **More options** (three dots), and then select **Add translation**.

2. Select the survey element, and then enter the translated text. Repeat this step for all survey elements.

   ![Translated text added for a few elements in the survey.](media/translation-added.png "Translated text added a few elements in the survey") 

3. After you've added translated text for all elements in the survey, select **Back** in the upper-left corner of the page to go back to the **Languages** panel.

4. Repeat steps 1 through 3 to add translations for other languages.

After adding translations for all languages, you can preview the survey to see whether everything works as expected. Select the language from the language selector at the upper-right corner of the survey.

![Translated survey.](media/translated-survey.png "Translated survey") 


## Restrict respondents to change survey language

If you've created a multilingual survey, you can choose if your respondents can select a preferred language to respond to the survey or view the survey in the language selected as per their browser language or locale variable. By default, respondents are allowed to change their survey language.

**To restrict respondents to change their survey language**

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

3. In the **Languages** panel, expand **Advanced options**, and then turn off the **Respondents can change languages** toggle.

   ![Restrict respondents to change survey language ](media/change-lang-respondent.png "Restrict respondents to change survey language")

> [!NOTE]
> When this setting is turned off, a respondent can see only one language and cannot change the language at all.

## Change the default language

Default language is the language in which the survey is loaded if no explicit locale variable is passed or if the respondent is using the web browser in a language for which you have not added a translation.

Let's assume, you use the Dynamics 365 Customer Voice application in English locale. When you create a survey, English is set as the default language for the survey. However, a majority of your survey respondents are from France, so you can change the default language from English to French.

> [!NOTE]
> The survey gets loaded in the default language only as a last resort – in case if the user is using a browser language which is different from the available languages and if there is no explicit locale variable passed through the URL. 

You can change the default language for your survey from the **Languages** panel. Note that you can change the default language only when multiple languages are added to the survey.

1. Open the survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

3. From the list of languages, hover over a language, select **More options** (three dots), and then select **Set as default**.

    ![Change default language of the survey ](media/survey-default-lang.png "Change default language of the survey")

    The default language is marked with ![Default language marker](media/default-lang-marker.png "Default language marker") in the **Default** column.

## Manage translations

After adding translations for the required languages in your survey, you can edit the existing translation or delete a language.

1. Open the multilingual survey.

2. On the **Design** tab, select **Customization** at the right side of the page, and then select **Languages**.

3. To edit the translations, select the language for which you want to edit translations.

4. Edit the translations as required.

5. To delete a language, hover over the language to be deleted, select **More options** (three dots), and then select **Delete**.

You cannot retrieve the already translated strings for a deleted language. You cannot retrieve this after a language is deleted.

## Locale codes to use in survey variable

When you create a multilingual survey, you can use the **locale** survey variable to set the default language for displaying the survey. Following is the list of out of the box languages within Dynamics 365 Customer Voice and their associated language codes.

|     Language   display name                  |     Language   ISO Code    |
|----------------------------------------------|----------------------------|
|     Catalan                                  |     ca                     |
|     Serbian   (Cyrillic, Serbia)             |     sr-cyrl-rs             |
|     Danish                                   |     da                     |
|     German                                   |     de                     |
|     Estonian                                 |     et                     |
|     Spanish   (Spain, International Sort)    |     es-ES                  |
|     Basque                                   |     eu                     |
|     French   (France)                        |     fr-FR                  |
|     Galician                                 |     gl                     |
|     Croatian                                 |     hr                     |
|     Indonesian                               |     id                     |
|     Italian                                  |     it                     |
|     Latvian                                  |     lv                     |
|     Lithuanian                               |     lt                     |
|     Hungarian                                |     hu                     |
|     Malay                                    |     ms                     |
|     Dutch                                    |     nl                     |
|     Norwegian Nynorsk   (Norway)             |     nb-no                  |
|     Polish                                   |     pl                     |
|     Portuguese   (Brazil)                    |     pt-br                  |
|     Portuguese   (Portugal)                  |     pt-pt                  |
|     Russian                                  |     ru                     |
|     Romanian                                 |     ro                     |
|     Slovak                                   |     sk                     |
|     Slovenian                                |     sl                     |
|     Serbian (Latin,   Serbia)                |     sr-latn-rs             |
|     Finnish                                  |     fi                     |
|     Swedish                                  |     sv                     |
|     Vietnamese                               |     vi                     |
|     Turkish                                  |     tr                     |
|     Ukrainian                                |     uk                     |
|     Czech                                    |     cs                     |
|     Greek                                    |     el                     |
|     Bulgarian                                |     bg                     |
|     Kazakh                                   |     kk                     |
|     Hebrew                                   |     he                     |
|     Arabic                                   |     ar                     |
|     Hindi                                    |     hi                     |
|     Thai                                     |     th                     |
|     Chinese   (Simplified)                   |     zh-Hans                |
|     Chinese   (Traditional)                  |     zh-Hant                |
|     Japanese                                 |     ja                     |
|     Korean                                   |     ko                     |
|     English   (United States)                |     en-us                  |


## Frequently asked questions

### How many languages can be added to a survey?

You can add up to 90 languages per survey. This consists of a total of out of the box and custom languages.

### How does Customer Voice decide which language to show to a particular respondent?

If you are sending a personalized survey invitation through email or Power Automate, you can define the locale code using the out of the box variable per invitation.

Let's say, your customer Milton's locale code in your backend CRM system contact record is set to “ar”. You can pass that as a parameter in your personalized invitation. This will ensure that the survey loads by default in Arabic for Milton.

You can also pass the locale parameters per contact by using a CSV file . More information: [Import contacts from a CSV file](send-survey-email.md#import-contacts-from-a-csv-file)

If you are not sending survey invitation through a personalized invitation link, and you know that all the respondents to your anonymous survey must see the survey in Arabic. In this case, you can have an explicit **lang=ar** parameter added to the anonymous URL of the survey. This will ensure that the survey loads in the Arabic language for all the respondents.

If you don't pass the value of the **lang** parameter in the URL, the survey loads in the browser language of the respondent.

So, the order of priority is:

1. The **locale** variable defined for personalized invitations sent through Power Automate or Email
2. The **lang** parameter defined in the URL 
3. Browser language of the respondent
4. Fallback language of the survey (in case the browser language is not setup in the survey)

### Which should I use for setting up translation strings? Uploading files through Excel or directly updating from the application's interface?

If you have a large number of languages added to your survey, and you need to get the translation strings verified from a translation team, you can upload the translations in the Excel file.

If you have a few languages, and you have the translated strings available handy, you can use the application's interface to update the translation strings.

### When should I setup the translation?

We recommend that you start updating the translation strings, only when the setup of the survey in its root language is complete. It makes updating the translations more manageable, and easy to maintain.

### What happens to email templates?

You will need to setup the localized templates for every language you want to add to the survey. After add the required languages to the survey, you can choose the languages from the **Language** list. You can then create separate email templates for all the languages you added to the survey. More information: [Create multilingual email templates](send-survey-email.md#create-multilingual-email-templates)

Let's say you have added seven additional languages to the survey. You will have to create seven email templates (one for each language). You will have to pass the value of the language code as a **locale** variable either in email or Power Automate, so that the customer gets the survey in the intended language.

### See also

[Add and configure satisfaction metrics](satisfaction-metrics.md)<br>
[Add logic by creating branching rules](create-branching-rule.md)<br>
[Personalize your survey by adding variables](personalize-survey.md)<br>
[Add branding to your survey](survey-branding.md)<br>
[Add formatting to your survey](survey-formatting.md)<br>
[Add formatting to survey elements](survey-text-format.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
