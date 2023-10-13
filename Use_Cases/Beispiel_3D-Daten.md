---
title: 3D-Digitalisierung
subject: Allgemein
dataformat:
- Bildformat
---

## Name  
3D-Digitalisierung

## Use Case  
Bei der 3D-Digitalisierung können Modelle und Scans in unterschiedlichen Dateiformate entstehen, abhängig von eingesetzter Technik und Software. Im Folgenden wird ein Überblick über gängige Formate gegeben:

*Photogrammetrie*: Bei der Photogrammetrie können aus Bildern 3D-Modelle erstellt werden. Die resultierenden Dateiformate können je nach Software und Verfahren variieren, aber gängige Formate sind beispielsweise OBJ, PLY oder glTF.

*3D-Scanner*: Je nach Art des 3D-Scanners können verschiedene Formate entstehen, z. B. STL, OBJ, PLY, XYZ, oder auch spezifische Formate, die von den Herstellern der Scanner verwendet werden.

*CAD (Computer-Aided Design):* CAD-Programme wie Autodesk AutoCAD oder SolidWorks verwenden oft eigene Dateiformate wie DWG (AutoCAD), SLDPRT (SolidWorks), oder auch STEP oder IGES, die als Industriestandards für den Austausch von CAD-Daten dienen.

*Animation und Visualisierung:* Bei der Erstellung von 3D-Animationen können Formate wie FBX, glTF oder Alembic (ABC) verwendet werden, um sowohl die 3D-Geometrie als auch die Animationen zu speichern.

*Echtzeit-Engines:* Für Echtzeit-Rendering-Engines wie Unity oder Unreal Engine werden häufig Formate wie FBX oder glTF verwendet, um 3D-Modelle in die Engine zu importieren.

*Medizinische Bildgebung:* Medizinische Scans: Bei medizinischen 3D-Bildgebungsverfahren wie CT (Computed Tomography) oder MRT (Magnetic Resonance Imaging) können DICOM (Digital Imaging and Communications in Medicine) oder NRRD (Nearly Raw Raster Data) als gängige Dateiformate verwendet werden.

*Virtuelle Realität (VR) und erweiterte Realität (AR):* Für immersive VR- und AR-Erlebnisse können Formate wie FBX oder glTF verwendet werden, um 3D-Modelle und Szenen in die virtuelle oder erweiterte Realität zu übertragen.

## Kontext 
* Allgemein  
* Bildformat  
* 3D-Digitalisierung  
* 3D-Modelle  

## Empfohlenes Vorgehen  

Um 3D-Dateien langfristig zu speichern und ihre Integrität und Zugänglichkeit über die Zeit zu gewährleisten, sollte ein robustes und weit verbreitetes Dateiformat gewählt werden, das von verschiedenen Softwareanwendungen unterstützt wird. Ideal sind offene Standardformate wie glTF oder OBJ, die eine gute Interoperabilität bieten.

*OBJ (Wavefront Object):*   
Vorteile: OBJ ist ein weit verbreitetes und plattformunabhängiges Dateiformat. Es unterstützt sowohl geometrische Informationen als auch Farbinformationen. Es kann von den meisten 3D-Softwareprogrammen gelesen und geschrieben werden.  
Nachteile: OBJ unterstützt keine Texturen oder Materialinformationen. Die Dateigröße kann relativ groß sein, insbesondere bei komplexen Modellen.

*STL (Standard Triangle Language):*   
Vorteile: STL ist ein häufig verwendetes Dateiformat für 3D-Modelle. Es besteht aus einer Sammlung von Dreiecksmeshes und speichert nur die Geometrie der Modelle. STL-Dateien sind klein und einfach zu handhaben.  
Nachteile: STL unterstützt keine Farbinformationen, Texturen oder komplexe Geometrien wie gekrümmte Oberflächen. Es ist nicht geeignet, um vollständige 3D-Modelle mit allen Details zu speichern.

*FBX (Filmbox):*  
Vorteile: FBX ist ein weit verbreitetes Dateiformat, das von vielen 3D-Softwareprogrammen unterstützt wird. Es kann sowohl geometrische Informationen als auch Animationen, Texturen und Materialien speichern. Es ist gut geeignet für den Austausch von 3D-Daten zwischen verschiedenen Softwareanwendungen.  
Nachteile: FBX ist ein proprietäres Dateiformat von Autodesk und die genaue Spezifikation ist nicht öffentlich verfügbar. Es kann zu Kompatibilitätsproblemen zwischen verschiedenen Versionen der Software kommen.

*PLY (Polygon File Format):*    
Vorteile: PLY ist ein flexibles Dateiformat, das sowohl geometrische Informationen als auch zusätzliche Attribute wie Farben, Normalen oder Texturkoordinaten speichern kann. Es ist einfach zu lesen und zu schreiben.  
Nachteile: PLY-Dateien können relativ groß sein, insbesondere wenn sie viele zusätzliche Attribute enthalten. Es wird möglicherweise nicht von allen 3D-Softwareprogrammen unterstützt.

*glTF (GL Transmission Format):*  
Vorteile: glTF ist ein plattformunabhängiges und effizientes Dateiformat für 3D-Modelle. Es unterstützt sowohl geometrische Informationen als auch Materialien, Texturen und Animationen. glTF-Dateien können in Echtzeitgrafikanwendungen verwendet werden und sind gut für Web-basierte 3D-Anwendungen geeignet.  
Nachteile: glTF ist ein vergleichsweise neues Format und wird möglicherweise nicht von allen älteren 3D-Softwareprogrammen unterstützt. Es kann Einschränkungen bei der Kompatibilität mit bestimmten Anwendungen geben.

Es ist wichtig zu beachten, dass die Wahl des Dateiformats von den spezifischen Anforderungen und Anwendungen abhängt. Einige Formate sind besser für den Austausch und die Zusammenarbeit zwischen verschiedenen Softwareanwendungen geeignet, während andere Formate spezifische Merkmale wie Farbinformationen oder Animationen unterstützen. Die Entscheidung für das passende Dateiformat sollte basierend auf den konkreten Anforderungen, der Kompatibilität mit der verwendeten Software und der beabsichtigten Verwendung getroffen werden.

Die Modelle sollten möglichst umfangreich mit Metadaten beschrieben werden, einschließlich Informationen wie Erstellungsdatum, Scanner, Autoren, Beschreibung und Nutzungslizenz. Metadaten erleichtern die spätere Verwaltung, Suche und Nutzung der Dateien.

## Grund  
Die Nachnutzung von Dateiformaten die mit proprietärer Software erstellt wurden, ist nur eingeschränkt möglich.
Eine Langzeitverfügbarkeit, sowie künftige Nachnutzung kann für diese Dateiformate ebenfalls nicht sichergestellt werden. Daher sollten nach Möglichkeit offene Dateiformate verwendet werden, beziehungsweise eine Konvertierung in diese erfolgen.

## Konsequenzen und Kosten  
Eine Konvertierung in offene Formate wie z.B. OBJ ist in vielen Fällen verlustfrei möglich. Diese können dann mit geringem Aufwand langfristig zugänglich gehalten werden.

## Weitere Hinweise  
[Task force report "3D content in Europeana"](https://pro.europeana.eu/project/3d-content-in-europeana)  
[Community Standards for 3D Data Preservation](https://www.ala.org/acrl/sites/ala.org.acrl/files/content/publications/booksanddigitalresources/digital/9780838939147_3D_OA.pdf)  
[Expert Group on Digital Cultural Heritage and Europeana](https://digital-strategy.ec.europa.eu/en/library/basic-principles-and-tips-3d-digitisation-cultural-heritage)  
