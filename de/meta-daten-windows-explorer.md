---
layout: page

title: Metadaten in Windows Explorer
description: Metadaten in Windows Explorer

language: de
language_reference: meta-data-windows-explorer

published: true
order: 11
---

# Metadaten in Windows Explorer

Einige Metadaten können im Windows Explorer als Spalten angezeigt werden. Sie können auch unter Eigenschaften, Registerkarte "Details", geändert werden. Wenn Sie dieselbe Datei mit QuickImageComment (oder einem vergleichbaren Programm) bearbeiten, kann dies zu seltsamen Effekten führen.

Beispiel:
Ausgangspunkt ist ein Bild von einer Digitalkamera. Im Windows Explorer wird als Titel "abc" eingegeben. Sie öffnen das Bild mit QuickImageComment und finden "abc" unter Exif.Image.ImageDescription. Ändern Sie den Eintrag in "abcdef" und schauen Sie im Windows Explorer nach. Unter Title ist dort aber immer noch "abc" zu finden.
Der Grund dafür ist, dass Windows Explorer Titel und andere Metadaten nicht nur unter einem Tag, sondern unter mehreren speichert. Bei der Anzeige von Metadaten werden mehrere Tags geprüft und der erste gefüllte verwendet.

Die folgende Beschreibung beschränkt sich auf Informationen, die normalerweise vom Benutzer zu Dokumentationszwecken ausgefüllt werden können. Es werden also nicht alle Informationen abgedeckt, die auf der Registerkarte "Details" des Windows Explorers sichtbar sind. Die Beschreibung basiert auf Tests mit dem Windows Explorer unter Windows 11 Home Version 24H2 und Windows 10 Home Version 1607.

Die Beschreibungen der Tags stammen aus
* [CIPA DC- 008-Translation-2023 Exif Version 3.0](https://www.cipa.jp/std/documents/download_e.html?DC-008-Translation-2023-E)
* [IPTC Photo Metadata User Guide](https://www.iptc.org/std/photometadata/documentation/userguide/)
* [XMP SPECIFICATION PART 1
DATA MODEL, SERIALIZATION, AND
CORE PROPERTIES](https://github.com/adobe/XMP-Toolkit-SDK/blob/main/docs/XMPSpecificationPart1.pdf)

### Allgemeine Regeln

Windows Explorer schreibt Informationen in alle Tags, wie unten für die jeweiligen Informationen aufgeführt.

Bei der Anzeige von Informationen prüft Windows Explorer die Tags in der aufgeführten Reihenfolge. Windows Explorer zeigt dann den Wert des ersten ausgefüllten Tags an.

In einigen Fällen erlaubt der Windows Explorer die Eingabe mehrerer Werte, aber einige zugehörige Tags lassen nicht mehrere Werte zu. Dann werden die Werte verkettet, getrennt durch das in den regionalen Windows-Einstellungen festgelegte Listentrennzeichen (Komma oder Semikolon). Zum Beispiel kann Exif.Image.XPKeyWords nur einen Wert enthalten, während es für Iptc.Application2.Keywords und Xmp.dc.subject mehrere Werte geben kann.

Der Windows Explorer füllt IPTC-Tags nur dann aus, wenn das Bild bereits einen IPTC-Abschnitt hat, d.h. wenn mindestens ein IPTC-Tag gefüllt ist.

### Titel

| Tag-Name | Beschreibung|
|:---|:---|
| Xmp.dc.title | DCMI definition: A name given to the resource.<br>DCMI comment: Typically, a title will be a name by which the resource is formally known.<br>XMP addition: XMP usage is a title or name, given in various languages. |
| Exif.image.imageDescription | A character string giving the content description of the image. It is possible to add a description of the content or comment such as "1988 company picnic" or the like |
| Iptc.application2.caption | The Description field, often referred to as a ‘caption', is used to describe the who, what (and possibly where and when) and why of what is happening in the photograph. It can include people’s names, their roles in the action, and location information. Geographic location details should also be entered in the Location fields. The amount of detail included will depend on the image and whether the image is documentary or conceptual. Typically, editorial images come with complete caption text, while advertising images may not. |
| Xmp.dc.description | DCMI definition: An account of the resource.<br>XMP addition: XMP usage is a list of textual descriptions of the content of the resource, given in various languages |
| Exif.Image.XPTitle |  Nicht dokumentiert in Exif Spezifikation.<br>Beschreibung von [exiv2.org](https://exiv2.org/tags.html):<br>Title tag used by Windows, encoded in UCS2 |
{:.tablestylegrey}

### Betreff

| Tag-Name | Beschreibung|
|:---|:---|
| Exif.Image.XPSubject | Nicht dokumentiert in Exif Spezifikation.<br>Beschreibung von [exiv2.org](https://exiv2.org/tags.html):<br>Subject tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

### Markierungen
Beim Anzeigen zeigt Windows Explorer alle Einträge der folgenden Tags an:


| Tag-Name | Beschreibung|
|:---|:---|
| Exif.Image.XPKeyWords |Nicht dokumentiert in Exif Spezifikation.<br>Beschreibung von [exiv2.org](https://exiv2.org/tags.html):<br>Keywords tag used by Windows, encoded in UCS2|
| Iptc.Application2.Keywords | Enter keywords to describe the visible and abstract content of the photograph.Keywords are in free text form, and may be single or compound terms.<br> Keywords are descriptive words added to an image to enable search and retrieval. They describe what is visible in the image and concepts associated with the image. Keywords are expressed as a list of terms. Keywords can be single or compound terms.|
| Xmp.dc.subject | DCMI definition: The topic of the resource.<br>DCMI comment: Typically, the subject will be represented using keywords, key phrases, or classification codes. Recommended best practice is to use a controlled vocabulary. To describe the spatial or temporal topic of the resource, use the dc:coverage element.<br>XMP addition: XMP usage is a list of descriptive phrases or keywords that specify the content of the resource.|
{:.tablestylegrey}

Beim Schreiben füllt der Windows Explorer diese Tags und zusätzlich die folgenden:
* Xmp.MicrosoftPhoto.LastKeywordIPTC
* Xmp.MicrosoftPhoto.LastKeywordXMP

Aufgrund des Namens erwartet man, dass Xmp.dc.subject von Windows Explorer eher der Gruppe "Betreff" (englisch Subject) zugeordnet wird. Aber die XMP Spezifikation sieht vor, das Tag eine Liste von beschreibenden Phrasen oder Schlüsselwörtern (englisch Keywords, im Windows Explorer in Deutsch wiederum als Markierungen bezeichnet) enthält, die den Inhalt der Ressource spezifizieren. 

### Kommentare
Bei der Anzeige zeigt der Windows Explorer den ersten gefüllten Eintrag von

| Tag-Name | Beschreibung|
|:---|:---|
| Exif.Photo.UserComment | A tag for Exif users to freely write keywords or comments on the image. |
| Xmp.exif.UserComment | Wie Exif.Photo.UserComment |
| Exif.Image.XPComment | Nicht dokumentiert in Exif Spezifikation.<br>Beschreibung von [exiv2.org](https://exiv2.org/tags.html):<br>Comment tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

Die Reihenfolge der ersten beiden Tags kann unterschiedlich sein: in einigen Fällen wird Xmp.exif.UserComment gegenüber Exif.Photo.UserComment bevorzugt. Der Grund dafür ist nicht klar.

Beim Schreiben füllt der Windows Explorer nur Exif.Image.XPComment aus und löscht die anderen aufgelisteten Tags.

### Autoren

| Tag-Name | Beschreibung|
|:---|:---|
| Exif.Image.Artist | This tag records name of the main person who created the image. The detailed format is not specified. When the field is left blank, it is treated as unknown.|
| Iptc.Application2.Byline | Name of the creator of the image. Where the artist cannot or should not be identified, the name of a company or organisation may be use.|
| Xmp.dc.creator | DCMI definition: An entity primarily responsible for making the resource.<br>DCMI comment: Examples of a creator include a person, an organization, or a service. Typically, the name of a creator should be used to indicate the entity.<br>XMP addition: XMP usage is a list of creators. Entities should be listed in order of decreasing precedence, if such order is significant. |
| Exif.Image.XPAuthor | Nicht dokumentiert in Exif Spezifikation.<br>Beschreibung von [exiv2.org](https://exiv2.org/tags.html):<br>Author tag used by Windows, encoded in UCS2|
{:.tablestylegrey}

### Copyright

| Tag-Name | Beschreibung|
|:---|:---|
| Exif.Image.Copyright | Copyright information. It is the copyright notice of the person or organization holding rights to the image.|
| Iptc.Application2.Copyright | The Copyright Notice contains information required to assert copyright in the image and should contain the name of the current copyright holder, whether an individual or a company. The format will differ according to the relevant copyright legislation. It may include the copyright symbol ©, the year of publication, and other commonly used terms such as ‘All Rights Reserved.' If an image is Public Domain, it can be indicated here.|
| Xmp.dc.rights | DCMI definition: Information about rights held in and over the resource.<br>DCMI comment: Typically, rights information includes a statement about various property rights associated with the resource, including intellectual property rights.<br>XMP addition: XMP usage is a list of informal rights statements, given in various languages.|
{:.tablestylegrey}
