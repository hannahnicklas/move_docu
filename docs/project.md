#Projektbeschreibung

Hier finden Sie eine detaillierte Beschreibung des MOVE-Projektes 

##Installationshinweise
Verwendete Software:
<ul>
    <li><a href="https://nodejs.org/en/download/">Nodejs </a></li>
    <li><a href="https://git-scm.com/downloads"> git-scm </a></li>
    <li> Angular 5 (npm install -g @angular/cli@1.7.4)</li> 
    <li> Node Package Manager (in Nodejs enthalten)</li>
    <li><a href="https://code.visualstudio.com/download"> Visual Studio Code </a></li>
    <li><a href="https://github.com/hannahnicklas/move">Git Repository</a></li>
</ul>

Erstmaliges starten des Projekts
<ol>
    <li><a href="https://nodejs.org/en/download/">Nodejs </a> installieren</li>
    <li> <a href="https://git-scm.com/downloads"> git-scm </a> installieren</li>
    <li><a href="https://code.visualstudio.com/download"> Visual Studio Code </a> oder andere Entwicklungsumgebung installieren</li>
    <li> Den Projektordner aus dem <a href="https://github.com/hannahnicklas/move">Git Repository</a> klonen und auf dem PC speichern </li>
    <li> In Visual Studio Code, oder anderer IDEA den Projektordner öffnen </li>
    <li> In der Konsole an den Speicherort navigieren (wenn Projektordner in VisualCode geöffnet ist, befindet man sich in der VSCode Konsole bereits dort) </li>
    <li> npm install -g @angular/cli@1.7.4 </li>
    <br>
    <ol style="background-color: lightgrey">
        Nur für Mac User
        <li>Ab macOS Sierra gibt es neue Sicherheitsvorschriften für das System, weshalb es notwendig sein könnte, die Befehle als Superuser sudo auszuführen. </li>
        <li> sudo npm install -g @angular/cli@1.7.4 </li>
        <li> Möglicherweise wurden trotz sudo nicht alle Packages installiert, weshalb diese nun einzeln nachinstalliert werden müssen. </li>
        <li> sudo install node scripts/build.js
             Damit der Befehl ordnungsgemäß ausgeführt werden kann, müssen die Develooper Tools von Apple installiert werden, dsfür bei dem Popup-Fenster auf installieren gehen. 
             Danach den Befehl nochmal ausführen:
             sudo install node scripts/build.jsS
             </li>
    </ol> 
     <li>npm install</li>
    <li>npm install firebase angularfire2 --save</li>
    <li>npm install ngx-breadcrumbs --save</li>
    <li>npm install mapbox-gl --save</li>
    <li>ng --serve --port 4200</li>
</ol>


##Hintergrund
Move ist eine Website für Studenten der Technischen Hochschule Ingolstadt, die im Ausland studieren oder ein Praktikum machen wollen.
Die THI bietet bereits umfangreiche Informationen zu den Partnerhochschulen, sowie einige Erfahrungsberichte an, allerdings sind diese für die Studierenden nur schwer auffindbar und ohne wirkliche Struktur an verschiedenen Stellen im Moodle der Hochschule gespeichert.
Wenn man es sich doch antut, alle diese Informationen auszuwerten und sich für ein Auslandssemester bewirbt, ist man bei allen weiteren Dingen auf sich allein gestellt, wenn man sich nicht selbstständig mit Fragen an einen Mitarbeiter des International Office wendet.

Deswegen soll Move alle relevanten Informationen an einem Ort bündeln und den Studenten übersichtlich präsentieren um die Frustration der Studenten im Bewerbungsprozess für ein Auslandssemester zu reduzieren.

##UX und Design Konzept
Als wir dieses Semester mit der Implementierung der Website begannen, war das nicht das erste Mal, dass wir uns mit dem Thema Move befassten. Bereits im Semester davor arbeiteten wir ein Designkonzept aus, um mit der späteren Website eine möglichst gute User Experience zu schaffen.
Genauere Informationen zum UX Konzept können unter Konzept gefunden werden.

##Projektablauf
Die Umsetzung des Projekts erfolgte mithilfe von Angular 5.
Da wir mit der Umsetzung von Move zum erstem Mal mit Angular oder überhaupt irgendeinem Workframe in Berührung kamen, mussten wir uns zunächst in den Angular Workflow einarbeiten.

Anschließend setzten wir auf der Grundlage unseres Prototyps die Komponenten und das Routing für die Website, sowie die Pseudodatenbank auf. Danach implementierten wir parallel zueinander die einzelnen Unterseiten.
Zuletzt schrieben wir noch die seitenübergreifende Logik wie zum Beispiel das Favorisieren einer Universität oder den Login.