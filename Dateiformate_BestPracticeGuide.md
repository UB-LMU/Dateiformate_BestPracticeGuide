# Dateiformate für die Langzeitverfügbarkeit

## Hintergrund

Die langfristige Verfügbarkeit digitaler Informationen ist nicht nur eine Frage der zur Verfügung stehenden technischen Infrastruktur. Moderne, redundante Archivsysteme können formal den dauerhaften Erhalt von digital erfassten Informationen gewährleisten (Bitstream-Preservation)[^1]. Dies erfordert allerdings regelmäßige Investitionen, um alternde Hardware auszutauschen. Damit alleine ist aber noch nicht sichergestellt, dass die Daten langfristig auch tatsächlich nutzbar bleiben. Entscheidend ist auch, ob die digitalen Informationen von zukünftigen Systemen und letztlich Personen noch sinnvoll verstanden werden können.

Dies ist insbesondere dann nicht mehr sichergestellt - und damit die langfristige Verfügbarkeit der Informationen gefährdet - wenn:  
- die Daten in Dateiformaten abgelegt wurden, die zu einem späteren Zeitpunkt von Computern nicht mehr ohne Informationsverlust interpretiert werden können   
- eine spezialisierte, nicht weitverbreitete Software notwendig ist, um die Dateien überhaupt verwenden zu können.

Während der zweite Fall oft bereits zum Zeitpunkt der Archivierung absehbar ist, ist das Risiko eines langsamen "Veraltens" von Dateiformaten nicht immer offensichtlich. Um dies zu minimieren, sollte idealerweise bereits beim Erstellen der Daten, aber spätestens beim Einbringen von Daten in ein Langzeitspeichersystem darauf geachtet werden, die Informationen in Formaten zu speichern, die allgemein als langfristig sicher angesehen werden.  Idealerweise sollte zusätzlich noch berücksichtigt werden, ob das Archivsystem bei drohendem Veralten die Daten automatisch auf modernere Formate migrieren - sprich in aktuelle Datenformate umwandeln - kann. 

Je nach erwarteten Nachnutzungsszenarios ist es dabei nicht immer nötig, das aus Sicht der Langzeitstabilität absolut beste Datenformat für den Datentyp zu wählen. Es kann beispielsweise ausreichen, eine pragmatische Lösung zu wählen, die den Erhalt der für die zukünftige Nachnutzungsszenarien entscheidenden Informationen sicherstellt. Dann rechtfertigen die Vorzüge eines formal überlegenden Dateiformats, unter Umständen nicht den mit dem Wechsel des Formates verbundenen Aufwand oder den möglicherweise durch eine Konvertierung entstehenden Informationsverlust.

Die Auswahl eines passenden Dateiformats ist also nicht immer offensichtlich. Daher soll diese Handreichung es Interessierten ermöglichen, sich bereits vor der Einreichung eines Datensatzes bei einem Archiv einen Überblick über geeignete Formate zu verschaffen. Die Empfehlungen wurden ursprünglich im Hinblick auf das in Bayern derzeit genutzte Langzeitarchivierungssystem Rosetta entwickelt. Da die Grundprinzipen der Langzeitverfügbarkeit jedoch unabhängig vom verwendeten Archiv gelten, kann die Handreichung auch in einem breiteren Kontext Anwendung finden. 

Anhand realer Fallbeispiele aus verschiedenen Fachdisziplinen mit unterschiedlichen Dateiformaten soll nicht nur eine Empfehlung für das Vorgehen im konkreten Anwendungsfall gegeben werden, sondern auch die sich daraus ergebenden möglichen Konsequenzen aufgezeigt werden. Für einen besseren Überblick werden die konkreten Fallbeispiele durch eine aus bereits existierenden Leitfäden und Handreichungen zusammengetragene Übersicht geeigneter Dateiformate ergänzt.

Der Leitfaden versteht sich ausdrücklich nicht als ein abgeschlossenes Dokument, sondern vielmehr als eine Empfehlungsgrundlage, die kontinuierlich um neue Fallbeispiele sowie weitere Dateiformate ergänzt werden kann.

## Aufbau der Fallbeispiele

Der Aufbau der Beispiele folgt grob der Struktur des sogenannten Pattern Konzepts[^2]. Dieses wird insbesondere in der Entwicklung verwendet, um kurz gesagt ein auftretendes Problem zu beschreiben und anschließend eine geeignete Lösungsmöglichkeit aufzuzeigen[^3]. Dabei wird stets eine fest formalisierte Struktur eingehalten. Diese erlaubt es, die Sammlung an Beispielen einfach und stetig zu erweitern sowie bei Recherchen schneller ein passendes Beispiel für die eigene Fragestellung zu finden. Je nach Anwendungsfall kann es daher für ein und dasselbe Dateiformat unterschiedliche geeignete Möglichkeiten für die Langzeitverfügbarkeit geben.  


### Name  
>Kurze, eindeutige Bezeichnung des Beispielfalls.

### Use Case  
>Beschreibung des konkreten Beispielfalls.

### Kontext  
>Auflistung von für den Beispielfall relevanten Rahmenbedingungen. Kann die Angabe des Datentyps, der Fachrichtung, des geplanten Nachnutzungsszenarios, des Datenvolumen oder weiterer Faktoren sein. 
Der Kontext soll es erleichtern ähnliche Beispiele zur eigenen Situation zu finden.

### Empfohlenes Vorgehen  
>Beschreibung des im vorliegenden Fall empfohlenen Vorgehens.

### Grund  
>Begründung des empfohlenen Vorgehens.  

### Konsequenzen und Kosten  
>Erläuterung des entstehenden Aufwands für die Konvertierung in ein anderes Format und Aufzeigen möglicher Konsequenzen, wenn eine andere Vorgehensweise gewählt wird. 

### Weitere Hinweise
>Verweise auf weiterführende Empfehlungen und Literatur.  



## Beispielsammlung


Die Beispiele werden im offen zugänglichen Repositorium GitHub gesammelt, kuratiert und bereitgestellt. Dadurch wird zum einen die freie Verfügbarkeit sichergestellt und zum anderen können somit neue Beispielfälle sowie Verbesserungvorschläge und Korrekturen einfach eingebracht werden. 

[https://github.com/UB-LMU/Dateiformate_BestPracticeGuide]


Ziel ist es, das Portfolio langfristig weiter auszubauen, mit weiteren beispielhaften Anwendungsfällen anzureichern und diese nachhaltig zur Verfügung zu stellen. Um die Sichtbarkeit zu erhöhen und eine bessere Zugänglichkeit zu erreichen, werden die Beispiele zusätzlich auf Zenodo veröffentlicht sowie in die Webseite der LZV-Initiative Bayern eingebunden.

[Link folgt]




## Allgemeine Empfehlungen

Für einen ersten Überblick zu geeigneten Dateiformaten für die Langzeitverfügbarkeit, kann die ["Interaktive Tafel gängiger Dateiformate"](https://www.lzv.nrw/dateiformate/) der Landesinitiative Langzeitverfügbarkeit lzv.nrw genutzt werden. Anhand der Dateiendung kann schnell überprüft werden, ob das vorliegende Dateiformat für die Langzeitverfügbarkeit geeignet ist.
Weitergehende, detailliertere Erläuterungen zu den einzelnen Dateiformaten finden sich in zahlreichen Quellen[^4]. Aus diesen wurde eine kurze Übersicht über empfohlene, bedingt geeignete und nicht geeignete Dateiformate zusammengestellt.   
Generell sollte bei der Auswahl von Dateiformaten darauf geachtet werden, dass diese möglichst und je nach Verwendungszweck offen, transparent, weit verbreitet sowie gut dokumentiert sind. 


|Dateityp|Empfohlene Dateiformate|Bedingt geeignete Dateiformate|Nicht geeignete Dateiformate|
|-----|-----|-----|-----|
|**Text**|<ul><li>Unformatierter Text (.txt): kodiert als ASCII, UTF-8 oder UTF-16 mit Byte Order Mark</li><li>PDF/A (.pdf): explizit für die Langzeitarchivierung entwickeltes Format, die Verwendung der Version PDF/A-2 wird empfohlen</li><li>XML (inklusive XSD/XSL/XHTML)(.xml): Angabe von Schema und Buchstabenkodierung</li></ul>|<ul><li>PDF (.pdf): spezielle Funktionalitäten und eingebettete Objekte problematisch</li><li>HTML (.html): Sicherung weiterer Ressourcen zur korrekten Darstellung notwendig</li><li>Open Document Format (.odt; .odp): offener Standard, nicht eingebettete Elemente und Makros problematisch</li><li>Office Open XML (.docx; .pptx): proprietäres Format, nicht eingebettete Elemente problematisch</li><li>LaTeX, TeX (.tex): verwendete Softwarepakete zusätzlich archivieren, nach Möglichkeit nur zusätzlich zu PDF/A-2</li></ul>|<ul><li> Microsoft Word (.doc): obsoletes, proprietäres Format</li><li> Microsoft PowerPoint (.ppt): obsoletes, proprietäres Format</li></ul>|
|**Rastergrafik**|<ul><li>Tagged Image File Format (TIFF)(.tiff): keine Patenteinschränkung oder technische Schutzmechanismen</li><li> Portable Network Graphics (PNG)(.png): verlustfrei komprimierendes Format u.a. für die Webdarstellung</li><li>JPEG2000 (.jp2, .jpg2): verlustfrei komprimierendes Format, v.a für Fotografien</li></ul>|<ul><li> JPEG (.jpeg, .jpg): verlustbehaftete Komprimierung</li><li>Graphics Interchange Format (GIF)(.gif): Vorgänger des PNG-Formats</li></ul>||
|**Vektorgrafik**|<ul><li>Scalable Vector Graphics (.svg; .svgz): XML-basiertes offenes Format, ermöglicht einfache Zugänglichkeit, nach Möglichkeit ohne script bindings archivieren</li></ul>|<ul><li>Drawing Interchange File Format (.dxf): offen dokumentiertes, aber proprietäres Austauschformat für CAD-Daten</li></ul>|<ul><li>Adobe Illustrator (.ai): proprietäres Format</li><li>CorelDraw (.cdr): proprietäres Format</li></ul>|
|**Tabellen**|<ul><li>Comma-separated values (CSV)(.csv): weit verbreitetes, offenes Austauschformat mit reinen Textdateien</li></ul>|<ul><li>Open Document Spreadsheet (ODS)(.ods): offener Standard, falls Erhaltung der Funktionalität notwendig, nicht eingebettete Inhalte problematisch</li><li> Office Open XML (.xlsx): proprietäres Format, falls Erhaltung der Funktionalität notwendig</li></ul>|<ul><li>Microsoft Excel (.xls): obsoletes, proprietäres Format</li></ul>|
|**Datenbanken**|<ul><li>Software Independent Archival of Relational Databases (SIARD)(.siard): auf XML-basierendes offenes Format für die Langzeitarchivierung, Archivierung der Datenbankstruktur und -inhalte</li><li>Strucured Query Language (SQL)(.sql): SQL-Dump, geeignet insofern ein offizieller, dokumentierter ISO-Standard verwendet wird</li>|<ul><li>Comma-separated values (CSV)(.csv): erlaubt keine Darstellung von Beziehungen, Metadaten und Strukturinformationen</li></ul>|<ul><li>Microsoft Access (.mdb): obsoletes, proprietäres Format</li></ul>|
|**Audio**|<ul><li>Waveform Audio File Format (WAV)(.wav): weit verbreitetes, offenes Containerformat für unkomprimierte Audiodaten</li><li>Free Lossless Audio Codec (FLAC)(.flac): frei verfügbarer, verlustfrei komprimierender Codec</li></ul>|<ul><li>MPEG-1 Audio Layer 3 (MP3)(.mp3): weit verbreitetes, verlustbehaftet komprimierendes Austauschformat</li></ul>||
|**Video**|<ul><li>Matroska (.mkv): offenes Containerformat, das zahlreiche Codecs unterstützt, in Verbindung z.B. mit dem Codec FFV1 für die LZA geeignet</li></ul>|<ul><li>MPEG-4 Part 14(MP4)(.mp4): ISO-zertifiziertes Containerformat, kann in Verbindung mit dem H.264-Codec sowie einer verlustfreien Kompression verwendet werden</li><li>Motion JPEG 2000 (MJ2): ISO-zertifiziertes Containerformat, sollte nur in Verbindung mit verlustfrei komprimierenden Codecs verwendet werden</li></ul>|<ul><li>Audio Video Interleave (AVI)(.avi): proprietäres Format</li><li>Quick Time File Format (MOV)(.mov): proprietäres Containerformat</li></ul>|


[^1]: Siehe [forschungsdaten.info-Glossar](https://forschungsdaten.info/praxis-kompakt/glossar/#c500908).
[^2]: Alexander C, Ishikawa S, Silverstein M, et al (1977) A Pattern Language. Oxford University Press, New York. 
[^3]: Johnson R, Helm R, Gamma E, Vlissides, J (2015). Design Patterns: Entwurfsmuster als Elemente wiederverwendbarer objektorientierter Software. mitp, Heidelberg.
[^4]: siehe beispielsweise:  
        [forschungsdaten.info](https://forschungsdaten.info/themen/veroeffentlichen-und-archivieren/formate-erhalten/)  
        [KOST](https://kost-ceco.ch/cms/kad_main_de.html)  
        [IANUS](https://ianus-fdz.de/it-empfehlungen/dateiformate/index)  

