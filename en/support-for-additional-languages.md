---
layout: page

title: Support for additional languages
description: Support for additional languages.

language: en
language_reference: support-for-additional-languages

published: true
order: 8
---

# Support for additional languages

New languages can generally be supported without program changes, if appropriate language files are created. Program changes are only necessary if it is not possible to keep the translations short enough to fit into the available space.

Below is an explanation of how language files are created for other languages - in the hope that someone is willing to do the necessary translation work, if necessary with the help of [https://translate.google.com](https://translate.google.com) or [https://www.deepl.com/translator](https://www.deepl.com/translator).

It is useful to inform quickimagecomment@gmail.com when you start a translation. If there are several volunteers for one language, this can be coordinated and duplication of work can be avoided. All files that are the basis for the translation can be found in the GitHub repository:<br>
[https://github.com/QuickImageComment/QuickImageComment](https://github.com/QuickImageComment/QuickImageComment)

Support for additional languages is divided into three areas, which are described below. Most important would be the translation of the mask texts and messages.

### Translations for the mask texts and messages

The following Excel file is used for these translations:<br>
[Translation_QIC.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_QIC.xlsm)

The file contains about 700 entries with together about 3000 words. This is a lot of translations, but the texts should be quite easy to translate. The file contains the texts in German and English. There is space for a third language, for other languages space can be created if needed. Detailed instructions are in the Excel file in the sheet "Anleitung-Instructions".

### Translations for tag names and related descriptions

For these translations, a separate Excel file is used for each language:

[Translation_Tags_Deutsch.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_Deutsch.xlsm)<br>
[Translation_Tags_French.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_French.xlsm) (So far only rudimentarily filled)<br>
[Translation_Tags_Spanish.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_Spanish.xlsm) (So far only rudimentarily filled)

Basis are the English tag names and descriptions from exiv2. Additionally there are a few entries for tags, which are defined internally in QuickImageComment. exiv2 knows about 3500 tags, some of them repeating. For example, FNumber appears among others as Exif.Image.FNumber, Exif.MinoltaCs5D.FNumber, Exif.MinoltaCs7D.FNumber and
Exif.MinoltaCsNew.FNumber. Without repetitions there are still about 2200 entries.

Some descriptions were translated for many languages within the exiv2 project. These translations are included in the files for Spanish and French. If somebody wants to translate another language: Please mail tomail@quickimagecomment.de, then a corresponding file will be provided.

While the mask texts and messages should be translated completely, there is no claim to completeness here, especially since some tags have a very specific meaning (e.g. "The complete scientific name of the genus in which the taxon was classified"). There are also some tags whose meanings are difficult to understand and therefore correspondingly difficult to translate.

Detailed instructions can be found in the Excel file in the sheet "Anleitung-Instructions".

### Translation of the user manual

The translation of the user manual is probably the most work. It contains about 80 pages. In addition, there are several pages with license conditions, but these do not have to be translated because the English version is legally binding. For the GPL, the user manual contains a German translation that is not legally binding. For other languages you can - if you like - surely find a translation on the internet.

Basis for the translation are the Word documents of the user manuals:<br>
[QIC_Benutzeranleitung.docm](https://github.com/QuickImageComment/QuickImageComment/blob/main/UserManual/QIC_Benutzeranleitung.docm) (German)<br>
[QIC_User_Manual.docm](https://github.com/QuickImageComment/QuickImageComment/blob/main/UserManual/QIC_User_Manual.docm) (English)

The other formats (PDF, HTML and CHM) are generated from it.


 

 