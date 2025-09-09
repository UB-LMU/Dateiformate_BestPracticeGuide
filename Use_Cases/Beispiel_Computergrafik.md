---
title: Rendering von CGI
subject: Ingenieurwissenschaften
dataformat:
- Bildformat
---

## Name  
Rendering von CGI

## Use Case    
Im Bereich der Computergrafik, der Computer Generated Imagery (CGI), wird an der Optimierung von Rendering Verfahren geforscht, mit dem Ziel, die Zeiten für das Erreichen einer hohen Qualität der erzeugten Bilder zu reduzieren.
Dazu wird ein Modell entwickelt, welches die Limitierungen des menschlichen Auges bei der Erkennung von Unterschieden abbildet. Dieses Modell wird anschließend angewendet, um die Zeit für die Bilderzeugung reduzieren zu können.

## Kontext  
* Ingenieurwissenschaften  
* Informatik, System- und Elektrotechnik  
* Informatik    
* Bildformat  
* Bildqualität  

## Empfohlenes Vorgehen    
Bei Bildern können durch eine verlustbehaftete Kompression (lossy compression) bei der Speicherung wichtige Informationen der Originaldaten verloren gehen, so dass eine originalgetreue Rekonstruktion nicht mehr möglich ist. Die im vorliegenden Beispielfall erzeugten Forschungsdaten - Bilder - müssen jedoch für eine spätere Nutzung in höchstmöglicher Qualität gespeichert werden. Aus diesem Grund sollten Formate mit einer verlustfreien Datenkompression (lossless compression) wie beispielsweise das TIFF- oder das PNG-Format verwendet werden.

## Grund  
Im vorliegenden Anwendungsfall sind bereits feine Nuancen bei der Beurteilung der Bildqualität entscheidend. Verlustbehaftete Verfahren, welche beispielsweise auch beim JPEG-Format verwendet werden, nutzen jedoch ähnliche Mechanismen, wie sie beim beschriebenen Rendering Verfahren für die Optimierung der Renderingzeit eingesetzt werden sollen. Durch die Verwendung eines solchen Formats bei der Speicherung wäre eine anschließende Nutzung der Forschungsdaten für diesen Forschungszweck nicht mehr möglich, da durch die Komprimierung mit hoher Wahrscheinlichkeit wichtige Informationen verloren gegangen sind.

## Konsequenzen und Kosten  
Es entsteht kein zusätzlicher Aufwand für die Langzeitarchivierung, da die Bilder bereits für die Forschung im korrekten, verlustfrei komprimierenden Format gespeichert werden müssen. Sowohl das TIFF- als auch das PNG-Format sind für eine Archivierung im Sinne der Langzeitverfügbarkeit gut geeignet und es sind perspektivisch keine Migrationen zu erwarten. 

## Weitere Hinweise    
[Tiff (Wikipedia)](https://en.wikipedia.org/wiki/TIFF)  
[JPEG (Wikipedia)](https://en.wikipedia.org/wiki/JPEG)  

