---
layout: page

title: Metadaten in Windows Explorer
description: Metadaten in Windows Explorer

language: en
language_reference: meta-data-windows-explorer

published: true
order: 11
---

# Meta data in Windows Explorer

Some meta data can be displayed as columns in Windows Explorer. They can also be changed under Properties, "Details" tab. If you edit the same file with QuickImageComment (or a comparable program), this can lead to strange effects.

Example:
The starting point is an image from a digital camera. With Windows Explorer, "abc" is entered as Title. You open the image with QuickImageComment and find "abc" under Exif.Image.ImageDescription. Change the entry to "abcdef" and look it up in Windows Explorer. However, you still find under Title "abc".
The reason for this is that Windows Explorer stores titles and other metadata not just under one tag, but under several. When displaying meta data, several tags are checked and the first filled is used.

The following description is limited to information which usually may be filled by user for documentation purposes, so not all information visible in property tab "Details" of Windows Explorer are coverd. The description is based on tests with Windows Explorer under Windows 11 Home version 24H2 and Windows 10 Home version 1607.

The tag descriptions are taken from 
* [CIPA DC- 008-Translation-2023 Exif Version 3.0](https://www.cipa.jp/std/documents/download_e.html?DC-008-Translation-2023-E)
* [IPTC Photo Metadata User Guide](https://www.iptc.org/std/photometadata/documentation/userguide/)
* [XMP SPECIFICATION PART 1
DATA MODEL, SERIALIZATION, AND
CORE PROPERTIES](https://github.com/adobe/XMP-Toolkit-SDK/blob/main/docs/XMPSpecificationPart1.pdf)

### General rules

Windows Explorer writes information in all tags as listed below for the respective information. 

When displaying information, Windows Explorer checks the tags in the sequence as listed. Windows Explorer shows then the value of the first filled tag.

In some cases Windows Explorer allows to enter several values, but some associated tags do not allow several values. Then the values are concatenated, separated by the list separator defined in Windows regional settings (comma or semicolon). For example Exif.Image.XPKeyWords can hold only one value whereas there can be several values for Iptc.Application2.Keywords and Xmp.dc.subject.

Windows Explorer fills IPTC tags only, if the image already has an IPTC-section, i.e. has at least one IPTC tag filled.

### Title

| Tag name | Description|
|:---|:---|
| Xmp.dc.title | DCMI definition: A name given to the resource.<br>DCMI comment: Typically, a title will be a name by which the resource is formally known.<br>XMP addition: XMP usage is a title or name, given in various languages.| 
| Exif.image.imageDescription | A character string giving the content description of the image. It is possible to add a description of the content or comment such as "1988 company picnic" or the like |
| Iptc.application2.caption | The Description field, often referred to as a ‘caption', is used to describe the who, what (and possibly where and when) and why of what is happening in the photograph. It can include people’s names, their roles in the action, and location information. Geographic location details should also be entered in the Location fields. The amount of detail included will depend on the image and whether the image is documentary or conceptual. Typically, editorial images come with complete caption text, while advertising images may not.|
| Xmp.dc.description | DCMI definition: An account of the resource.<br>XMP addition: XMP usage is a list of textual descriptions of the content of the resource, given in various languages|
| Exif.Image.XPTitle | Not documented in Exif specification.<br>Description from [exiv2.org](https://exiv2.org/tags.html):<br>Title tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

### Subject

| Tag name | Description|
|:---|:---|
| Exif.Image.XPSubject | Not documented in Exif specification.<br>Description from [exiv2.org](https://exiv2.org/tags.html):<br>Subject tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

### Tags
When displaying, Windows Explorer shows all entries of following tags:

| Tag name | Description|
|:---|:---|
| Exif.Image.XPKeyWords |Not documented in Exif specification.<br>Description from [exiv2.org](https://exiv2.org/tags.html):<br>Keywords tag used by Windows, encoded in UCS2|
| Iptc.Application2.Keywords | Enter keywords to describe the visible and abstract content of the photograph.Keywords are in free text form, and may be single or compound terms.<br> Keywords are descriptive words added to an image to enable search and retrieval. They describe what is visible in the image and concepts associated with the image. Keywords are expressed as a list of terms. Keywords can be single or compound terms.|
| Xmp.dc.subject | DCMI definition: The topic of the resource.<br>DCMI comment: Typically, the subject will be represented using keywords, key phrases, or classification codes. Recommended best practice is to use a controlled vocabulary. To describe the spatial or temporal topic of the resource, use the dc:coverage element.<br>XMP addition: XMP usage is a list of descriptive phrases or keywords that specify the content of the resource.|
{:.tablestylegrey}

When writing, Windows Explorer fills these tags and additionally the following:
* Xmp.MicrosoftPhoto.LastKeywordIPTC
* Xmp.MicrosoftPhoto.LastKeywordXMP

Due to its name, you would expect Xmp.dc.subject to be assigned to the "Subject" group by Windows Explorer. However, the XMP specification stipulates that the tag contains a list of descriptive phrases or keywords that specify the content of the resource.

### Comments
When displaying, Windows Explorer shows the first filled entry of 

| Tag name | Description|
|:---|:---|
| Exif.Photo.UserComment | A tag for Exif users to freely write keywords or comments on the image. |
| Xmp.exif.UserComment | Like Exif.Photo.UserComment |
| Exif.Image.XPComment | Not documented in Exif specification.<br>Description from [exiv2.org](https://exiv2.org/tags.html):<br>Comment tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

The sequence of the first two tags can be different: in some cases Xmp.exif.UserComment is preferred to Exif.Photo.UserComment. The reason for this is not clear.

When writing, Windows Explorer fills Exif.Image.XPComment only and clears the other listed tags.

### Authors

| Tag name | Description|
|:---|:---|
| Exif.Image.Artist | This tag records name of the main person who created the image. The detailed format is not specified. When the field is left blank, it is treated as unknown.|
| Iptc.Application2.Byline | Name of the creator of the image. Where the artist cannot or should not be identified, the name of a company or organisation may be use.|
| Xmp.dc.creator | DCMI definition: An entity primarily responsible for making the resource.<br>DCMI comment: Examples of a creator include a person, an organization, or a service. Typically, the name of a creator should be used to indicate the entity.<br>XMP addition: XMP usage is a list of creators. Entities should be listed in order of decreasing precedence, if such order is significant. |
| Exif.Image.XPAuthor | Not documented in Exif specification,<br>Description from [exiv2.org](https://exiv2.org/tags.html):<br>Author tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

### Copyright

| Tag name | Description|
|:---|:---|
| Exif.Image.Copyright | Copyright information. It is the copyright notice of the person or organization holding rights to the image.|
| Iptc.Application2.Copyright | The Copyright Notice contains information required to assert copyright in the image and should contain the name of the current copyright holder, whether an individual or a company. The format will differ according to the relevant copyright legislation. It may include the copyright symbol ©, the year of publication, and other commonly used terms such as ‘All Rights Reserved.' If an image is Public Domain, it can be indicated here.|
| Xmp.dc.rights | DCMI definition: Information about rights held in and over the resource.<br>DCMI comment: Typically, rights information includes a statement about various property rights associated with the resource, including intellectual property rights.<br>XMP addition: XMP usage is a list of informal rights statements, given in various languages.|
{:.tablestylegrey}
