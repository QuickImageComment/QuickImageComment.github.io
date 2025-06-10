---
layout: page

title: Problembehandlung
description: Problembehandlung.

language: de
language_reference: troubleshooting

published: true
order: 3
toc: true
---

## Problembehandlung

Diese Seite enthält Probleme/Fragen und deren Lösungen/Antworten. Neue Einträge werden jeweils oben ergänzt.

### Bedienelemente sind teilweise verdeckt oder Inhalt ist abgeschnitten
Die Größe der meisten Masken kann angepasst werden. In einigen Fällen kann auch die Größe einzelner Bereiche, insbesondere in der Hauptmaske, angepasst werden. Normalerweise kann eine Maske oder ein Bereich nicht so klein gemacht werden, dass nicht mehr alle Bedienelemente Platz finden. In besonderen Fällen ist es aber möglich, einen Bereich so klein zu machen, dass sich Bedienelemente überlappen oder Inhalte abgeschnitten sind, damit in einem anderen, wichtigeren Bereich mehr Platz zur Verfügung steht.

Abhilfe: Masken können mit der linken Maustaste an den Rändern vergrößert werden. Teilbereiche, deren Größe innerhalb einer Maske verändert werden kann, können durch Ziehen der grauen Trennlinien vergrößert werden.

### Texte in den Masken sind nicht übersetzt
Wenn Beschriftungen oder Meldungen nicht übersetzt sind, bitte eine Information an <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a> senden. Dann ist der entsprechende Text leider bei der Übersetzung übersehen worden.

Wenn Beschreibungen von Feldern nicht übersetzt sind, kann das zwei Gründe haben. 

Die Übersetzung der Feld-Beschreibungen ist sehr aufwändig und in manchen Fällen ist die englische Original-Beschreibung unklar, sodass diese bisher noch nicht übersetzt wurde. In Französisch sind noch keine Feld-Beschreibungen übersetzt. Auch hier bitte eine Info an <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a>, damit man sich um eine Übersetzung bemühen kann. 

Wenn das Programm zum ersten Mal gestartet wird, wird eine initiale Konfiguration erstellt, die für verschiedene Bereiche (z.B. "Übersicht") definiert, welche Felder angezeigt werden. Dabei werden die Beschreibungen entsprechend der gewählten Sprache genommen. Wenn später die Sprache geändert wird, werden diese Felder und deren Beschreibungen nicht mehr geändert, weil sie - abgesehen von der initialen Befüllung - nicht vom Programm sondern vom Anwender verändert werden.

Um Feld-Beschreibungen in der gewünschten Sprache zu erhalten, gibt es mehrere Möglichkeiten:

* Gilt nur für Deutsch: Wenn man selbst noch keine und nur sehr wenige Konfigurationsänderungen vorgenommen hat, ist es am einfachsten, die bestehende Konfigurationsdatei (QuickImageComment.ini oder QuickImageCommentX64.ini in<br>C:\Benutzer\{Benutzername}\AppData\Roaming)<br>zu löschen und das Programm neu mit der gewünschten Sprach zu starten. 
* Gilt nur für Deutsch: Wenn man schon Konfigurationsänderungen vorgenommen hat und mit einem Textvergleichstool wie z.B. WinDiff oder WinMerge vertraut ist, sollte man die bestehende Konfigurationsdatei umbenennen. Anschließend startet man das Programm neu mit der gewünschten Sprache und vergleicht die alte mit der neuen Konfigurationsdatei. Die Zeilen, die mit "MetaDataDefFor..." beginnen, enthalten die Beschreibungen, die in den Masken angezeigt werden. Diese Zeilen übernimmt man von der neu erzeugten Datei, weil die Beschreibungen dort in der gewünschten Sprache vorliegen. Alle anderen Zeilen übernimmt man aus der umbenannten Datei und behält damit die eigenen Konfigurationsänderungen.
* Die Beschreibungen kann man selbst in der Maske "Felddefinitionen" (Menü: Extras - Felddefinitionen) ändern. Das ist allerdings etwas Arbeit.

### Suche nach einem Ort in Kartenansicht liefert kein Ergebnis
Sofern die Suchbegriffe richtig geschrieben wurden, konnte der entsprechende Ort vermutlich von Nominatim nicht gefunden werden. Um dies zu verfizieren, kann die Abfrage auf der [Nominatim Testseite](https://nominatim.openstreetmap.org/ui/search.html) wiederholt werden. Falls dort ein Ergebnis geliefert wird, bitte eine Info mit der Abfrage an <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a>, damit das Problem innerhalb von QuickImageComment gelöst werden kann.

### Im Reiter "Übersicht" der Hauptmaske ist ein roter Balken
Im Reiter "Übersicht" zeigt ein roter Balken links an, dass es Auffälligkeiten oder Fehler bei den Eigenschaften gibt. Diese werden unten in dem Reiter angezeigt. Auffälligkeiten können sein:
* Für bestimmte Eigenschaften, für die es nur einen Wert geben sollte, gibt es mehrere Werte im Bild.
* Die verschiedenen Eigenschaften (Exif, IPTC, XMP), die in der Maske "Einstellungen" ausgewählt wurden, um darin Künstler (Autor) und Kommentar zu speichern, haben unterschiedliche Werte.

Fehler können beim Lesen der Eigenschaften durch die Bibliothek exiv2 gemeldet werden, z.B. "The memory contains data of an unknown image type".

Fehler können auch bei der Anzeige des Bildes auftreten. Wenn neben "Fehler Bildanzeige" eine Meldung beginnend mit "BitmapDecoder:" oder "LibRaw:" angezeigt wird, fehlt ein Codec für das Einlesen des RAW-Bildes und sollte installiert werden. Als Alternative kann die Microsoft Raw Image Extension installiert werden, die verschiedene RAW-Formate unterstützt. Andere Meldungen deuten auf einen Softwarefehler und sollten an <a href="mailto:quickimagecomment@gmail.com">quickimagecomment@gmail.com</a> gemeldet werden.
