---
title: Lehr- und Lernvideos
subject: Lebenswissenschaften
dataformat:
- Multimediaformat
---

## Name    
Lehr- und Lernvideos

## Use Case    
An einem Lehrstuhl für Didaktik einer Hochschule werden Lehrvideos zu verschiedenen Experimenten für eine Nutzung im Schulunterricht produziert. Diese werden im Containerformat QuickTime (.mov) mit dem Videocodec MPEG-2 gespeichert.

## Kontext   
* Lebenswissenschaften  
* Didaktik  
* Multimediaformat  
* Lehrvideos  

## Empfohlenes Vorgehen    
Neben dem Containerformat der Videodateien müssen für eine Langzeitverfügbarkeit auch die enthaltenen Codecs berücksichtigt werden. Generell sollten die Videos dafür einerseits nach Möglichkeit in einem offenen Containerformat gespeichert werden und andererseits sollte, wenn möglich keine verlustbehaftete (lossy) Kompression verwendet werden. Ein mögliches offenes Containerformat, das für die Langzeitverfügbarkeit gut geeignet ist, ist beispielsweise das Matroska-Format (.mkv). In Kombination mit diesem ist der offene und verlustfrei komprimierende Codec FFV1 für Videos gut geeignet, sowie falls benötigt FLAC als verlustfrei komprimierender Codec für Audiodaten.
Sofern die Videos noch im Rohdatenformat vorliegen, können diese direkt in passenden Formaten für die Langzeitverfügbarkeit gesichert werden. Liegen die Videos hingegen nur in einem bereits komprimierten Format vor, sollte abgewogen werden, ob eine Konvertierung in ein offenes Format sinnvoll ist. Denn die Konvertierung von bereits komprimierten Dateien in ein anderes Dateiformat kann zu weiteren Informationsverlusten führen.
Es wird empfohlen, sich frühzeitig über die verschiedenen Formate zu informieren und die für den jeweiligen Zweck geeigneten auszuwählen.

## Grund    
Grundsätzlich sind für die Sicherung im Sinne der Langzeitverfügbarkeit immer offene, gut dokumentierte und nicht-proprietäre Formate zu bevorzugen. Dies gilt sowohl für die verwendeten Container als auch für die darin enthaltenen Codecs. Das im vorliegenden Fall verwendete QuickTime-Format ist zwar ein offen dokumentiertes, aber dennoch proprietäres Containerformat von Apple. Das Format erlaubt grundsätzlich auch die Integration verschiedener offener Video- und Audiocodecs, welche für die Langzeitverfügbarkeit gut geeignet sind, jedoch kann es aufgrund des proprietären Containerformats bei einer eventuell notwendigen Migration zu Problemen kommen.  
Generell sind Dateien in einem unkomprimierten Format für die Langzeitverfügbarkeit am besten geeignet. In der Praxis ist dies bei Videodaten aufgrund des hohen Speicherplatzbedarfs aber of nur schwer realisierbar. Daher sollte bei der Komprimierung nach Möglichkeit darauf geachtet werden, dass diese verlustfrei (lossless) erfolgt, um Informationsverlust zu vermeiden. Der in dem Beispiel-Fall verwendete Videocodec MPEG-2 komprimiert die Daten in der Regel verlustbehaftet (lossy), ebenso wie die anderen weit verbreiteten MPEG-Standards. Je geringer die Kompressionsrate ist, desto höher ist auch der Speicherplatzbedarf (Beispiel-Video mit einer Dauer von 30 min: unkomprimiert - 600 GB vs. FFV1-Codec - 350 GB vs MPEG-4-Codec - 1.8 GB).

## Konsequenzen und Kosten    
Sofern die Videodateien in einem proprietären Format gespeichert werden, kann im Sinne der Langzeitverfügbarkeit unter Umständen nur eine technische Erhaltung (Bitstream Preservation) erfolgen. Dadurch besteht die Möglichkeit, dass die Dateien in Zukunft nicht mehr genutzt werden können, da eine Migration in ein zukünftig aktuelles Dateiformat nicht mehr möglich ist. Bei komprimierten Dateien sollte außerdem berücksichtigt werden, dass es bei jeder Migration zu weiteren Datenverlusten kommen kann, wodurch Informationen verloren gehen können, so dass auch hier die Möglichkeit besteht, dass die Dateien nicht mehr nutzbar sind. 
Welche Codecs für welchen Zweck geeignet sind, sollte im Einzelfall und in Abhängigkeit von der späteren Nutzung entschieden werden. 

## Weitere Hinweise    
* [Videoformate (KOST)](https://kost-ceco.ch/cms/videoformate-einleitung.html)
