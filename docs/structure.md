# Projektstruktur

Hier finden Sie eine Erklärung über unsere gewähle Projekt- bzw. Ordnerstruktur und Methode. 

##Ordnerstruktur

###App
![Screenshot](img/structure/src.jpg) <br>
Die Ordnerstruktur der App ergiebt sich aus der Ineinanderstapelung der verschiedenen Angular Komponenten und Services.
Auf der Obersten Ebene befinden sich die vier Hauptseiten der Seite (Home, Study Abroad, Internship, User), sowie eine Komponente für die Navigationsleiste oben und den Footer unten. Die vier inhaltlichen Komponenten unterteilen sich dann noch mal in ihre entsprechenden Unterkomponenten.

###Assets
![Screenshot](img/structure/assets.jpg) <br>
Unter Assets haben wir alle Dateien abgelegt, die mit zur Seite gehören, aber kein Code sind. Diese haben wir in drei unterschiedliche Gruppen unterteilt.
Unter Data liegt unsere Pseudodatenbank und die in ihr abgelegten Datentypen als Typescript Dateien. Die Verwendung dieser von Angular bereitgestellten Datenbank war uns dabei vorgegeben.
Da Angular es nicht erlaubt, mehrere Datenbanken dieses Typs in ein Projekt einzubinden, waren wir gezwungen, alle unsere Daten untereinander in eine Tabelle zu speichern (university-data.service.ts). <br>
Bei Move verwendeten wir scss statt css. Das erlaubte es uns, Variablen festzulegen und diese im kompletten css der Seite weiterzuverwenden. Da wir das globale style.scss file der Seite nicht komplett mit Variablendeklarationen füllen und damit unübersichtlich machen wollten, entschieden wir uns dafür, diese Auszulagern. Deswegen liegt im Ordner GlobalScss eine var.scss Datei, in der sämtliche scss Variablendeklarationen für unser Projekt hinterlegt sind. <br>
Unter images sind selbsterklärend alle Bilder gespeichert, die wir auf der Seite verwenden. Wir haben darauf geachtet, die Ordnerstruktur im images Ordner identisch zu der Ordnerstruktur des Projektes an sich zu halten, um die Wiederauffindbarkeit einzelner Bilder zu erleichtern.

##Routing 
![Screenshot](img/structure/routing.jpg)
Das Routing ist Angular typisch über das bereitgestellte routing-module.

##Methoden  

## Gliederung in Komponenten 