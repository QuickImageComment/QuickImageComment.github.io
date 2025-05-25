---
layout: page

title: Änderungshistorie
description: Änderungshistorie.

language: de
language_reference: change-history

published: true
order: 7
---

# Änderungshistorie

## Version 4.66 veröffentlicht am 28.03.2025

Erweiterungen und Verbesserungen:

* Trennlinie erlaubt Anpassung der Breite der Auswahlliste für Karten-Quelle und Ankreuzfeld darunter. Dadurch kann mehr Platz für die Felder links geschaffen werden, die öfter verwendet werden.
* Neuer Menüeintrag unter "Bild" zum unwiderruflichen Löschen.
* Mit gedrückter Umschalttaste wird mit der Löschtaste unwiderruflich gelöscht.
* In der Maske "Einstellungen" kann konfiguriert werden, dass mit der Löschtaste auch ohne Umschalttaste unwiderruflich gelöscht wird.
* In den Reitern Übersicht/Exif/IPTC/XMP/Sonstige ist das Kontextmenü um "Kopieren" erweitert.

Folgende Fehler wurden behoben:

* Im Reiter "Sonstige" konnten Änderungen für "Image (Bild).Kommentar" nicht gespeichert werden.
* Der Längengrad von Orten auf oder westlich von 100°W wurde nicht im Koordinatenfeld unter der Karte angezeigt.

## Version 4.65 veröffentlicht am 16.02.2025

Erweiterungen und Verbesserungen:

* Nur für die .Net 4.6.1-Varianten: Neue Version 0.28.4 der Bibliothek exiv2 integriert: Erkennung von mehr Objektiven, kleinere Fehler behoben.

Folgende Fehler wurden behoben:

* Die Suche nach einem Ort (z.B. Paris) in der Kartenansicht funktionierte nicht mehr, weil die Syntax für die Abfrage geändert wurde.
* Die Angabe eines Verzeichnisses in der Kommandozeile führte immer zur Fehlermeldung "Verzeichnis/Datei nicht gefunden".

## Version 4.64 veröffentlicht am 09.02.2025

Neu: Sprachdatei für Französisch. Dank an Régis für Erstellung der Übersetzung.
Hinweis an dieser Stelle: Neue Sprachen können grundsätzlich ohne Programmänderungen ergänzt werden, wenn eine entsprechende Sprachdatei erzeugt wird. Unterstützung dafür ist sehr willkommen. Weitere Hinweise unter www.quickimagecomment.de.

Die Übermittlung von Fehlerberichten und elementarer anonymer Nutzungsdaten mit Hilfe des Microsoft AppCenters wurde entfernt, weil AppCenter am 31. März 2025 von Microsoft eingestellt wird.

## Version 4.63 veröffentlicht am 26.12.2024

Erweiterungen und Verbesserungen:

* Anzeige von Aufnahmerichtung und -winkel in Karte.
* Neue Version 0.21.3 der Bibliothek LibRaw integriert, die 4-Komponenten JPEG-komprimierte DNG-Dateien unterstützt.
* Im Parameter FindDataTableFileName (Dateiname zum Speichern der für die Suche gelesenen Daten) kann auch ein absoluter Pfad angegeben werden. Bisher konnte die Datei nur im Speicherort für Benutzer-Einstellungen abgelegt werden.
* In Ansicht "Liste" bzw. Miniaturansicht wird mit Cursor unten/oben bzw. rechts/links über die Grenze der Zeile bzw. Spalte weiternavigiert.

Folgende Fehler wurden behoben:

* Das Anlegen von benutzerdefinierten Schaltflächen war abhängig von den Konfigurationseinstellungen häufig nicht möglich.

## Version 4.62 veröffentlicht am 15.10.2024

Folgende Fehler wurden behoben:

* Wenn das Programm mit Kartenansicht gestartet wurde und WebView2 aktiviert war, stürzte es ab.
* Wenn Kartenansicht mit WebView2 aktiv war, wurde beim Bildwechsel angezeigt, dass der Aufnahmeort geändert wurde, obwohl das nicht der Fall war.

## Version 4.61 veröffentlicht am 06.10.2024

Folgende Fehler wurden behoben:

* Das Programm stürzte ab, wenn versucht wurde, einen leeren Wert in den Reitern für Eigenschaften zu speichern. 
* Das Programm konnte beim Start mit "Invoke oder BeginInvoke kann nicht auf einem Steuerelement aufgerufen werden, bis die Fensterverknüpfung erstellt ist." abstürzen. 
* In seltenen Fällen konnte das Programm beim Wechsel der Ansicht der Dateiliste abstürzen.
 
## Version 4.60 veröffentlicht am 26.09.2024

Erweiterungen und Verbesserungen:

* Bilder können in einen anderen Ordner kopiert oder verschoben werden.
* Maske "Konfiguration Bearbeiten-extern": Programm-Pfad und Fenstertitel können von geöffneten Programmen übernommen werden, d.h. diese Daten müssen nicht manuell eingegeben werden.
* Vor dem Speichern wird geprüft, ob die Datei seit dem Lesen außerhalb des Programmes verändert wurde.
* Wenn ein Bild außerhalb des Programmes verändert wird, wird jetzt das angezeigte Bild auch dann aktualisiert, wenn nicht gespeicherte Änderungen vorliegen. Die vorgenommenen Änderungen werden nicht überschrieben, auch wenn die entsprechenden Felder außerhalb verändert wurden.
* Maske "Benutzerdefinierte Schaltflächen": Icons von einer Datei können zugewiesen werden. Handelt es sich bei dem Menüpunkt um einen Eintrag aus "Bearbeiten-Extern" mit der Konfiguration "Programm", kann das dem Programm zugeordnete Icon zugewiesen werden.

Folgender Fehler wurde behoben:

* Bei Eingabe in den Reitern für Eigenschaften: Mit der Escape-Taste wurde nicht der Wert wiederhergestellt, der eingelesen wurde sondern der Wert, den die Zelle hatte, als sie zuletzt verlassen wurde, also ggfs. eine vorherige Eingabe war. 

## Version 4.59 veröffentlicht am 14.08.2024

Erweiterungen und Verbesserungen:

* Verbesserte Fehlererkennung
* Nur für die .Net 4.6.1-Varianten: Neue Version 0.28.3 der Bibliothek exiv2 integriert: kleinere Fehler wurden behoben.

Folgender Fehler wurde behoben:

* Das Programm stürzte ab, wenn die Größe der Vorschaubilder größer als 256x256 konfiguriert wurde.

## Version 4.58 veröffentlicht am 17.03.2024

Erweiterungen und Verbesserungen:

* Nur für die .Net 4.6.1-Varianten: Neue Version 0.28.2 der Bibliothek exiv2 integriert: Objektiverkennung erweitert und kleinere Fehler wurden behoben.

Hinweis: Wegen Geschäftsaufgabe des Hosting-Providers wird die bisherige Kontakt-E-Mail-Adresse Anfang Mai deaktiviert. Bitte ab sofort folgende Adresse verwenden: [quickimagecomment@gmail.com](mailto:quickimagecomment@gmail.com). Links im Programm und in der Hilfe sind entsprechend angepasst.

## Version 4.57 veröffentlicht am 29.12.2023

Erweiterungen und Verbesserungen:

- Für Anwender/Anwenderinnen, die über die Kommandozeile (bzw. angepasste Shortcuts) das Programm mit unterschiedlichen Konfigurationen starten: Mit dem Schalter "/TitleSuffix:" kann ein Text definiert werden, der zusätzlich im Maskentitel der Hauptmaske angezeigt wird.
- Export von ausgewählten Eigenschaften: Zeilenumbruch und Zeilenvorschub (CR/LF) in Metadaten werden durch Leerzeichen ersetzt, um Probleme beim Import in Excel zu vermeiden.
- Nur für die .Net 4.6.1-Varianten: Neue Version 0.28.1 der Bibliothek exiv2 integriert: kleinere Fehler wurden behoben.
- Nur für die .Net 4.6.1-Varianten: Neue Version 0.21.1 der Bibliothek LibRaw integriert: kleinerer Fehler beim Decoding von Bildern von einigen Panasonic-Kameras behoben.
- Metadaten von iPhone .heic-Dateien und JPEG-XL-Dateien (.jxl) werden angezeigt.

Folgende Fehler wurden behoben:

- Gelegentlich konnte das Programm blockieren, wenn im angezeigten Ordner Dateien von anderen Programmen hinzugefügt, geändert oder gelöscht wurden.
- Wenn Dateien gelöscht wurden, wurde der Dateizähler unten links nicht aktualisiert.
- Wenn bei der ersten Benutzung des Programmes (d.h. noch keine Konfigurationsdatei gespeichert) ein Ordner geöffnet wurde, der Bilder mit IPTC-Schlüsselworten enthielt, stürzte das Programm ab.
- Verzeichnisbaum aktualisieren unter Windows 11 verursachte Absturz. Unter anderen Windows-Versionen war die Aktualisierung unvollständig, wenn es mehrere Ordner mit dem gleichen Namen gab.

## Version 4.56 veröffentlicht am 04.09.2023

Erweiterungen und Verbesserungen:

- Laufende Nummer des Bildes wird unter dem Bild links vom Dateinamen angezeigt.
- Neue interne Felder "Image (Bild).Meta-Daten Warnungen-Exiv2" und "Image (Bild).Meta-Daten Warnungen-nicht-Exiv2". Die Felder erlauben es nach Bildern mit entsprechenden Meldungen zu suchen – getrennt danach, ob die Meldung von Exiv2 oder nicht kommt. Da bei der Suche die Meta-Daten nicht vollständig gelesen werden, können die Warnungen unvollständig sein.
- Im Textfeld für die Abfrage in der Maske "Suche über Eigenschaften - Abfrage bearbeiten" können manuelle Änderungen mit Strg-Z rückgängig und mit Strg-Y wieder hergestellt werden. Es werden jeweils alle Änderungen seit dem Füllen des Textfeldes (bei Öffnen der Maske oder bei Betätigen von "Vorherige" oder "Nächste") rückgängig gemacht.

Folgender Fehler wurde behoben:

- Mit jedem Neustart wurde die Maske kleiner, wenn Skalierung für Symbolleiste auf einen anderen Wert als für die allgemeine Skalierung eingestellt war.
- Bei Änderung der Skalierung im Vollbildmodus konnte rechts und unten ein Teil der Maske abgeschnitten werden.
- Nur Variante für Windows XP: Absturz beim Speichern von Änderungen in JPEG-Dateien.

## Version 4.55 veröffentlicht am 02.06.2023

Erweiterungen und Verbesserungen:

- Neu in Maske "Bild in eigenem Fenster": Blättern der Bilder mit Tastatur oder Maus; Anzeige von Meta-Daten in Titelleiste (konfigurierbar).
- Maske "Vordefinierte IPTC Schlüsselworte": Durch Einrücken kann eine Hierarchie der Schlüsselworte definiert werden. Dadurch können im Baum des Bereiches "IPTC Schlüsselworte" Teile auf- und zugeklappt werden, was die Auswahl der Schlüsselworte erleichtert.
- Optional kann ein Hinweis angezeigt werden, wenn einem Bild ein nicht vordefiniertes Schlüsselwort zugewiesen wurde. Nach solchen Bildern kann auch gesucht werden. Damit soll eine konsistente Verschlagwortung erleichtert werden.
- Suche über Eigenschaften: Wenn die Option "Daten bei Beenden speichern" aktiviert ist, beginnt die Aktualisierung der Daten jetzt bei Start des Programmes, nicht erst beim ersten Öffnen der Suchmaske. Damit stehen die aktualisierten Daten früher zur Verfügung.
- Suche über Eigenschaften: Wenn IPTC-Schlüsselworte als Suchfeld definiert ist, wird rechts im unteren Bereich der Maske ein Baum mit den vordefinierten Schlüsselworten angezeigt. Schlüsselworte, nach denen gesucht werden soll, können hier angekreuzt werden.
- Suche über Eigenschaften: Einige Felder können mehrere Werte haben, z.B. IPTC-Schlüsselworte. Für die Suche werden diese Werte zu einer Zeichenkette zusammengefasst, wobei die Reihenfolge nicht definiert ist. Daher sind für diese Felder die Vergleichsoperatoren entfernt worden, bei denen die Reihenfolge der Einzelwerte wichtig ist.
- Suche über Eigenschaften: auch der zweite Operator kann nun "<>", "enthält", "enthält nicht", "beginnt nicht mit" oder "endet nicht mit" sein.
- Suche über Eigenschaften: In einer zusätzlichen Maske kann die Abfrage in einer SQL-ähnlichen Syntax bearbeitet werden. Damit sind komplexere Abfragen möglich. Außerdem kann eine zuvor ausgeführte Abfrage ausgewählt werden um sie zu anzupassen und erneut auszuführen.
- Nur für die .Net 4.6.1-Varianten: Neue Version 0.28.0 der Bibliothek exiv2 integriert: einige neue Tags und Objektivdaten; für ExifEasy werden weitere Exif-Eigenschaften berücksichtigt, sodass nun ExifEasy-Eigenschaften von einigen Bilder gefüllt sind, die in der vorherigen Version noch leer waren.  
    Da exiv2 0.28.0 nicht mehr unter Windows XP lauffähig ist, wird die Variante für Windows XP weiterhin mit exiv2 0.27.5.1 ausgeliefert.

Folgender Fehler wurde behoben:

- Bei Wechsel von "einschl. Karten nur für Anzeige (\* ...)" wurde die Auswahlliste falsch gefüllt, Auswahl am Ende der Liste führte zu Programmabsturz.

## Version 4.54 veröffentlicht am 02.05.2023

Erweiterungen und Verbesserungen:

- Neue Maske "Skalierung": Die Vergrößerung aller Masken kann eingestellt werden; separate Skalierung für Symbolleiste und Miniaturansicht/Kacheln. Der Zoom-Faktor in Maske "Maske anpassen" kann weiterhin verwendet werden, um einzelne Masken zu skalieren. Maskenspezifische Zoom-Faktoren können in "Maske anpassen" deaktiviert werden, indem einmalig der Faktor auf den generellen Skalierungsfaktor gesetzt wird.
- Einige Eigenschaften können auch in den Reitern "Übersicht", "Exif" und "IPTC" geändert werden. Änderbare Werte werden mit weißem Hintergrund angezeigt, nicht-änderbare mit hellgrauem Hintergrund. Details in der Hilfe, Kapitel 3.6, Unterabschnitt "Eingabe in den Reitern für Eigenschaften".
- Veränderte Werte für Künstler, Kommentar und IPTC-Schlüsselworte sowie im konfigurierbaren Eingabebereich werden durch hellgelben Hintergrund kenntlich gemacht. Wird die Eingabe rückgängig gemacht, wird der Hintergrund wieder weiß. Anstatt hellgelb kann in der allgemeinen Konfigurationsdatei auch eine andere Farbe festgelegt werden.

Folgende Fehler wurden behoben:

- Beim zweiten Öffnen einer Untermaske wurde der Zoom-Faktor aus Maske "Maske anpassen" nicht berücksichtigt.
- Das Programm konnte bei "Dateidatum auf Aufnahmedatum setzen" abstürzen, wenn Aufnahmedatum außerhalb des zulässigen Bereiches für Dateidatum war.

## Version 4.53 veröffentlicht am 16.02.2023

Erweiterungen und Verbesserungen:

- Die ausgewählten Dateien können zur weiteren Bearbeitung an andere Programme oder an Windows-Batch-Skripte übergeben werden.
- Das erste Einlesen und vor allem das Aktualisieren der eingelesenen Daten für die Suche wurde beschleunigt.
- Das Menü "Datei" hat einen neuen Eintrag zur Auswahl eines Ordners. Es wird eine Maske geöffnet, in der ein Ordner in einem Verzeichnisbaum oder aus einer Auswahlliste mit zuletzt ausgewählten Ordnern ausgewählt werden kann. Auf diese Weise kann der Platz für den Verzeichnisbaum in der Hauptmaske für andere Informationen genutzt werden, z.B. für eine längere Liste von Dateien.
- Neue Felder: "Image (Bild).Fehlermeldung Bild-Anzeige" enthält Fehlermeldung bei der Anzeige des Bildes, "Image (Bild).Meta-Daten Warnungen" enthält Warnungen beim Lesen von Metadaten. Beide Informationen werden schon jetzt im Reiter Übersicht angezeigt. Die Felder erlauben es nach Bildern mit entsprechenden Meldungen zu suchen. Da bei der Suche die Meta-Daten nicht vollständig gelesen werden, können die Warnungen unvollständig sein.

Folgende Fehler wurden behoben:

- Das Programm konnte abstürzen, wenn unbekannte XMP-Tags für die Änderung von Daten ausgewählt wurden.
- Das Programm konnte abstürzen, wenn XMP-Struct-Felder (z.B. Xmp.iptcExt.LocationShown\[1\]/…) für die Suche konfiguriert wurden.

## Version 4.52 veröffentlicht am 14.01.2023

Erweiterungen und Verbesserungen:

- Variante für Net 4.6.1 und höher und wenn WebView2 Runtime installiert ist: Bei der Anzeige des Aufnahmeortes auf Karte können Karten nur für Anzeige (z.B. Google Maps und Bing Maps) ausgeblendet werden (was technisch das Deaktivieren von WebView2 bedeutet).  
    Hintergrund: Für Google Maps und Bing Maps ist WebView2 erforderlich. WebView2 verursacht aber gelegentlich Probleme. Anstatt wie bisher WebView2 über die allgemeine Konfigurationsdatei zu deaktivieren, kann man dies nun direkt in der Oberfläche.
- Im Dateifilter können nun auch Platzhalterzeichen ("?" für ein beliebiges Zeichen, "\*" für eine beliebige Anzahl von Zeichen) verwendet werden.

Folgender Fehler wurde behoben:

- Wenn die installierte Version von WebView2 nicht zu den mit dem Programm gelieferten Komponenten passte, konnte das Programm abstürzen. In solchen Fällen wird jetzt die "alte" Browserkomponente verwendet, die aber Google Maps und Bing Maps nicht unterstützt.
- Maske "Suche über Eigenschaften": Mit der Schaltfläche "Kriterien von akt. Datei" wurden die GPS-Daten des Aufnahmeortes nicht übernommen.
- Programm konnte mit "Die SplitterDistance muss zwischen Panel1MinSize und Width - Panel2MinSize liegen." abstürzen, wenn der Container mit Bild-Details sehr klein gemacht wurde.

## Version 4.51 veröffentlicht am 29.11.2022

Erweiterungen und Verbesserungen:

- In der allgemeinen Konfigurationsdatei können Karten-Quellen für Leaflet definiert werden. Mit diesen Karten ist - anders als bei den Karten für "Karte in Standard Browser" - der Aufnahmeort geändert werden.
- Bilder von JPEG-2000- (\*.jp2) und Photoshop-Dateien (\*.psd) können angezeigt werden; bisher wurden nur die Metadaten angezeigt.

Folgender Fehler wurde behoben:

- Programmabsturz mit Ausnahmefehler "ctor System.NullReferenceException: Der Objektverweis wurde nicht auf eine Objektinstanz festgelegt. ExtendedImage.cs:Zeile 287.". Gemeldet über AppCenter.

Hinweis: Version 4.51 ist auch für Windows XP 32-Bit und .Net 4.0 Framework verfügbar.

## Version 4.50 veröffentlicht am 30.10.2022

Erweiterungen und Verbesserungen:

- Bei der Anzeige von Bildern wird auch die Orientierungsinformation der herstellerspezifischen Tags berücksichtigt (bisher wurde nur Exif.Image.Orientation verwendet).
- Da einige RAW-Dekoder die Bilder gemäß Exif.Image.Orientation drehen, kann mit dem neuen Menüpunkt "Zoom/Drehen - RAW: Drehen nach Dekodierung" ausgewählt werden, ob die Drehung nach der Dekodierung angewendet werden soll oder nicht. Wird dies für ein Bild ausgewählt, gilt es für alle Bilder, die mit demselben Decoder gelesen werden.
- Über Kontextmenü können Feld-Einträge aus den Reitern "Übersicht", "Exif", "IPTC", "XMP" und "Sonstige" in die Tabelle im Reiter "Mehrfach-Bildbearbeitung" übernommen werden.
- In der Maske "Felddefinitionen" werden zusätzliche Gruppen von Exif-Tags angezeigt. Sofern sie in Bildern enthalten waren, wurden die Werte auch in der vorherigen Version angezeigt.
- Der Dateifilter wurde geändert: Dateien werden danach gefiltert, ob sie die Filterzeichenfolge enthalten, und nicht wie bisher danach, ob sie mit der Filterzeichenfolge beginnen.

Folgende Fehler wurden behoben:

- In sehr seltenen Fällen wurde der Objektivnamen falsch angezeigt.
- Die Schaltfläche "Speichern" wurde nicht aktiviert, wenn die Geodaten gelöscht wurden.
- Die Einstellungen für "Bilddetails" wurden nicht korrekt geladen, so dass ein Bereich bei jedem Neustart des Programms kleiner wurde.

Hinweis: Version 4.50 ist nur für .Net 4.6.1 (oder höher) verfügbar. Net 4.6.1 wurde bereits im November 2015 veröffentlicht und somit wird die Unterstützung für das sehr alte .Net 4.0 eingestellt.

## Version 4.49 veröffentlicht am 29.05.2022

Erweiterungen und Verbesserungen:

- Die Anzeige von RAW-Bildern wird für mehr Kameramodelle unterstützt.  
    In der Variante für .Net 4.6.1 ist LibRaw für die Anzeige von RAW-Bildern integriert. Bei Verwendung der Variante für .Net 4.0 oder wenn LibRaw das RAW-Format nicht unterstützt, muss ein Codec des Kameraherstellers installiert werden, um das Bild anzuzeigen. Als Alternative kann die Microsoft Raw Image Extension installiert werden, die verschiedene RAW-Formate unterstützt.

Folgende Fehler wurden behoben:

- Aufnahmeort auf Karte: einige Karten konnten nicht angezeigt werden, wenn WebView2 installiert war.
- Aufnahmeort auf Karte: Die Karten "HikeBike.HikeBike" und "OpenMapSurfer.Roads" sind nicht mehr frei verfügbar. Sie wurden daher aus der Auswahlliste entfernt.
- Programmabsturz "Not a valid Win32 FileTime" aufgrund von ungültigem Änderungsdatum/-zeit einer Datei. Gemeldet über AppCenter.

## Version 4.48 veröffentlicht am 29.03.2022

Erweiterungen und Verbesserungen:

- Unter Windows 10 mit Microsoft Raw Image Extension: DNG-Bilder von einigen Samsung-Modellen können jetzt angezeigt werden.

Folgende Fehler wurden behoben:

- Die Eigenschaften File.ImageSize und Image.CodecInfo waren nach dem Speichern leer.
- Das Öffnen einer Datei über Menü "Datei – Öffnen" und Eingabe einer URL funktionierte nicht.
- Programmabsturz, wenn in der Kommandozeile nicht vorhandene Datei oder Ordner angegeben waren.
- Es war nicht möglich, alle IPTC Schlüsselworte zu löschen, sondern nur alle bis auf eines.
- Programmabsturz mit Ausnahmefehler "GeneralUtilities.comboBox_Resize_Unselect (Object sender, EventArgs e) System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1544604736' no es válido para 'start'. Nombre del parámetro: start". Gemeldet über AppCenter

Hinweise:

- Für die Anzeige von RAW-Bildern muss ggfs. ein Codec des Kameraherstellers installiert werden. Als Alternative kann die Microsoft Raw Image Extension installiert werden, die verschiedene RAW-Formate unterstützt. Mit dem Codec des Kameraherstellers könnte die Anzeige aber schneller sein. Man kann einen spezifischen Codec und die Microsoft Extension installieren. Der spezifische Codec wird dann für die entsprechenden Bilder verwendet, für alle anderen die Microsoft Extension.
- Um den Einstieg in QuickImageComment zu erleichtern, gibt es jetzt Tutorials auf YouTube. Für den Zugriff gibt es einen neuen Eintrag im Hilfe-Menü. Derzeit decken fünf Videos die Grundlagen ab, weitere sollen folgen.

## Version 4.47 veröffentlicht am 09.01.2022

Erweiterungen und Verbesserungen:

- Mit der Variante für .Net 4.6.1 und höher und wenn WebView2 Runtime installiert ist: Für die Kartenanzeige kann nun auch Google-Maps oder Bing Maps verwendet werden. Hierfür werden die Links verwendet, die bisher schon für "Karte in Standard Browser" verwendet wurden. Mit diesen Links ist nur eine Anzeige möglich, die Koordinaten können nicht verändert werden.
- Neue Version 0.27.5 der Bibliothek exiv2 integriert, mit neuem Tag Exif.Photo.Gamma.

Folgende Fehler wurden behoben:

- Programmabsturz, wenn während des Entfernens von Meta-Daten das Bild von einem anderen Prozess verwendet wurde.
- Kartenansicht: Suche funktionierte nicht in der Variante für .Net4, Fehlermeldung: Could not create SSL/TLS secure channel.
- Wenn die Maske "Einstellungen" mit "Abbrechen" verlassen wurde, wurden keine Werte im konfigurierbaren Eingabebereich angezeigt.
- Die Anwendung konnte in der Kachelansicht oder der Miniaturansicht einfrieren, wenn mehrere Dateien innerhalb kurzer Zeit geändert wurden.

## Version 4.46 veröffentlicht am 22.10.2021

Erweiterungen und Verbesserungen:

- Für häufig benutzte Menüeinträge können Schaltflächen definiert werden. Selbst definierte Schaltflächen werden in der Symbolleiste angezeigt, rechts von den vordefinierten. Menüeintrag: "Extras - Benutzerdefinierte Schaltflächen".

Folgende Fehler wurden behoben:

- Verwendung von Platzhaltern scheiterte bei Feldern mit bestimmtem Format (z.B. für Datum) an der Eingabeprüfung. Werte mit Platzhalter werden nicht mehr geprüft.
- Programmabsturz, wenn Hauptmaske minimiert ist, während Änderungen in Maske "Ansicht anpassen" vorgenommen werden.
- Programmabsturz mit Ausnahmefehler "System.ArgumentNullException: Der Schlüssel darf nicht NULL sein. Parametername: key".

## Version 4.45 veröffentlicht am 09.10.2021

Erweiterungen und Verbesserungen:

- Die Dateien können über das Menü "Ansicht", über das Kontextmenü in der Dateiliste oder durch klicken in die Überschriften in der Ansicht "Details" aufsteigend oder absteigend nach Namen, Größe, Geändert oder Erstellt sortiert werden.

Folgende Fehler wurden behoben:

- Konfigurierbarer Eingabebereich: Datumsänderungen über Kalender (Schaltfläche recht neben Eingabefeld) funktionierte nicht.
- Mehrfach-Bildbearbeitung: angezeigte Datei wurde nicht markiert, keine Aktualisierung, wenn Dateien außerhalb QuickImageComment verändert wurden.
- Die Einstellungen für "IPTC Schlüsselworte" wurden nicht korrekt geladen, so dass das Feld für freie Eingabe von Schlüsselworten unsichtbar werden konnte.
- Nach Umbenennen wurden umbenannten Dateien in Dateiliste doppelt angezeigt.

## Version 4.44 veröffentlicht am 08.07.2021

Erweiterungen und Verbesserungen:

- Wenn für die Dateiliste die Ansicht "Miniaturansicht" oder "Kacheln" ausgewählt war, wurden bisher erst alle anzuzeigenden Bilder mit deren Vorschaubildern geladen, bevor eine Nutzereingabe akzeptiert wurde. Speziell bei RAW-Bildern konnte das lange dauern. Jetzt werden die Bilder zuerst mit Dateinamen aufgelistet wodurch Nutzereingaben schneller akzeptiert werden. Die Vorschaubilder werden im Hintergrund nachgeladen.
- Anzeige von RAW-Bildern von einigen Nikon-Modellen beschleunigt.
- Neue Version 0.27.4 der Bibliothek exiv2 integriert, unterstützt DNG 1.6 und Exif 2.32 (etwa 150 neue Tags).
- Platzhalter: für Datum/Zeit-Eigenschaften kann das Format ausgewählt werden. Neues Datum/Zeit-Format: Exif.

Folgender Fehler wurde behoben:

- Programmabsturz mit Ausnahmefehler "System.NullReferenceException: Referencia a objeto no establecida como instancia de un objeto.". Gemeldet über AppCenter.

Hinweis:

- Für diejenigen, die die allgemeine Konfigurationsdatei geändert haben: der (undokumentierte) Parameter DisplayFullSizeImageCacheContent wurde entfernt.

## Version 4.43 veröffentlicht am 01.06.2021

Erweiterungen und Verbesserungen:

- Die in der Maske "Ansicht anpassen" mit Namen gespeicherten benutzerdefinierten Einstellungen können direkt im Menü "Ansicht" ausgewählt werden.
- Aufnahmeort auf Karte: die Einträge der letzten verwendeten Positionen können umbenannt werden. Damit können gespeicherte Orte, die zunächst nur mit Koordinaten gelistet werden, mit einem sprechenden Namen versehen werden. Nicht mehr benötigte Einträge können gelöscht werden.

Folgender Fehler wurde behoben:

- Programmabsturz, wenn die letzte Datei in einem Ordner gelöscht wurde.

Hinweis:

- Die allgemeine Konfigurationsdatei sowie andere Konfigurationsdateien liegen jetzt nicht mehr im Programmverzeichnis selbst sondern in einem Unterordner "config". Der Namen der allgemeinen Konfigurationsdatei für 32-Bit und 64-Bit ist jetzt identisch. Dieser Hinweis ist nur wichtig, falls man diese Dateien selbst anpassen möchte.

## Version 4.42 veröffentlicht am 11.05.2021

Folgender Fehler wurde behoben:

- Schwerwiegender Fehler beim Caching: Je nach Einstellungen und Ordnerinhalt konnte das Caching zu 100% CPU-Last führen.

## Version 4.41 veröffentlicht am 08.05.2021

Erweiterungen und Verbesserungen:

- Suche über Eigenschaften: Daten können in einer XML-Datei gespeichert werden und beim nächsten Programmstart geladen werden. Dies kann viel Zeit für die Vorbereitung der Suche sparen.
- Anstatt nur einem Bild/Video können nun mehrere Bilder/Videos gleichzeitig per Drag-and-Drop übergeben werden.
- Neuer Menüeintrag "Hilfe - GitHub": Direkter Zugriff auf das neu angelegte GitHub Repository mit Quellcode, Issues (Fehlermeldungen, Feature-Anfragen) und Diskussionen.
- Sofern eine Masken-bezogene Hilfe vorhanden ist, kann diese mit F1 geöffnet werden.
- F11 ist der Funktion "Bild speichern und vorheriges Bild anzeigen" zugeordnet. Wenn diese Zuordnung gelöscht wird (siehe Maske "Maske anpassen", Tastaturkürzel), schaltet F11 nun den Ansichtsmodus zwischen normal und maximiert um.
- Keine direkte Auswirkung für Anwender, aber erwähnt um Transparenz zu gewährleisten: Um die Analyse von Abstürzen zu erleichtern, die über Appcenter.ms gemeldet werden, werden die Ereignisse "Initialisierung beendet", "Beginn Schließens des Programmes = Sichern der Konfiguration" und "Ende Schließens des Programmes" in Appcenter.ms protokolliert.

Folgende Fehler wurden behoben:

- Programmabsturz, wenn eine Datei zwischen dem Füllen der Dateiliste aus der Suchmaske und dem Doppelklick auf diesen Eintrag gelöscht wurde.
- Programmabsturz beim Starten des Programms in englischer Sprache, wenn die Symbolleiste auf "Hide - symbols in menu" eingestellt ist.
- Programmabsturz mit Ausnahmefehler "System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1' no es válido para 'startIndex'. Nombre del parámetro: startIndex". Gemeldet über AppCenter; ähnlich einem Fehler der in 4.40 an anderer Stelle behoben wurde; die eigentliche Ursache ist diesmal hoffentlich gefunden worden.
- Bilder, die mit Nikon NEF Codec 1.31.1 geladen wurden, wurden mit falschen Farben angezeigt.

## Version 4.40 veröffentlicht am 25.02.2021

Folgende Fehler wurden behoben:

- Programmabsturz mit Ausnahmefehler "System.ArgumentOutOfRangeException: InvalidArgument=Value mit dem Wert -1 ist für startIndex ungültig. Parametername: startIndex" bzw. "System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1' no es válido para 'startIndex'. Nombre del parámetro: startIndex". Gemeldet über AppCenter; unklar, welche Aktivitäten dazu geführt haben.
- Programmabsturz mit Ausnahmefehler "System.NotImplementedException: No se puede implementar el método o la operación.". Gemeldet über AppCenter. Grund muss eine Benachrichtigung über eine Änderung im Dateisystem gewesen sein, die für QuickImageComment nicht relevant war und daher wird diese Art der Benachrichtigung in Zukunft ignoriert.
- Programmabsturz wenn Programm minimiert und anschließend beendet wurde.
- Programmabsturz mit Ausnahmefehler "System.IO.FileNotFoundException: No se pudo encontrar el archivo '....tif'.". Gemeldet über AppCenter. Ursache ist vermutlich, dass eine Datei zwischen Füllen der Dateiliste in der Hauptmaske und dem Auswählen gelöscht wurde.

## Version 4.39 veröffentlicht am 13.02.2021

Erweiterungen und Verbesserungen:

- Bilder/Videos können über Position auf Karte mit Umkreis gesucht werden.
- Kartenansicht: Position kann über Koordinaten (Grad in Dezimalangabe oder mit Grad/Minute/Sekunde) eingegeben werden.
- Neue Felder "Image (Bild).GPS Breite mit Vorzeichen" (Image.GPSsignedLatitude, negative Werte für Süd) und "Image (Bild).GPS Länge mit Vorzeichen" (Image.GPSsignedLongitude, negative Werte für West), primär für Suche nach Bildern über Position.
- Wenn eine Datei ausgewählt wird, die schreibgeschützt oder auf die generell kein Zugriff erlaubt ist, werden die Bedienelemente zum Ändern von Daten gesperrt. In der Fußzeile erscheint ein Hinweis "schreibgeschützt" bzw. "kein Zugriff".
- Die maximale Anzahl der GPS-Positionen, die für die Suchliste der Karten-Anzeige gespeichert werden, gilt nun jeweils getrennt für unbenannte Einträge, die durch Markieren auf der Karte entstanden sind, und für benannte Einträge, die Ergebnis einer Suche sind (erkennbar an einem sprechenden Namen wie z.B. "Düsseldorf Hbf"). Damit soll verhindert werden, dass neue unbenannte Einträge nach und nach benannte Einträge aus der Liste verdrängen.

Folgende Fehler wurden behoben:

- Programmabsturz bei Suche, wenn ein Bild zwischen Dateneinlesen und Start der Suche gelöscht wurde.
- Programmabsturz, wenn ein leerer Ordner ausgewählt, eine Position in der Karte ausgewählt und anschließend der Ordner gewechselt wurde.
- Programmabsturz ohne Meldung beim Öffnen eines Bildes mit Tag vom Typ XmpSeq der Länge Null.
- Programmabsturz beim Versuch eine schreibgeschützte Datei zu speichern.
- Programmabsturz beim Versuch den Kalender im konfigurierbaren Eingabebereich zu öffnen, wenn das zugehörige Eingabefeld leer war.
- Programmabsturz bei Wechsel der Einstellungs-Konfiguration in Maske "Ansicht anpassen".
- Wenn kein Zugriff auf eine Datei möglich war, wurden die Exif/IPTC/XMP-Daten der zuvor gelesenen Datei angezeigt.

## Version 4.38 veröffentlicht am 21.01.2021

Erweiterungen und Verbesserungen:

- Programm startet schneller.
- Exportdateien und Benutzerkonfiguration werden mit der Kodierung UTF-8 (einschließlich Byte Order Mark) geschrieben. Alte Konfigurationsdateien können weiterhin gelesen werden.
- Neuer Menüeintrag in Hauptmaske: Hilfe - Webseite - Änderungshistorie.
- Datum in der Maske "Auf neue Version prüfen" wird im Format angezeigt, das in den Windows-Systemeinstellungen definiert ist. Zusätzlich werden die Tage seit letzter Prüfung angezeigt.

Folgende Fehler wurden behoben:

- Die Fehlerberichte, die mit Hilfe des Microsoft AppCenters übermittelt wurden, enthielten nicht die vollständige Aufrufhierarchie (Stack-Trace). Daher konnten gemeldete Fehler nicht beseitigt werden.

## Version 4.37 veröffentlicht am 30.11.2020

Erweiterungen und Verbesserungen:

- Bilder/Videos können über ihre Eigenschaften gesucht werden.
- Maske "Bild in eigenem Fenster" wird bei Mehrfachauswahl für jedes in der Hauptmaske ausgewählte Bild geöffnet und enthält eine konfigurierbare Tabelle mit Eigenschaften.
- Neue Felder "Image (Bild).Künstler kombiniert" (Image.ArtistCombinedFields) und "Image (Bild).Kommentar kombiniert" (Image.CommentCombinedFields) beinhalten die Werte von verschiedenen Feldern für Künstler bzw. Kommentar um einfacher danach suchen zu können.
- Nur für Windows 10 mit .Net 4.6.1: Mit Hilfe des Microsoft AppCenters können Fehlerberichte von Programm-Abstürzen und elementare anonyme Nutzungsdaten an den Entwickler übermittelt werden. Abstürze können so leicht gemeldet werden. Der Entwickler erhält Informationen, die bei der Weiterentwicklung helfen können.
- Separate Zip-Dateien mit Programmvarianten (32 und 64 Bit) für ältere Betriebssysteme mit .NET 4.0 verfügbar.

Folgende Fehler wurden behoben:

- Einträge im Kontextmenü auf Ebene 2 und Tooltip-Texte wurden nicht übersetzt.
- Tag-Namen und -Beschreibungen wurden nicht übersetzt, wenn das Programm in Deutsch gestartet wurde.
- Reiter "Mehrfach-Bildbearbeitung": Wenn die Hauptmaske klein war, waren die Ankreuzfelder für änderbare Eigenschaften nicht sichtbar.
- Der noch verfügbare Speicher zum Puffern von Bildern wurde falsch ermittelt, sodass weniger Bilder gepuffert wurden als möglich gewesen wäre – was ggfs. den Bildwechsel langsamer gemacht hat.

## Version 4.36 veröffentlicht am 26.08.2020

Erweiterungen und Verbesserungen:

- Anzeige des Arbeitsspeichers ist geändert in "Physikalischer Speicher, der von aktiven Prozessen verwendet wird". Dies ist der Wert, der üblicherweise im Taskmanager angezeigt wird.
- Überarbeitung der Ordner-Ansicht: Beinhaltet nun auch andere Geräte im Netzwerk (bisher nur Netzwerkadressen).
- Ordner- und Datei-Ansicht werden aktualisiert, wenn Ordner oder Dateien außerhalb des Programmes hinzugefügt, geändert oder gelöscht werden. Es erfolgt keine Aktualisierung, wenn Dateien außerhalb geändert werden, die im Programm ausgewählt sind und noch nicht gespeicherte Änderungen haben.
- In den Eigenschaften-Tabellen wird eine Änderung der Breite der Spalte "Wert" bei der Anzeige des nächsten Bildes berücksichtigt. Bisher wurde die Breite immer abhängig vom längsten Eintrag neu festgelegt, wobei eine feste maximale Breite nicht überschritten wurde.
- Neuer Eintrag im Menü "Extras" um eine Karte im Standard-Browser anzuzeigen. Dies ermöglicht die Anzeige von Google-Maps, was von der eingebauten Browser-Komponente nicht unterstützt wird. In der allgemeinen Konfigurationsdatei sind die URLs für diese Anzeige hinterlegt und können dort geändert oder ergänzt werden. Hinweis: Eine Änderung der GPS-Daten ist hier nicht möglich.
- Exif- und IPTC-Daten werden in UTF8 gespeichert, was im Allgemeinen besser durch andere Programme zur Anzeige von Metadaten unterstützt wird. In der Maske "Einstellungen" kann dies abgeschaltet werden, sodass die Daten wie mit den früheren Versionen gespeichert werden.
- Exif.Photo.UserComment wird mit charset=Unicode geschrieben, was im Allgemeinen besser durch andere Programme zur Anzeige von Metadaten unterstützt wird. In der Maske "Einstellungen" kann dies auf Ascii geändert werden, sodass die Daten wie mit den früheren Versionen gespeichert werden.
- Beim Lesen von Exif- und IPTC-Daten wird erkannt, ob sie in UTF8 kodiert sind und werden ggfs. umgewandelt. Dadurch ist es unwahrscheinlicher, dass Daten von anderen Programmen nicht korrekt angezeigt werden, wenn sie spezielle Zeichen wie die deutschen Umlaute (ä, ö, ü) enthalten.
- Neue Version 0.27.3 der Bibliothek exiv2 integriert, enthält Fehlerkorrekturen und einige neue Tags.

Folgende Fehler wurden behoben:

- Änderungen der GPS-Daten über die Karte wurden nicht gespeichert.
- Mehrere andere kleinere Fehler

Hinweis:

- Diese Version erfordert nun das .NET-Framework 4.0 (oder höher).

## Version 4.35 veröffentlicht am 17.11.2019

Erweiterungen und Verbesserungen:

- Neue Version 0.27.2 der Bibliothek exiv2 integriert mit Fehlerkorrekturen, zusätzlichen Objektivdaten, Nikon AutoFocus und Sony FocusPosition Metadaten.
- Die tags Exif.Image.XPAuthor, Exif.Image.XPComment, Exif.Image.XPKeywords, Exif.Image.XPSubject and Exif.Image.XPTitle können jetzt als Zeichenketten bearbeitet werden. Weil sie vom Typ Byte sind, konnten sie bisher nur als Byte-Vektor bearbeitet werden.
- Exif.Image.XPComment und Exif.Image.XPTitle können als Tags für das Speichern der Eingaben im Textfeld für Kommentar in der Mitte der Hauptmaske verwendet werden, Exif.Image.XPAuthor als Tag für Eingaben im Kombinationsfeld für Namen des Künstlers (Autor).

Folgende Fehler wurden behoben:

- Manchmal wurden die Dateien nicht sortiert in der Liste angezeigt.

## Version 4.34 veröffentlicht am 28.12.2018

Erweiterungen und Verbesserungen:

- Maske für das Einfügen und Bearbeiten von Platzhaltern hinzugefügt.
- Netzwerkordner und Standardordner "Bilder" werden im Verzeichnisbaum angezeigt.

Folgende Fehler wurden behoben:

- Programmabsturz bei Mehrfachbildbearbeitung, wenn Kommentar nicht gefüllt und "Kommentar anhängen" ausgewählt war.
- Programmabsturz nach mehrfachem Drücken von Strg-A in der Dateiliste.
- Export von Eigenschaften mit mehreren Werten (z.B. vom Typ LangAlt, XmpSeq) war unvollständig.

## Version 4.33 veröffentlicht am 02.12.2018

Erweiterungen und Verbesserungen:

- Daten-Vorlagen können definiert werden um damit mehrere Eigenschaften gleichzeitig zu setzen.
- Markierung für Aufnahmeort (und damit die Koordinaten) können mit rechter Maustaste entfernt werden.
- Schaltflächen und Menüeintrage werden abhängig vom Kontext aktiviert bzw. deaktiviert.
- Wenn nicht gespeicherte Änderungen verloren gehen können, z.B. weil andere Bilder ausgewählt werden oder das Programm beendet werden soll, hat der Anwender drei Möglichkeiten: Speichern und fortsetzen, fortsetzen ohne Speichern oder die neue Aktivität abbrechen. Bisher gab es zwei Möglichkeiten, abhängig von der jeweiligen Situation.
- Die Escape-Taste und die Schaltfläche "Zurücksetzen" können auch verwendet werden, wenn mehrere Bilder ausgewählt wurden.

Folgende Fehler wurden behoben:

- Anstatt maskenbezogener Hilfe wurde stets die Lizenz-Information angezeigt.
- Speicherproblem beim Export ausgewählter Eigenschaften der Bilder in einem Verzeichnis.

## Version 4.32 veröffentlicht am 21.09.2018

Erweiterungen und Verbesserungen:

- Über Konfigurationsdatei kann die Anzeige von versteckten Dateien und Ordnern aktiviert werden.
- Kleinere Erweiterungen in der Fehlerbehandlung.
- Upgrade von Leaflet (Komponente für Kartendarstellung) auf 1.3.4
- Kartendarstellung kann aus mehreren Quellen gewählt werden, darunter topographisch, Satellit und hybrid.

Folgende Fehler wurden behoben:

- Suche nach Orten in der Karten-Ansicht funktionierte nicht (Anfrage wurde von OpenStreetMap nicht akzeptiert).

## Version 4.31 veröffentlicht am 01.03.2018

Erweiterungen und Verbesserungen:

- In den Reitern für Exif, IPTC, XMP und sonstige Eigenschaften können Felder markiert und per Kontextmenü (rechte Maustaste) in den Bereich für änderbare Eigenschaften oder den Reiter Übersicht hinzugefügt werden.
- Im Reiter Übersicht können Felder markiert und per Kontextmenü (rechte Maustaste) in den Bereich für änderbare Eigenschaften hinzugefügt werden.
- Im Reiter für XMP-Eigenschaften wird die Sprache in der Spalte Typ bei Einträgen vom Typ LangAlt hinzugefügt, da dieser Typ für verschiedene Sprachen unterschiedliche Werte erlaubt.
- Verbesserte Prüfungen der Platzhalter.

Folgende Fehler wurden behoben:

- Nicht zutreffende Meldung " Für ... weicht der gespeicherte Wert ... vom Zielwert ... ab", wenn Kommentar in Xmp.dc.description oder Xmp.dc.title gespeichert werden sollte.
- Bei Mehrfach-Bildbearbeitung mit Platzhaltern wurde für alle Bilder die Ersetzung des ersten Bildes gewählt. Jetzt erfolgt die Ersetzung für jedes einzelne Bild individuell.

## Version 4.30 veröffentlicht am 05.11.2017

Erweiterungen und Verbesserungen:

- Per Drag-and-Drop und über den Menüeintrag "Datei - Öffnen" können auch Bilder über URLs geöffnet werden. Sie werden dazu in den Ordner "Downloads" heruntergeladen.
- Mehrere Dateien können gelöscht werden (bisher war nur einzeln löschen möglich).
- Die Dateieigenschaften "Erstellt am/um" und "Geändert am/um" können auf das Aufnahmedatum (Exif.Photo.DateTimeOriginal) gesetzt werden.
- Neue Version 0.26 der Bibliothek exiv2 integriert mit ca. 250 neuen Feldern (Tags), insbesondere XMP sowie Lesen einer Initialisierungsdatei mit Zuordnungen von Objektiv-Namen zu Objektiv-Kennnummern (für die Anzeige von ExifEasy.LensName).

Folgende Fehler wurden behoben:

- Bei einigen XMP-Einträgen (festgestellt mit Fotos, aufgenommen mit iPhone) stürzte das Programm ab.
- Bei Mehrfach-Speichern konnte das Programm manchmal "einfrieren".

## Version 4.29 veröffentlicht am 25.02.2017

Erweiterungen und Verbesserungen:

- Anzeige von Bild Details in separater Maske möglich (insbesondere nützlich, wenn zwei Bildschirme verfügbar sind). Mehrere Fenster können geöffnet werden, um Details von mehreren Bildern vergleichen zu können.
- Der sichtbare Bereich des Bildes in "Bild Details" kann durch Bewegung der Maus bei gedrückter linker Maustaste verschoben werden.
- Aufnahmeort eines Bildes können auf einer Karte angezeigt und die zugehörigen Daten geändert werden. Dies ist in einem der Bereiche der Hauptmaske oder einer separaten Maske möglich.

## Version 4.28 veröffentlicht am 22.12.2016

Folgende Fehler wurden behoben:

- Programmabsturz beim Speichern im Anzeige-Modus "Kacheln" oder "Miniaturansicht".

## Version 4.27 veröffentlicht am 18.12.2016

Erweiterungen und Verbesserungen:

- Starten des Programmes beschleunigt.

Fehlerkorrekturen:

- Nach dem Löschen eines Bildes wurde ein falsches Vorschaubild angezeigt. Der Fehler ist behoben.

## Version 4.26 veröffentlicht am 17.11.2016

Fehlerkorrekturen:

- Fehler in der Anzeige wurde behoben.

## Version 4.25 veröffentlicht am 13.11.2016

Erweiterungen und Verbesserungen:

- Ein Ordner- oder Dateiname kann als Argument in der Kommandozeile übergeben werden, womit es möglich wird, das Programm über "Senden an" im Kontextmenü des Windows Explorers zu nutzen.
- Dateien können über Drag-and-Drop geöffnet werden.
- Neuer Menüeintrag "Datei - Öffnen" um Ordner oder Dateien durch die Eingabe des vollständigen Namens (d.h. mit vollständiger Pfadangabe) öffnen zu können.
- Maske "Felddefinitionen": Ermöglicht es eine Liste gültiger Werte zu definieren, die in der Hauptmaske im konfigurierbaren Eingabebereich zur Eingabeprüfung verwendet wird.
- Haupt-Maske: Wenn Exif.Image.Orientation zum konfigurierbaren Eingabebereich hinzugefügt wird, wird eine Auswahlliste angezeigt. Diese enthält die gültigen (numerischen) Werte zusammen mit einer Erläuterung (z.B. "bottom, left (180° + horiz.flip)"). Nach Speichern der Änderung von Exif.Image.Orientation, wird das Bild entsprechend gedreht.
- Öffnen von Ordnern wurde beschleunigt.
- Während mit der Bildlaufleiste in der Dateiliste mit Ansicht Kacheln oder Miniaturansicht geblättert wird, werden keine Vorschaubilder neu erzeugt. Lediglich bereits vorhandene Vorschaubilder werden angezeigt. Dadurch kann erheblich schneller geblättert werden. Bei schneller Drehung des Mausrades wird ebenfalls die Erzeugung von Vorschaubildern vermieden.
- Haupt-Maske: Größe und Abstände in Kachel- und Miniaturansicht können über die allgemeine Konfigurationsdatei angepasst werden.
- Haupt-Maske: Neue Schaltflächen um zum ersten und letzten Bild im Ordner zu springen.

Fehlerkorrekturen:

- Ein Fehler beim Drehen der Bilder basierend auf der in den Exif-Eigenschaften gespeicherten Orientierung wurde behoben.

## Version 4.24 veröffentlicht am 27.09.2016

Erweiterungen und Verbesserungen:

- In der Maske "Felddefinitionen" können für Datums-Werte fünf weitere Formate ausgewählt werden. Diese Formate können über die allgemeine Konfigurationsdatei individuell definiert werden.

Fehlerkorrekturen:

- Wenn beim Auslesen der Metadaten aus den Bildern ein Fehler auftrat, konnte in diesen Bildern keine Metadaten geändert werden, auch die nicht, die korrekt angezeigt werden konnten. Dieser Fehler ist behoben.
- Übersetzung in Englisch war nicht vollständig auf Rechnern, die eine andere Code Page als 1252 verwendet haben. Dies führte auch zu einer Fehlermeldung beim Start. Dieser Fehler ist behoben.

## Version 4.23 veröffentlicht am 22.09.2016

Erweiterungen und Verbesserungen:

- Der Speicherort für Benutzer-Einstellungen kann ausgewählt werden:
  - %Appdata%:  
        Falls auf dem Rechner mehrere Benutzer eingerichtet sind, hat jeder Benutzer eigene Einstellungen.  
        Einstellungen bleiben beim Wechsel auf eine neuere Programmversion erhalten.  
        Das Programm-Verzeichnis kann schreibgeschützt sein.
  - Programm-Verzeichnis:  
        Empfohlen für portablen Einsatz auf USB-Stick: die Einstellungen sind ebenfalls auf dem USB-Stick, es werden keine Einstellungen auf einem anderen Rechner abgelegt.  
        Beim Wechsel auf eine neuere Programmversion müssen die Einstellungen kopiert werden oder die Programm-Dateien im aktuell verwendeten Ordner überschrieben werden.
- In der Maske "Felddefinitionen" können für Datums-Werte folgende Formate ausgewählt werden:  
    Lokales Datum/Zeit-Format (entsprechend der Systemeinstellungen)  
    ISO Datum/Zeit-Format (z.B. 2016-09-20T18:25:00)
- Wenn beim Auslesen der Metadaten aus den Bildern ein Fehler auftrat, wurden bisher keine Metadaten angezeigt. Da diese Fehler bisher immer nur einzelne (und für den Anwender eher uninteressante) Eigenschaften betrafen, werden jetzt Metadaten angezeigt.
- Da Fehler bei den Metadaten erfahrungsgemäß keine für den Anwender interessanten Eigenschaften betreffen, wurde eine Einstellung geändert: In diesem Fall wird jetzt keine Message-Box mehr angezeigt. Auf Wunsch kann diese über die Maske "Einstellungen" geändert werden.

Fehlerkorrekturen:

- Wenn keine Internet-Verbindung vorhanden war, stürzte das Programm bei der Prüfung auf neue Version ab. Der Fehler ist behoben.

## Version 4.22 veröffentlicht am 20.05.2016

Erweiterungen und Verbesserungen:

- Maske "Ansicht Anpassen": Die Ansicht kann angepasst werden sodass mehre Bereiche nebeneinander anstatt übereinander angezeigt werden. Mehrere benutzerdefinierte Ansichten können mit Namen gespeichert werden.
- Hauptmaske - konfigurierbarer Eingabebereich: Für die Eingabe eines Datums kann ein Kalender geöffnet werden (neue Schaltfläche rechts neben dem Eingabefeld).
- Hauptmaske: Über Kontextmenü kann direkt die Maske "Felddefinitionen" geöffnet werden, um die Eigenschaften im konfigurierbarem Eingabebereich, im Reiter "Übersicht", in der Datei-Anzeige mit Ansicht "Kacheln" und in der Tabelle für "Mehrfach-Bildbearbeitung" zu ändern.
- Maske "Meta-Daten" entfernen:  
    Über Schaltflächen kann direkt die Maske "Felddefinitionen" geöffnet werden, um die zu entfernenden Eigenschaften bzw. die Ausnahmen auszuwählen.
- Maske "Dateien umbenennen":  
    Die Auswahllisten für "Feld" und "sortieren nach" haben einen Eintrag "&lt;neues Feld&gt;", über den direkt die Maske "Felddefinitionen" geöffnet werden kann, um die Auswahllisten anzupassen.
- Maske "Aufnahmedatum/zeit ändern":  
    Auswahlliste für Gruppierung (oben links) enthält einen neuen Eintrag "alle" sowie einen Eintrag "andere Gruppierung", mit dem direkt die Maske "Felddefinitionen" geöffnet wird zur Anpassung der Gruppierungen.
- Maske "Dateien vergleichen":  
    Über Schaltfläche "Ausgeblendete Spalten konfig." kann direkt die Maske "Felddefinitionen" geöffnet werden, um die zu nicht zu vergleichenden Spalten zu konfigurieren.
- Export: Ausgew. Eigenschaften der Bilder im Verzeichnis:  
    Vor dem Export erscheint Abfrage zum Öffnen der Maske "Felddefinitionen" um die zu exportierenden Eigenschaften auswählen zu können.

Fehlerkorrekturen:

- Video-Daten wurden nicht korrekt angezeigt.
- Prüfung auf neue Version hat mit der vorherigen Version verglichen (und damit fälschlicherweise gemeldet, dass eine neue Version verfügbar sei).
- Diverse andere kleinere Fehler.

## Version 4.21 veröffentlicht am 25.10.2015

Erweiterungen und Verbesserungen:

- Neue Version 0.25 der Bibliothek exiv2 integriert mit ca. 350 neuen Feldern (Tags), insbesondere XMP, Panasonic und Casio.

Fehlerkorrekturen:

- Maske "Felddefinitionen": Nach Betätigung der Schaltfläche "Meta Datum 1" stürzte das Programm ab. Das ist nun behoben.

## Version 4.20 veröffentlicht am 29.03.2015

Erweiterungen und Verbesserungen:

- Anpassung für Bildschirme mit DPI Werten größer als 96  
    Diese Version ist nun auch verwendbar, wenn DPI über die Windows Konfiguration "Text und weitere Elemente vergrößern oder verkleinern" oder "Benutzerdefinierte Textgröße (DPI) festlegen" auf einen Wert größer als 96 gesetzt wird.

Fehlerkorrekturen:

- Die letzten beiden Versionen liefen nicht unter Windows XP. Das ist nun behoben.

## Version 4.19 veröffentlicht am 08.02.2015

Erweiterungen und Verbesserungen:

- Mehrsprachig  
    Das Programm kann nun auch auf Englisch umgestellt werden. Neue Sprachen können durch Hinzufügen einer Sprachdatei einfach verfügbar gemacht werden (sofern sich jemand findet, der die notwendigen Übersetzungen liefert).
- Hauptmaske, neu: Bild Details  
    In der Hauptmaske können "Bild Details" frei in einem der Bereiche (z.B. anstatt "Letzte und vordefinierte Kommentare") angezeigt werden. Angezeigt werden eine Bildausschnitt (mit variablem Zoom-Faktor) sowie graphische und numerische Darstellung von Helligkeit und RGB-Werten
- Hauptmaske:  
    In den Reitern Exif, IPTC und XMP wird die Beschreibung der Eigenschaft (sofern vorhanden) angezeigt, wenn der Mauszeiger über der ersten Spalte steht.
- Hauptmaske:  
    Neuer Menüeintrag "Verzeichnisbaum aktualisieren"
- Neue Maske "Auf neue Version prüfen"  
    Mit dieser neuen Maske kann geprüft werden, ob eine neue Version verfügbar ist. Zusätzlich kann hier eingestellt werden, ob und nach wie vielen Tagen bei Programmstart auf eine neue Version geprüft wird.
- Maske "Dateien vergleichen"  
    Wenn der Mauszeiger über der Spaltenüberschrift steht, wird die Beschreibung der Eigenschaft (sofern vorhanden) angezeigt.

Fehlerkorrekturen:

- Falls ein USB-Speichermedium nach Start des Programmes entfernt wurde und dann versucht wurde, darauf zuzugreifen, stürzte das Programm ab. Jetzt wird der Verzeichnisbaum in solchen Fällen (oder wenn ein Ordner nicht mehr vorhanden ist) aktualisiert.

## Version 4.18 veröffentlicht am 25.09.2014

Erweiterungen und Verbesserungen:

- Auslesen von Metadaten aus Video-Dateien und Anzeige eines Frames  
    Metadaten aus verschiedenen Typen von Video-Dateien können ausgelesen werden. Es werden grundsätzlich alle Typen unterstützt, die auch von der Bibliothek exiv2 (<www.exiv2.org>) unterstützt werden. In der Maske "Einstellungen" können die Datei-Erweiterungen definiert werden, für die die Metadaten angezeigt werden.  
    Die Auswahlliste für die Gruppe von Eigenschaften in der Maske "Felddefinitionen" ist erweitert worden um:  
    \- Anzeige im Reiter "Übersicht" – Video  
    \- Datei-Anzeige in Ansicht "Kacheln" – Video  
    Aus den Video-Dateien kann ein Frame angezeigt werden. In der Maske "Einstellungen" kann definiert werden, für welche Datei-Erweiterungen ein Frame angezeigt wird. Dort kann auch die Frame Position in Sekunden ab Anfang definiert werden.  
    Für welche Typen von Video-Dateien ein Frame angezeigt werden kann, hängt von dem System ab, auf dem QuickImageComment läuft. Ich habe leider keine Lösung finden können, die auf allen (noch) gängigen Betriebssystemen funktioniert. Daher auch die Konfiguration der Datei-Erweiterungen.  
    Die Anzeige des Videos ist nicht Bestandteil des Programmes, ist aber - sofern der jeweilige Video-Typ vom System unterstützt wird - durch Doppelklick in der Dateiliste möglich.
- Hauptmaske:  
    Es können bis zu sechs Raster über das Bild gelegt werden. In der neuen Maske "Raster definieren" können Breite, Höhe, Farbe und Typ (durchgehende Linie, durchgehende Linie mit Skala, gestrichelte Linie, Fadenkreuz) definiert werden. Die Raster ermöglichen z.B. die Prüfung auf Verzeichnung eines Objektes oder "Ausmessen" von Details (speziell bei der Einstellung mit Skala).
- Konfiguration:  
    Mit dem Eintrag "KeepFileModifiedTime:yes" in der allgemeinen Konfigurationsdatei bleibt das Datei-Änderungsdatum beim Speichern erhalten.
- Hauptmaske:  
    Die Ankreuzfelder für IPTC Schlüsselworte und zu ändernde Eigenschaften im Reiter "Mehrfach-Bildbearbeitung" wechseln nun den Status mit einem Click (bisher: erster Click = Auswahl, zweiter Click = Statuswechsel).
- Maske "Meta-Daten entfernen":  
    Die Ankreuzfelder wechseln nun den Status mit einem Click (bisher: erster Click = Auswahl, zweiter Click = Statuswechsel).
- Bessere Kontrolle des Speicherverbrauchs und Anzeige des freien Speichers in der Fußzeile der Hauptmaske.

Fehlerkorrekturen:

- Metadaten von PNG-Dateien wurden nicht ausgelesen (bei der 32-Bit-Version gab es dabei eine Fehlermeldung) und konnten nicht geändert werden. Der Fehler ist behoben.

## Version 4.17 veröffentlicht am 21.03.2014

Erweiterungen und Verbesserungen:

- Hauptmaske:  
    Die Position der Maske wird beim Beenden gespeichert und beim nächsten Start wieder eingenommen.

Fehlerkorrekturen:

- Hauptmaske:  
    Falls die Liste in einem der Reiter Exif, IPTC, XMP und Sonstige leer war und man auf die Überschrift klickte, führte das zu einem Programmabsturz. Der Fehler ist behoben.

## Version 4.16 veröffentlicht am 16.03.2014

Fehlerkorrektur:

- Hauptmaske:  
    Das Aus- und anschließende Einblenden der letzten Gruppe in den Reitern Exif, IPTC, XMP und Sonstige führte zu einem Programmabsturz. Der Fehler ist behoben.

## Version 4.15 veröffentlicht am 25.01.2014

Erweiterungen und Verbesserungen:

- Hauptmaske:  
    Im zentralen Eingabebereich ist die Beschriftung jetzt dynamisch. Falls für das Eingabefeld kein Feld (Tag) konfiguriert wurde, wird als Beschriftung "nicht konfiguriert" angezeigt und das Eingabefeld ist nicht aktiv. Falls genau ein Feld zum Speichern konfiguriert wurde, wird dieses Feld angezeigt. Falls mehr als ein Feld konfiguriert wird, wird der Text wie bisher angezeigt ("Künstler (Autor)", bzw. "Kommentar").
- Maske Felddefinitionen:  
    Die Reaktion des Programmes war für den Anwender kaum nachvollziehbar, wenn man versucht hat, ein Feld für den konfigurierbaren Eingabebereich einzutragen, das bereits für den zentralen Eingabebereich konfiguriert war. Das Verhalten wurde geändert.

Fehlerkorrekturen:

- Hauptmaske:  
    Speichern in einem schreibgeschützten Ordner führte zu einem Programmabsturz.
- Maske Felddefinitionen:  
    Beim Öffnen konnte es zu einem Programmabsturz kommen, abhängig von Betriebssystem, Ordnergröße und verfügbarem Speicher.

## Version 4.14 veröffentlicht am 05.01.2014

Erweiterungen und Verbesserungen:

- Maske "Dateien Umbenennen": Das Löschen von Einstellungen muss nun bestätigt werden.
- Hauptmaske: Fehler beim Lesen der Meta-Daten durch exiv2 werden als Warnung gemeldet (wurden bisher nicht gemeldet).
- Im Menü "?": Direkter Zugriff auf das Forum unter der Webseite <www.quickimagecomment.de>.

Fehlerkorrekturen:

- Wenn der Ordner, den das Programm beim Start öffnet, keine Bilder enthält, stürzte das Programm ab. Der Fehler ist behoben.

## Version 4.13 veröffentlicht am 28.12.2013

Erweiterungen und Verbesserungen:

- Verwendung der neuen Version 0.24 der Bibliothek exiv2, die einige neue Daten (z.B. Objektiv-Namen) liefert.
- Hauptmaske: Die Auswahl der Kategorie bleibt erhalten, wenn die Maske "Vordefinierte Kommentare" benutzt wird.

Fehlerkorrekturen:

- Mit einer Änderung von Version 4.9 zur Version 4.10 funktionierte die Anzeige und Änderung der Werte im konfigurierbaren Eingabebereich nicht mehr. Der Fehler ist jetzt behoben.
- Bilder, die skaliert wurden (Auflösung geändert), konnten fehlerhafte Exif-Daten enthalten und so zu einem Programmabsturz führen. Die fehlerhaften Exif-Daten werden nun ignoriert.

## Version 4.12 veröffentlicht am 02.12.2013

Erweiterungen und Verbesserungen:

- Neue Maske "Ansicht anpassen"  
    Über diese Maske können die Inhalte aller Bereiche außer dem Bereich mit dem Bild und den zentralen Eingabefeldern frei zugeordnet werden.  
    Beispiel: Wenn man die Listen der letzten und vordefinierten Kommentare nicht benötigt, kann man den die Felder für IPTC Schlüsselworte links neben dem konfigurierbaren Eingabebereich anzeigen lassen und hat damit etwas mehr Platz für das Bild und/oder die Anzeige der Eigenschaften.  
    Außerdem sind in der Maske die bereits vorhanden Möglichkeiten zur Anpassung der Ansicht (Anzeige der Dateien, Symbolleiste, etc.) möglich.
- Direkter Zugriff auf die Webseite <www.quickimagecomment.de> im Menü "?" (Startseite mit letzten Meldungen, Tutorials, Kontaktformular und Downloadbereich).
- Weitgehende Übersetzung der Tag-Beschreibungen  
    Auch hier gilt (wie für die Übersetzung der Tag-Namen in Version 4.11): Wenn die Bedeutung des Tags und damit eine korrekte Übersetzung nicht sicher war, wurde auf eine Übersetzung verzichtet.
- Symbol für Maske "Felddefinitionen" in Symbolleiste ergänzt

Fehlerkorrekturen:

- Wenn es zu einer Eigenschaft mehrere Werte gab (z.B. IPTC.Application2.Keywords), wurde der Eigenschaftsname beim zweiten und folgenden Werten nicht übersetzt. Dieser Fehler ist nun behoben. Außerdem enthielt der Eigenschaftsname einen intern verwendeten Anhang, um den Eintrag eindeutig zu machen. Der Anhang wird nicht mehr angezeigt.

## Version 4.11 veröffentlicht am 01.09.2013

Erweiterungen und Verbesserungen:

- Deutsche Übersetzung der Tag-Namen und zu einem kleinen Teil der Beschreibungen  
    Die Übersetzungen wurden möglichst so gewählt, dass zusammengehörige Tags in der Sortierung auch zusammen stehen.  
    Beispiel: "Category" und "SuppCategory" wurden mit "Kategorie" und "Kategorie zusätzlich" übersetzt, nicht als "Kategorie" und "zusätzliche Kategorie".  
    Wenn die Bedeutung des Tags und damit eine korrekte Übersetzung nicht sicher war, wurde auf eine Übersetzung verzichtet.
- Haupt-Maske
  - Die Tag-Namen in den Reitern Exif, IPTC, XMP und Sonstige der Hauptmasken sind nun überwiegend in Deutsch.
  - Über das Kontextmenü können die original englischen Tag-Namen angezeigt werden.
  - Über das Kontextmenü ist eine weitere Ansicht "Einfache Liste, Gruppe hinten" verfügbar:  
        In dieser Ansicht wird der Gruppen-Name nicht in einer eigenen Zeile angezeigt sondern steht jeweils hinter dem Tag-Namen. So können Eigenschaften unabhängig von ihrer Gruppe sortiert werden. Dies ist hilfreich, wenn man (speziell bei hersteller-spezifischen Eigenschaften) nicht weiß, in welcher Gruppe sie zu finden sind. Außerdem gibt es Eigenschaften, die in verschiedenen Gruppen enthalten sind - diese stehen dann auch untereinander.  
        Da diese Ansicht nur bei passender Sortierung hilfreich ist, ist sie nicht für englische Tag-Namen verfügbar (siehe Hinweis zur Übersetzung weiter oben).
  - Die Einstellungen für die Ansicht (Liste mit Überschriften/Einfache Liste, Deutsch/Englisch) werden nun gespeichert und die Anzeige wird beim nächsten Programmstart entsprechend eingestellt.
- Maske "Felddefinitionen"
  - Die Tag-Namen und einige Beschreibungen werden nun normalerweise in Deutsch angezeigt. Über ein Ankreuzfeld können auch die englischen (Original) Tag-Namen und Beschreibungen angezeigt werden.
  - Die Übersetzungen der Tag-Namen sind so gewählt, dass sie sich direkt als Name bei der Neuanlage einer Felddefinition eignen. Die vorgeschalteten Hierarchieebenen werden beim Anlegen einer neuen Felddefinition nicht in den Namen mit übernommen.  
        Beispiel:  
        Bisher wurde bei Auswahl des Tags "File.Size" auch "File.Size" als Name übernommen, jetzt wird als deutscher Tag-Name "Datei.Dateigröße \[kB\]" angezeigt und als Name "Dateigröße \[kB\]" in die Felddefinition übernommen.
- Maske "Dateien vergleichen"
  - Die Tag-Namen werden nun normalerweise in Deutsch angezeigt. Über ein Ankreuzfeld können auch die englischen (Original) Tag-Namen und Beschreibungen angezeigt werden.
  - Die Anzeige wird nach Tag-Namen sortiert.

Fehlerkorrekturen:

- Bei Änderung des Kommentars mit Mehrfach-Bildbearbeitung konnte eine Meldung kommen, dass der Kommentar nicht gespeichert wurde (obwohl das nicht der Fall war). Die falsche Meldung kommt nicht mehr.

## Version 4.10 veröffentlicht am 09.06.2013

Erweiterungen und Verbesserungen:

- Meta-Daten von Bildern können verglichen werden. Näheres hierzu in Kapitel Maske "Dateien vergleichen".
- Neuer Export: alle Eigenschaften der markierten Bilder. Je Bild wird eine Textdatei mit allen Eigenschaften (Meta-Daten) des Bildes erzeugt.
- Haupt-Maske
  - Reiter "Einzel-Bildbearbeitung"  
        Für die Tabellen in den Reitern "Exif", "IPTC", "XMP" und "Sonstige" können über das Kontext-Menü (rechte Maustaste) zwei Ansichten gewählt werden:  
        Liste mit Überschriften  
        Dies ist die voreingestellte Ansicht. Die Eigenschaften sind verschiedenen Gruppen zugeordnet. Vor jeder Gruppe wird der Gruppen-Name in einer grau hinterlegten Zelle angezeigt. Durch klicken in die graue Zeile können die zu der Gruppe gehörenden Eigenschaften ein- oder ausgeblendet werden.  
        Einfache Liste  
        In dieser Ansicht wird der Gruppen-Name nicht in einer eigenen Zeile angezeigt sondern steht jeweils am Anfang des Tag-Namens, womit etwas mehr Breite für die Anzeige benötigt wird. In dieser Ansicht können die Spalten sortiert werden, z.B. nach der Tag-Nummer.  
        Im Reiter "Sonstige" wird eine Gruppe "ExifEasy" angezeigt. Näheres zu Eigenschaften dieser Gruppe unter "Erleichterter Zugriff auf einzelne Exif-Eigenschaften".
  - Reiter "Mehrfach-Bildbearbeitung"  
        Durch Klicken auf die Spaltenüberschriften werden die Bilder entsprechend der Spalte sortiert.
- Maske "Dateien umbenennen":
  - Die Zeilen zur Definition des Dateinamens basierend auf Feldern können nun sortiert werden.
  - Texte in den Eingabefeldern werden grau hinterlegt, um Leerzeichen sichtbar zu machen.
  - Einstellungen zum Umbenennen der Dateien können unter einem Namen gespeichert werden. Damit können praktisch beliebig viele Einstellungen definiert und einfach ausgewählt werden.
- Erleichterter Zugriff auf einzelne Exif-Eigenschaften:  
    Einige Bild-Informationen können sowohl in den allgemeinen Exif-Eigenschaften als auch in Hersteller-spezifischen Eigenschaften gespeichert werden. Andere Informationen werden nur in den Hersteller-spezifischen Eigenschaften gespeichert. Eigenschaften der Gruppe "ExifEasy" ermöglichen es, auf diese Werte zuzugreifen, ohne sich auf einen Kamera-Hersteller festzulegen. Wenn die Werte ermittelt werden, werden die verschiedenen dazu gehörigen Eigenschaften durchsucht.  
    Zwei Anwendungsbeispiele:
  - Wird bei einer Nikon Spiegelreflexkamera die ISO-Einstellung auf "Hi" gesetzt, enthält Exif.Photo.ISOSpeedRatings keinen Wert. Die Einstellung wird aber in Exif.Nikon3.ISOSettings gespeichert. Exif.Nikon3.ISOSettings wird natürlich nicht von Kameras anderer Hersteller gefüllt. Mit dem Tag-Namen Exif.\_sel.ISOspeed wird die ISO-Einstellung immer angezeigt, egal ob bei einer Nikon "Hi" eingestellt ist oder es sich um eine beliebige Kamera handelt.
  - Spiegelreflexkameras verschiedener Hersteller speichern das verwendete Objektiv, z.B. Sony in Sony1.LensID. Nikon speichert nur eine Referenznummer in NikonLd3.LensIDNumber. Mit ExifEasy.LensName wird das Objektiv für eine Reihe von Herstellern angezeigt, wobei die von Nikon verwendete Referenznummer in vielen Fällen durch den Objektivnamen ersetzt wird.
- Empfehlung für Umsteiger von früheren Versionen: Man sollte in der Maske "Felddefinitionen" prüfen, ob nicht in der einen oder anderen Definition einer der neuen Tag-Namen "ExifEasy..." sinnvoll ist.
- Bei der Anzeige von Eigenschaften gibt es u.a. folgende Optionen:
  - Interpretiert (Original)
  - Interpretiert = Original
  - Original (Interpretiert)
  - Original = Interpretiert
- Falls der interpretierte Wert identisch mit dem Original-Wert ist, wird nun nur noch ein Wert angezeigt.

## Version 4.9 veröffentlicht am 25.02.2013

Erweiterungen und Verbesserungen:

- Meta-Daten können gelöscht werden. Dazu gibt es zwei Optionen:
  - Entfernen von Gruppen von Meta-Daten: Exif, IPTC, XMP und JPEG Kommentar. Die Gruppen können einzeln gewählt werden. Es können Eigenschaften ausgewählt werden, die dabei nicht entfernt werden (Ausnahmen).
  - Entfernen von Meta-Daten, die einzeln ausgewählt werden.
- Es können Platzhalter für Eigenschaften verwendet werden, um die Werte von Eigenschaften in andere Eigenschaften zu kopieren. Näheres hierzu (mit Beispielen von Anwendungsfällen) in Kapitel Platzhalter für Eigenschaften.
- Falls die Bilddatei nicht lesbar ist (Datei ist leer, entsprechender Codec nicht installiert oder schlicht keine Bild-Datei) beendet sich das Programm nicht mehr.
- Die Eigenschaften, die im Reiter "Mehrfach-Bildbearbeitung" angezeigt werden, können nun konfiguriert werden.
- Neues Tag "File.DirectoryName" verfügbar, hauptsächlich ergänzt um in der Export-Datei der Eigenschaften leichter nach Verzeichnissen filtern zu können.
- Neben JPEG-Dateien können nun auch weitere Bildformate bearbeitet werden:  
    BMP, GIF, PNG, TIFF sowie verschiedene RAW-Formate wie CR2 (Canon), NEF (Nikon), ...  
    Für das Anzeigen von RAW-Bildern muss zusätzlich das Microsoft-Kamera-Codec-Paket installiert werden.
- Bei den änderbaren Eigenschaften können nun auch Eigenschaften geändert werden, die aus mehreren Werten bestehen (Felder).  
    Beispiel:  
    Exif.Nikon3.Lens; der Wert "180/10 1050/10 35/10 56/10" steht für das 18-105mm F3.5-5.6  
    Diese Eigenschaft kann nun für ältere Objektive ohne CPU nachgetragen werden.
- Weitere Zoom-Einstellungen: 2:1, 4:1, 8:1
- Maske Feldeigenschaften:
  - Auswahlliste für Formatierung ergänzt um "Dezimalzahl ohne Nachkommastellen"
  - Bei Neueinträgen oder Änderungen wird nun verhindert, dass Meta Datum 1 mehrfach verwendet wird.  
        Grund: mehrfache Einträge sind nicht sinnvoll und bei den konfigurierbaren Eingabefeldern entstünden Konflikte (zwei Eingabefelder für die gleiche Eigenschaft). Da bei der Anzeige keine Konflikte entstehen können, ist die mehrfache Verwendung einer Eigenschaft als Meta Datum 2 weiterhin möglich.

Fehlerkorrekturen:

- Wenn beim Abspeichern die beiden Bereiche "Letzte/Vordefinierte Kommentare" und "Eingabe für weitere Eigenschaften" ausgeblendet waren, wurde beim nächsten Start der Bereich "Eingabe für weitere Eigenschaften" wieder sichtbar. Jetzt sind beide Bereiche beim nächsten Start wieder ausgeblendet.
- Eigenschaften im Reiter "Mehrfach-Bildbearbeitung" werden nach dem Speichern aktualisiert.

## Version 4.8 veröffentlicht am 13.08.2012

Erweiterungen:

- Allgemein:
  - Neben Bildern mit Dateierweiterung .jpg werden jetzt auch Bilder mit .jpeg angezeigt.
- Haupt-Maske:
  - Layout-Änderung:  
        Die Bereiche für "letzte Kommentare" und "vordefinierte Kommentare" sind in einem Bereich mit zwei Reitern zusammengefasst worden. Der Bereich unten rechts (bisher für "vordefinierte Kommentare") ist jetzt ein konfigurierbarer Eingabebereich, in dem Eingabefelder für frei auswählbare Felder angezeigt werden. Dieser konfigurierbare Eingabebereich ersetzt die Auswahlliste für weitere Eigenschaften und das zugehörige Textfeld für weitere Eigenschaften.
  - Der Dateifilter kann mit der Return-Taste aktiviert werden.
  - Das Textfeld für freie Eingabe von IPTC-Schlüsselworten hat nun einen vertikalen Rollbalken und die Schlüsselworte werden alphabetisch sortiert angezeigt.
  - Die XMP-Tags vom Typ "LangAlt" und "XmpSeq" können mehrere Werte haben, die bisher in einer Zeile, durch Komma getrennt, angezeigt wurden. Jetzt wird jeder Wert in einer Zeile angezeigt.
- Maske "Felddefinitionen":
  - Die Exif-Datentypen Byte, SByte, Double und Float, die IPTC-Datentypen Date und Time sowie die XMP-Datentypen LangAlt, XmpBag, XmpSeq und XmpText können jetzt in der Liste für Änderung von Eigenschaften eingetragen werden.
  - Bei Auswahl von numerischen Datentypen in der Liste für Änderung von Eigenschaften erfolgt ein Meldung, die auf mögliche Gefahren hinweist (siehe auch das neue Kapitel Hinweise zu Datentypen).
- Verhalten bei Tags mit mehreren Werten  
    Bis zur Version 4.7 wurden mehrere Werte für ein Tag nur in den Reitern für Exif, IPTC und XMP angezeigt - jeder Wert in einer Zeile. An allen anderen Stellen (z.B. in der Ansicht Kacheln) wurde nur jeweils ein Wert angezeigt. Mehrere Werte konnten nur für das Tag "Iptc.Application2.Keywords" geändert werden. In dem Textfeld für weitere Eigenschaften wurde nur ein Wert angezeigt und es konnte auch nur ein Wert geändert werden.  
    Die Anzeige mehrerer Werte für ein Tag in den Reitern für Exif, IPTC und XMP bleibt unverändert. In den Textfeldern für weitere Eigenschaften im neuen konfigurierbaren Eingabereich der Hauptmaske können nun mehrere Werte angezeigt und geändert werden (sofern für das Tag mehrere Werte zulässig sind). An allen anderen Stellen werden mehrere Werte für ein Tag in einer Zeichenkette angezeigt, wobei die Werte durch einen senkrechten Strich (" | ") getrennt werden.

Fehlerkorrekturen:

- Maske "Felddefinitionen":  
    Definitionen "für Änderung von Eigenschaften" werden mit Anzeige-Typ "Original" (bisher "Interpretiert") definiert. Falls "Interpretiert" von "Original" abwich, konnte der Wert nicht geändert werden.
- Hauptmaske:  
    XMP-Werte mit "Ä", "Ö", "Ü" und "ß" werden nun korrekt angezeigt. "ä", "ö" und "ü" (Kleinbuchstaben) wurden auch bisher korrekt angezeigt.
- Hauptmaske:  
    IPTC-Werte, die als UTF8-kodiert waren, wurden nicht korrekt angezeigt. Das Tag "Iptc.Envelope.CharacterSet" wird jetzt ausgewertet, um zu prüfen, ob die IPTC-Werte in UTF8 kodiert sind.