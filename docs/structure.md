# Projektstruktur
Hier finden Sie eine Erklärung über unsere gewählte Projekt- bzw. Ordnerstruktur und Methode. 

##Ordnerstruktur
###App
![Screenshot](img/structure/src.jpg) <br>
Die Ordnerstruktur der App ergibt sich aus der Ineinanderstapelung der verschiedenen Angular Komponenten und Services.
Auf der obersten Ebene befinden sich die vier Hauptseiten der Seite (Home, Study Abroad, Internship, User), sowie eine Komponente für die Navigationsleiste oben und den Footer unten. Die vier inhaltlichen Komponenten unterteilen sich dann noch mal in ihre entsprechenden Unterkomponenten.

###Assets
![Screenshot](img/structure/assets.jpg) <br>
Unter Assets haben wir alle Dateien abgelegt, die mit zur Seite gehören, aber kein Code sind. Diese haben wir in drei unterschiedliche Gruppen unterteilt.
Unter Data liegt unsere Pseudodatenbank und die in ihr abgelegten Datentypen als Typescript Dateien. Die Verwendung dieser von Angular bereitgestellten Datenbank war uns dabei vorgegeben.
Da Angular es nicht erlaubt, mehrere Datenbanken dieses Typs in ein Projekt einzubinden, waren wir gezwungen, alle unsere Daten untereinander in eine Tabelle zu speichern (university-data.service.ts).  

Bei Move verwendeten wir SCSS statt CSS. Das erlaubte es uns, Variablen festzulegen und diese im kompletten CSS der Seite weiterzuverwenden. Da wir das globale style.scss-File der Seite nicht komplett mit Variablendeklarationen füllen und damit unübersichtlich machen wollten, entschieden wir uns dafür, diese Auszulagern. Deswegen liegt im Ordner GlobalScss eine var.scss Datei, in der sämtliche SCSS Variablendeklarationen für unser Projekt hinterlegt sind.
Unter images sind alle Bilder gespeichert, die wir auf der Seite verwenden. Wir haben darauf geachtet, die Ordnerstruktur im images-Ordner identisch zu der Ordnerstruktur des Projektes an sich zu halten, um die Wiederauffindbarkeit einzelner Bilder zu erleichtern.

##Routing 
![Screenshot](img/structure/routing.jpg)
Das Routing ist Angular typisch über das bereitgestellte routing-module.


##Gliederung in Komponenten 
Durch Angular legten wir alle Unterseiten und wiederverwendbaren Codebausteine in einzelne, ineinandergeschachtelte Komponenten an. 
Komponentne können mit Angular leicht über den Befehl "ng generate component komponentenname" generiert werden und beinhalten die HTML, SCSS und Typescript Dateien der Komponente. Diese einzelnen Komponenten können nun beliebig als HTML-Tag durch ihren Selektor (in der Typescript Datei) wiederverwendet werden. Dies wendeten wir als Beispiel bei der Anzeige der Vorschau der einzelnen Experiences an. 