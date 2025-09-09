---
title: Statistische Modelle, Neuronale Netzwerke, LLMs
subject: Allgemein
dataformat:
- Software
---

## Name    
Statistische Modelle, Neuronale Netzwerke, LLMs

## Use Case

In der Forschung oder bei iterativen Datenaufbauten sind frühere Modelle oft interessant (z. B. um zu sehen, wie sich die Performanz mit zusätzlichen Trainingsdaten verändert). Bei verwandten Architekturen oder Transfer Learning kann es auch sinnvoll sein, auf alten Gewichten aufzubauen (Pretraining, Fine-Tuning). Für das Speichern bestehender Modellen (genauer: die trainierte Gewichte und ggf. Metadaten) gibt es noch kein universelles Datenformat, das von allen genutzt wird. Stattdessen verwenden unterschiedliche Frameworks teils eigene Formate [^1]:

* **PyTorch** speichert Modelle üblicherweise als *.pt*, *.pth* oder *.pkl* (binäre Pickle-Dateien)[^2].
* **TensorFlow** nutzt savedModel, ein Verzeichnis bestehend aus Protobuf(*.pb*)-Dateien mit Modellstruktur und Metadaten und Unterverzeichnissen mit den Modelldaten[^3].
* **Keras** nutzt bevorzugt *.keras* (zip-Verzeichnis mit Modelldaten, Metadaten und Graph), alternativ auch HDF5-Dateien (*.h5*)[^4]. Es erlaubt aber auch Tensorflow/PyTorch-spezifische Formate.
* **R** nutzt *.rds* für einzelne Modellobjekte oder *.rda* / *.RDATA* für mehrere Objekte oder gesamte Workspaces[^5].

Folgende Formate/Standards sind unabhängig von der verwendeten Software nutzbar:

* **ONNX (Open Neural Network Exchange)[^6]** ist ein offener Standard, der den Austausch zwischen verschiedenen Frameworks erleichtern soll. Besonders relevant für die Interoperabilität der Modelle.

* **CSV oder JSON** eignen sich lediglich für kleine Modelle oder für die Visualisierung, sind aber in der Praxis zu ineffizient für moderne Netze (bei Millionen von Gewichten wäre entweder das nötige Speichervolumen zu groß oder die Präzision ist niedrig, außerdem leidet die Ladezeit).

* **PMML (Predictive Model Markup Language)[^7]** ist ein XML-basierter offener Standard, der vor allem im Kontext zu Business Analytics und Data Mining verbreitet ist und den Transfer von Statistischen Modellen zwischen verschiedenen Programmen ermöglicht.


In der Praxis zeigt sich aber, dass alte Modelle oft schnell überholt sind, wenn z. B. die Architektur komplett geändert wurde. Dann sind die alten Gewichte nicht mehr direkt nutzbar.
Bei deterministischen Modellen reicht es theoretisch auch Seed, Daten, Architektur und Hyperparameter zu speichern, um das Modell erneut zu erzeugen. In der Praxis ist das jedoch nicht trivial, etwa aufgrund von Framework-Updates, Hardwareunterschieden, Zufälligkeit bei Datenshuffling. Außerdem kann die erneute Berechnung eines Modells einen hohen Zeit- und Ressourcenbedarf erfordern, der eine Erstellung des Modells zum Zweck der Evaluation oder Nachnutzung unrentabel macht.


## Kontext    
* Statistik
* Large Language Models
* Machine Learning
* Neuronale Netze
* Python
* R

## Empfohlenes Vorgehen    
Das Speichern eines Modells in einem proprietären Binärformat des jeweiligen Frameworks sollte zur Datensicherung und Nachvollziehbarkeit mehrfach im Auswertungsprozess durchgeführt werden.
Beim Archivieren der Daten sollte des Weiteren ein Export nach ONNX/PMML oder bei kleineren Modellen in ein gebräuchliches Textformat geprüft werden.
Grundsätzlich müssen bei der Archivierung außer den trainierten Modellen auch die Skripte die zur Erstellung benutzt wurden, abgelegt werden, inklusive von Random-Seeds und anderen variablen Größen, die die Generierung verändern können (z.B. Hardwareparameter).
Die genutzten Trainingsdaten sollten, wenn möglich, ebenso abgeliefert werden, was sich durch die Datenmenge jedoch schwierig gestalten kann.

## Grund    
Für die Langzeitverfügbarkeit von Daten sollten grundsätzlich offene, nicht-proprietäre Dateiformate gewählt werden, die unabhängig von einem spezifischen Framework bzw. dessen Version sind.
Ein gemeinsames Speichern der Skripte und des resultierenden Modells ermöglichen eine Evaluation der Archivierung, indem das Skript erneut ausgeführt und mit dem gespeicherten Modell verglichen wird.
So wird auch die Replizierbarkeit sichergestellt, welche der guten wissenschaftlichen Praxis entspricht.


## Konsequenzen und Kosten    
Das langfristige Speichern von Modellen und Skripten ist oft nicht mit zu hohen Kosten verbunden, vor allem im Vergleich zu den Kosten, die Modelle zu erzeugen. 
Einen enormen Kostenfaktor kann jedoch die Archivierung der Trainingsdaten darstellen, da diese besonders bei Big-Data-Modellen mehr Speicherplatz benötigen als es wirtschaftlich sinnvoll ist.
Eine Lösung kann das zurückgreifen auf veröffentlichte Korpora an Daten sein, die für die Forschung zugänglich und nutzbar sind.
Hier sollte bei der Archivierung auf eine genaue Angabe der Quellen geachtet werden und bestenfalls eine periodische Überprüfung der Zugänglichkeit der genutzten Daten stattfinden.


## Weitere Hinweise

[^1]: [ML Model Formats and File Extensions](https://www.jocheojeda.com/2023/12/17/ml-model-formats-and-file-extensions/)
[^2]: [The difference of. Pt,. PTH,. Pkl](https://programmerah.com/the-difference-of-pt-pth-pkl-and-the-way-to-save-the-model-1777/)
[^3]: [Using the SavedModel format](https://www.tensorflow.org/guide/saved_model)
[^4]: [ Save and load models](https://www.tensorflow.org/tutorials/keras/save_and_load)
[^5]: [Saving Data into R Data Format: RDS and RDATA](https://www.sthda.com/english/wiki/saving-data-into-r-data-format-rds-and-rdata?title=saving-data-into-r-data-format-rds-and-rdata)
[^6]: [Wikipedia: Open Neural Network Exchange](https://en.wikipedia.org/wiki/Open_Neural_Network_Exchange)
[^7]: [Predictive Model Markup Language](https://en.wikipedia.org/wiki/Predictive_Model_Markup_Language)