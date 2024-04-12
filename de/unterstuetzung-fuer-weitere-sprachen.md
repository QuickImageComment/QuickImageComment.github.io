---
layout: page

title: Unterstützung für weitere Sprachen
description: Unterstützung für weitere Sprachen.

language: de
language_reference: support-for-additional-languages

published: true
order: 7
---

# Unterstützung für weitere Sprachen

Neue Sprachen können grundsätzlich ohne Programmänderungen unterstützt werden, wenn entsprechende Sprachdateien erstellt werden. Programmänderungen sind nur dann notwendig, wenn es nicht möglich ist, die Übersetzungen so kurz zu halten, dass sie in den verfügbaren Platz passen.

Im Folgenden wird erläutert, wie Sprachdateien für weitere Sprachen erstellt werden - in der Hoffnung, dass jemand bereit ist, die dafür notwendige Übersetzungsarbeit auf sich zu nehmen, ggfs. mit Hilfe von [https://translate.google.com](https://translate.google.com) oder [https://www.deepl.com/translator](https://www.deepl.com/translator).

Es ist sinnvoll, quickimagecomment@gmail.com zu informieren, wenn man mit einer Übersetzung beginnt. Falls sich mehrere Freiwillige für eine Sprache melden, kann das koordiniert und doppelte Arbeit vermieden werden. Alle Dateien, die Basis für die Übersetzung sind, sind im GitHub-Repository zu finden:
[https://github.com/QuickImageComment/QuickImageComment](https://github.com/QuickImageComment/QuickImageComment)

Die Unterstützung für weitere Sprache teilt sich in drei Bereiche auf, die nachfolgend beschrieben werden. Am wichtigsten wäre die Übersetzung der Maskentexte und Meldungen.

### Übersetzungen für die Maskentexte und Meldungen

Für diese Übersetzungen wird folgende Excel-Datei verwendet:<br>
[Translation_QIC.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_QIC.xlsm)

Die Datei enthält etwa 700 Einträge mit zusammen rund 3000 Worten. Das sind viele Übersetzungen, aber die Texte sollten sich recht einfach übersetzen lassen. In der Datei sind die Texte in Deutsch und Englisch enthalten. Für eine dritte Sprache ist Platz vorgesehen, für weitere Sprachen kann bei Bedarf Platz geschaffen werden. Detaillierte Hinweise sind in der Excel-Datei im Blatt "Anleitung-Instructions".

### Übersetzungen für Tag-Namen und zugehörigen Beschreibungen

Für diese Übersetzungen wird je Sprache eine eigene Excel-Datei verwendet:<br>
[Translation_Tags_Deutsch.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_Deutsch.xlsm)<br>
[Translation_Tags_French.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_French.xlsm) (bisher nur rudimentär gefüllt)<br>
[Translation_Tags_Spanish.xlsm](https://github.com/QuickImageComment/QuickImageComment/blob/main/Translation/Translation_Tags_Spanish.xlsm) (bisher nur rudimentär gefülltbr)

Basis sind die englischen Tag-Namen und Beschreibungen aus exiv2. Dazu kommen einige wenige Einträge für Tags, die intern in QuickImageComment definiert werden. exiv2 kennt etwa 3500 Tags, davon einige Wiederholungen. Bespielsweise taucht FNumber unter anderen als Exif.Image.FNumber, Exif.MinoltaCs5D.FNumber, Exif.MinoltaCs7D.FNumber und
Exif.MinoltaCsNew.FNumber auf. Ohne Wiederholungen sind es immer noch rund 2200 Einträge.

Einige Beschreibungen wurden im Rahmen des exiv2-Projekts für viele Sprachen übersetzt. Diese Übersetzungen sind in den Dateien für Spanisch und Französisch enthalten. Wenn jemand eine andere Sprache übersetzen möchte: Bitte Mail an mail@quickimagecomment.de, dann wird eine entsprechende Datei bereit gestellt.

Während die Maskentexte und Meldungen vollständig übersetzt werden sollten, besteht hier keinerlei Anspruch auf Vollständigkeit, zumal einige Tags eine sehr spezifische Bedeutung haben (z.B. "Der vollständige wissenschaftliche Name der Gattung, in der das Taxon klassifiziert wurde."). Außerdem gibt es einige Tags, deren Bedeutungen schwer verständlich und daher entsprechend schwer zu übersetzen sind.

Detaillierte Hinweise sind in der Excel-Datei im Blatt "Anleitung-Instructions".

### Übersetzung der Benutzeranleitung

Am meisten Arbeit dürfte die Übersetzung der Benutzeranleitung machen. Sie umfasst rund 80 Seiten. Dazu kommen zwar noch etliche Seiten mit Lizenzbedingungen, die aber nicht übersetzt werden müssen, weil die englische Variante juristisch bindend ist. Für die GPL ist in der Benutzeranleitung eine nicht rechtskräftige deutsche Übersetzung enthalten. Für andere Sprache ist - wenn man möchte - sicherlich auch eine Übersetzung im Internet zu finden.

Grundlage für die Übersetzung sind die Worddokumente der Benutzeranleitungen:<br>
[QIC_Benutzeranleitung.docm](https://github.com/QuickImageComment/QuickImageComment/blob/main/UserManual/QIC_Benutzeranleitung.docm) (Deutsch)<br>
[QIC_User_Manual.docm](https://github.com/QuickImageComment/QuickImageComment/blob/main/UserManual/QIC_User_Manual.docm) (Englisch)

Die anderen Formate (PDF, HTML und CHM) werden daraus generiert.

 