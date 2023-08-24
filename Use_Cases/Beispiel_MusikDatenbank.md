---
title: Musik-Datenbanken
context:
- Datenbank
- Geisteswissenschaften
- Faktendatenbank
---


## Name    
Musik-Datenbanken

## Use Case  
In einem musikwissenschaftlichen Projekt werden Schaffende, deren Lebensdaten, Werke, Aufführungen und weitere Informationen in einer SQL-Datenbank erfasst. Die Datenbank besteht aus mehreren Tabellen.  

## Kontext    
* Datenbank
* Geisteswissenschaften
* Faktendatenbank

## Empfohlenes Vorgehen    
Aus Datenbanken können die darin enthaltenen Informationen sowie die Struktur der Datenbank in Form von sogenannten Datenbankdumps exportiert werden. Dabei wird beispielsweise bei SQL-Datenbanken eine Datei mit einer Liste von SQL-Befehlen erzeugt, die die Datenbank abbilden. Diese Dumps sind reine Text-Dateien und daher sehr gut langfristig digital zu archivieren. Aus dem Dump kann die Datenbank exakt in dem Zustand wiederhergestellt werden, in dem sie sich zum Zeitpunkt des Dumps befand. 

Zusätzlich zum Dump können die einzelnen Tabellen auch als CSV-Dateien gespeichert werden. Dieser zusätzliche Aufwand, der bei einfachen Datenbanken in der Regel gering ist, ermöglicht einen etwas direkteren Zugang zu den Informationen.         

## Grund    
Die Archivierung der Datenbank-Datei selbst garantiert nicht zwangsläufig, dass diese langfristig auch geöffnet und mit vollem Funktionsumfang genutzt werden kann. Datenbankdumps haben den Vorteil, dass - auch wenn die Datenbanksprache nicht mehr aktiv verwendet wird - alle Informationen aus der Textdatei rekonstruiert werden können.  

## Konsequenzen und Kosten  
Der Aufwand für die Erstellung eines Datenbankdumps ist gering. Meist kann dieser mit einem einzigen Datenbankbefehl erzeugt werden - etwa [bei PostgreSQL](https://www.postgresql.org/docs/current/backup-dump.html). Eine Wiederherstellung erfolgt ebenfalls durch ein kurzes Datenbankkommando, mit dem eine leere Datenbank aus dem Dump befüllt wird. Es wird empfohlen, zu prüfen, ob die Datenbank aus dem Dump fehlerfrei rekonstruiert werden kann oder ob eine Fehlermeldung auftritt.

Bei großen Datenbanken kann der Dump speicherintensiv sein. In diesen Fällen ist es von Vorteil, den Dump nach der Fehlerkontrolle zu komprimieren, beispielsweise mit gzip oder einem anderen Programm. Das geringere Datenvolumen reduziert die Kosten für die Archvierung und beschleunigt den Datentransfer.

Bei der Archivierung der Datenbank selbst ist eine langfristige Verfügbarkeit nicht sichergestellt. Wenn die Datenbankstruktur von zukünftig verwendeten Programmen nicht mehr vollständig interpretiert werden kann, können wichtige Informationen verloren gehen. Durch eine entsprechende Kuratierung kann das verhindert werden. Dies erfordert jedoch Ressourcen, die für Datenbankdumps nicht notwendig sind.  

## Weitere Hinweise   
* [Datenbankdump (Wikipedia)](https://en.wikipedia.org/wiki/Database_dump)

