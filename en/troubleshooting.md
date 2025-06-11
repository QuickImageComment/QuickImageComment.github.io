---
layout: pageOwnNav

title: Trouble shooting
description: Trouble shooting.

language: en
language_reference: troubleshooting

published: true
order: 3
toc: true
---

This page contains problems/questions and their solutions/answers. The page is intended as a supplement to the user manual or the help file supplied with the program. Specific problems and questions are dealt with here, the solution or answer to which cannot be found in the user manual or is rather difficult to find. In particular, new problems or questions of general interest can be added here at short notice.

New entries will be added at the top.

### Control elements are partially concealed or content is truncated
The size of most masks can be adjusted. In some cases, the size of individual sections, especially in the main mask, can also be adjusted. Normally, a mask or area cannot be made so small that there is no longer room for all the control elements. In special cases, however, it is possible to make an area so small that control elements overlap or content is truncated so that more space is available in another, more important area.

Remedy: Masks can be enlarged at the edges using the left mouse button. Sub-areas whose size can be changed within a mask can be enlarged by dragging the gray deviding lines.

### Texts in the masks are not translated
If labels or messages are not translated, please send information to <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a>. If so, the relevant text has unfortunately been overlooked in the translation.

If field descriptions are not translated, there may be two reasons for this.

The translation of the field descriptions is very time-consuming and in some cases the original English description is unclear, so it has not yet been translated. No field descriptions have yet been translated into French. Here too, please send information to <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a> so that a translation can be sought.

When the program is started for the first time, an initial configuration is created that defines which fields are displayed for various areas (e.g. "Overview"). The descriptions are taken according to the selected language. If the language is changed later, these fields and their descriptions are no longer changed because - apart from the initial filling - they are not changed by the program but by the user.

There are several ways to obtain field descriptions in the desired language:

* Applies only to German: If you have not yet made any or very few configuration changes yourself, it is easiest to delete the existing configuration file (QuickImageComment.ini or QuickImageCommentX64.ini in<br>C:\Users\{username}\AppData\Roaming)<br>and restart the program with the desired language.
* Only applies to German: If you have already made configuration changes and are familiar with a text comparison tool such as WinDiff or WinMerge, you should rename the existing configuration file. Then restart the program with the desired language and compare the old configuration file with the new one. The lines beginning with "MetaDataDefFor..." contain the descriptions that are displayed in the masks. These lines are copied from the newly created file because the descriptions are available there in the desired language. All other lines are taken from the renamed file and thus retain your own configuration changes.
* You can change the descriptions yourself in the "Field definitions" screen (Menu: Tools - Field definitions). However, this is a bit of work.

### Search for a location in map view returns no result
If the search terms were spelled correctly, the corresponding location could probably not be found by Nominatim. To verify this, the query can be repeated on the [Nominatim test page](https://nominatim.openstreetmap.org/ui/search.html). If a result is returned there, please send a message with the query to <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a> so that the problem can be solved within QuickImageComment.

### There is a red bar in the "Overview" tab of the main screen
In the "Overview" tab, a red bar on the left indicates that there are anomalies or errors in the properties. These are displayed at the bottom of the tab. Anomalies can be:
* For certain properties for which there should only be one value, there are several values in the screen.
* The various properties (Exif, IPTC, XMP) selected in the "Settings" screen to save the artist (author) and comment have different values.

Errors can be reported by the exiv2 library when reading the properties, e.g. "The memory contains data of an unknown image type".

Errors can also occur when displaying the image. If a message starting with "BitmapDecoder:" or "LibRaw:" is displayed next to "Image display error", a codec for reading the RAW image is missing and should be installed. Alternatively, you can install the Microsoft Raw Image Extension, which supports various RAW formats. Other messages indicate a software error and should be reported to <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a>.

