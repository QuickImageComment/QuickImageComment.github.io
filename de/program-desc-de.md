QuickImageComment zeigt Exif-, IPTC- und XMP-Eigenschaften von Digitalbildern (z.B. JPEG und TIFF sowie einigen RAW-Formaten) an und ermöglicht sie zu ändern. Speziell die Bearbeitung von Benutzerkommentar und Künstler (Autor) wird erleichtert, indem auf die letzten eingegebenen und auf vordefinierte Werte zurückgegriffen werden kann. Metadaten (XMP) in Video-Dateien werden angezeigt.

### Übersicht der Funktionalitäten:
- Anzeige aller Exif-, IPTC- und XMP-Eigenschaften von Bildern, außerdem noch einige andere Dateieigenschaften wie z.B. Änderungsdatum.
- Anzeige von Metadaten (XMP) in Video-Dateien sowie (abhängig von der Windows-Version und ggfs. installierten Komponenten) Anzeige eines Frames des Videos.
- Bilder bzw. Videos können über ihre Eigenschaften und Aufnahmeort auf Karte gesucht werden.
- Neben den vollständigen Listen der Exif-, IPTC- und XMP-Eigenschaften wird eine Liste mit Eigenschaften angezeigt, die konfigurierbar ist.
- Neben Kommentar und Künstler können noch weitere Exif-, IPTC und XMP-Eigenschaften in Bildern geändert werden. Die Liste der änderbaren Eigenschaften ist konfigurierbar. 
- Daten-Vorlagen können definiert werden, um damit mehrere Eigenschaften gleichzeitig zu setzen.
- Platzhalter erlauben es, Werte von Eigenschaften in andere zu kopieren.
- Änderungen können auch für mehrere Dateien gleichzeitig durchgeführt werden.
- Exif-, IPTC- und XMP-Eigenschaften können gelöscht werden, dabei können Ausnahmen definiert werden. Einzelne Eigenschaften können gezielt gelöscht werden.
- Dateien können unter Verwendung von Exif, IPTC und XMP-Eigenschaften umbenannt werden.
- Die in den Dateien enthaltenen Exif-, IPTC- und XMP-Eigenschaften können verglichen werden.
- Eine spezielle Maske dient zum Synchronisieren der Aufnahmezeit einer Menge von Bildern, die mit verschiedenen Kameras aufgenommen wurden. Bilder werden nach Eigenschaften (meist Kamera-Modell) gruppiert. Für jede Gruppe kann eine Verschiebung der Aufnahmezeit eingegeben werden. Danach werden die Bilder sofort sortiert, um prüfen zu können, ob so die Bilder zeitlich in der richtigen Reihenfolge sind.
- Ausgewählte Eigenschaften aller Bilder/Videos eines Ordners (einschließlich eventuell vorhandener Unterordner) können in eine Textdatei exportiert werden.
- Alle Bildeigenschaften von ausgewählten Bildern/Videos können in Textdateien exportiert werden (eine Datei je Bild). 
- Anzeige von Bilddetails mit graphischer und numerischer Darstellung von Helligkeit und RGB-Werten.
- Anzeige des Aufnahmeortes auf einer Karte anhand der GPS-Koordinaten; Änderung der GPS-Koordinaten durch Wahl der Position auf der Karte.

Eine weitere Bearbeitung der Bilder (z.B. Anpassen von Kontrast und Helligkeit) ist nicht Sinn und Zweck dieses Programms.

Für das Auslesen und Ändern der Exif-, IPTC- und XMP-Eigenschaften wird die Bibliothek exiv2 verwendet. Auf [www.exiv2.org](www.exiv2.org) findet man neben der Beschreibung dieser Bibliothek auch umfangreiche Informationen und weiterführende Links zu Exif, IPTC und XMP. Die von exiv2 unterstützten Formate sind hier dokumentiert:  
[https://github.com/Exiv2/exiv2/blob/main/exiv2.md#file_types](https://github.com/Exiv2/exiv2/blob/main/exiv2.md#file_types)

Für die Anzeige von RAW-Bildern ist die LibRaw-Bibliothek integriert. Wenn der Codec des Kameraherstellers oder die Microsoft Raw Image Extension (die verschiedene RAW-Formate unterstützt) installiert sind, werden sie verwendet und die Anzeige ist dann in der Regel schneller. Man kann sowohl einen spezifischen Codec als auch die Microsoft-Erweiterung installieren. Der spezifische Codec wird dann für die entsprechenden Bilder verwendet. Für alle anderen wird zunächst die Microsoft Extension ausprobiert und als letzte Option die integrierte LibRaw-Bibliothek. Für die Anzeige der Metadaten wird kein Codec benötigt.

Das Programm läuft unter Microsoft Windows 7, 8, 10 und 11 und ist als 32-Bit und 64-Bit Variante verfügbar. Als Sprache kann Deutsch oder Englisch gewählt werden. Es gibt auch eine Variante mit leicht reduzierter Funktionalität, die unter Windows XP mit .Net 4.0 Framework läuft.

QuickImageComment ist freie Software. Sie können es unter den Bedingungen der GNU General Public License (wie von der Free Software Foundation veröffentlicht) verwenden.
