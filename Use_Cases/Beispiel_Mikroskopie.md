---
title: Mikroskopische Aufnahmen
context:
- Bilddaten
- Lebenswissenschaften
- Mikroskopie
---

## Name    
Mikroskopische Aufnahmen  

## Use Case  
Am Mikroskop aufgenommene Bilder werden in der Regel standardmäßig in einem herstellerspezifischen proprietären Dateiformat abgespeichert, beispielsweise im Leica Image File Format (.lif) oder im Zeiss Vision Image - Format (.zvi). 

## Kontext  
* Bilddaten      
* Lebenswissenschaften  
* Mikroskopie  

## Empfohlenes Vorgehen  
Proprietäre Dateiformate sollten nach Möglichkeit in ein offenes nicht-proprietäres Format konvertiert werden. Typische Formate sind beispielsweise in das Tagged Image File Format (TIFF) oder in JPEG. Mithilfe des Open Source Tool Fiji (https://github.com/fiji) können viele der proprietären Formate geöffnet und anschließend im entsprechend gewünschten Format gespeichert werden.
Dabei sollte darauf geachtet werden, dass wichtige in dem Herstellerformat hinterlegte Metadaten ebenfalls erhalten bleiben.  

## Grund  
Proprietäre Firmenformate können zum aktuellen Zeitpunkt noch mithilfe der entsprechenden Firmen-Software geöffnet werden. Sollte jedoch in Zukunft beispielsweise der Support für eine der benötigten Softwares eingestellt werden, kann auf diese im Zweifelsfall nicht mehr zurückgegriffen werden. Die Dateien wären damit im Ursprungsformat unbrauchbar.

## Konsequenzen und Kosten  
Da mikroskopische Aufnahmen häufig auch mithilfe eines Bearbeitungsprogramms ausgewertet oder weiter bearbeiten werden, entsteht kein zusätzlicher Aufwand wenn die vorliegenden Bilddateien in einem weiteren Schritt zusätzlich in einem offenen Format abgespeichert werden.

Bei der Auswahl des offenen Formats sollte nach Möglichkeit darauf geachtet werden ein für die Langzeitverfügbarkeit geeignetes Format auszuwählen. Wenn für weitere Analysen beispielsweise hohe Auflösung und Farbtiefe notwendig ist, kann etwa das TIFF-Format gewählt werden. Werden die Aufnahmen hingegen lediglich zu Dokumentations- oder Präsentationszwecken verwendet, kann zum Beispiel auch das verlustbehaftet komprimierende Format JPEG verwendet werden.
Bei der Wahl des Formats sollte auch berücksichtigt werden, dass selbst ein verlustfrei komprimiertes TIFF-Format noch mehr Speicherplatz benötigt als etwa das JPEG-Format.
(Beispiel-Bild: TIFF - 7,53 MB vs. JPEG - 20,2 KB)

Werden die Daten lediglich im proprietären Hersteller-spezifischen Format abgespeichert, kann unter Umständen keine Langzeitverfügbarkeit gewährleistet werden, sondern lediglich eine technische Erhaltung der Daten (Bitstream Preservation) ermöglicht werden.

## Weitere Hinweise  
* [The Open Microscopy Environment](https://www.openmicroscopy.org/bio-formats/)  
* [Fiji-Git](https://github.com/fiji)  
