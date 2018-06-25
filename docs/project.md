#Projektbeschreibung

Hier finden Sie eine detaillierte Beschreibung des MOVE-Projektes 

##Installationshinweise
Verwendete Software:
<ul>
    <li> Nodejs </li>
    <li> git-scm </li>
    <li> Angular 5 </li>
    <li> Node Package Manager </li>
    <li> Visual Studio Code </li>
</ul>
Um das Projekt erstmals zu starten müssen die Projektdateien zuerst in VS Code geöffnet werden. Anschließend muss zuerst der Befehl "npm install" ausgeführt werden, um die grundlegenden, nicht im Git gespeicherten Bibliotheken zu installieren. Danach kann das Projekt mit dem Befehl "ng --serve --port 4200" gestartet werden. In der darauf folgenden Fehlermeldung stehen alle von uns zusätzlich installierten Pakete. Diese müssen manuell mit dem Befehl "npm --save install [Paketname]" nachinstalliert werden. Ist dies geschehen, sollte Move nach dem nochmaligen ausführen von "ng --serve --port 4200" im Browser unter "localhost:4200" problemlos erreichbar sein.

##Hintergrund
Move ist eine Website für Studenten der Technischen Hochschule Ingolstadt, die im Ausland studieren oder ein Praktikum machen wollen.
Die THI bietet bereits umfangreiche Informationen zu den Partnerhochschulen, sowie einige Erfahrungsberichte an, allerdings sind diese für die Studierenden nur schwer auffindbar und ohne wirkliche Struktur an verschiedenen Stellen im Moodle der Hochschule gespeichert.
Wenn man es sich doch antut, alle diese Informationen auszuwerten und sich für ein Auslandssemester bewirbt, ist man bei allen weiteren Dingen auf sich allein gestellt, wenn man sich nicht selbstständig mit Fragen an einen Mitarbeiter des International Office wendet.

Deswegen soll Move alle relevanten Informationen an einem Ort bündeln und den Studenten übersichtlich präsentieren um die Frustration der Studenten im Bewerbungsprozess für ein Auslandssemester zu reduzieren.

##UX und Design Konzept
Als wir dieses Semester mit der Implementierung der Website begannen, war das nicht das erste Mal, dass wir uns mit dem Thema Move befassten. Bereits im Semester davor arbeiteten wir ein Designkonzept aus, um mit der späteren Website eine möglichst gute User Experience zu schaffen.
<mark>Hier würde eine Beschreibung des UX Konzeptes kommen, wenn wir das brauchen / wollen</mark>

##Projektablauf
Die Umsetzung des Projekts erfolgte mithilfe von Angular 5.
Da wir mit der Umsetzung von Move zum erstem Mal mit Angular oder überhaupt irgendeinem Workframe in Berührung kamen, mussten wir uns zunächst in den Angular Workflow einarbeiten.

Anschließend setzten wir auf der Grundlage unseres Prototyps die Komponenten und das Routing für die Website, sowie die Pseudodatenbank auf. Danach implementierten wir parallel zueinander die einzelnen Unterseiten.
Zuletzt schrieben wir noch die seitenübergreifende Logik wie zum Beispiel das Favorisieren einer Universität oder den Login.