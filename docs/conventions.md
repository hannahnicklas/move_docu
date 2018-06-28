#Code Conventions 
Hier finden Sie alle Erklärungen zu den verwendeten Bezeichnungen und der Nomenklatur. 

##CSS Klassen 
Wir achteten sehr auf eine einheitliche und konsistente Benennung. Insbesondere sind häufig verwendete CSS Klassen für Schriften und Layout global ausgelagert. Die verwendeten CSS Klassen wurden möglichst nach den zu stylenden Objekten benannt. In allen Selektoren wird Kleinschreibung vorgesehen und Wortkombinationen erfolgen durch Bindestriche "-". Zusätzlich wird jede CSS Klasse mit der jeweiligen Seitenbenennung versehen, um die Zugehörigkeit zur Seite hervorzuheben und Doppelbenennungen zu vermeiden. So erhalten z.B. alle CSS Klassen der "university-consider" Komponente das Präfix "consider-".

###Beispiel 
![Screenshot](img/conventions/consider_screen.png)
![Screenshot](img/conventions/consider_example.png)

Das Präfix "consider-" gibt die Zugehörigkeit zur Komponente "university-consider" an und gewährleistet die Verwendung des Namens ausschließlich in dieser Komponente. Ein Objekt der Auflistung besteht aus einem Icon und einem Beschreibungstext, diese Kombination wird als "consider-fact" bezeichnet. Das zugehörige Icon ist Teil von "consider-fact" und erhält daher das Präfix "consider-fact-" und zusätzlich die Klasse "-icon" (class= "consider-fact-icon"). Nach demselben Prinzip erhält auch der Beschreibungstext eine Klasse. Er ist ebenfalls Teil von "consider-fact" und wird daher "consider-fact-text" benannt. Somit wird auch nochmals die Zusammengehörigkeit und die Ineinanderverschachtelung veranschaulicht.

##var.scss (globale Styles) 

Alle mehrmals vorkommenden Styles werden in der var.scss deklariert und können für alle Komponenten herangezogen werden. So stellen wir eine einheitliche Änderung von z.B. dem Margin jeder Seite oder bestimmter Farben sicher. Zudem bleibt der Code übersichtlicher und es werden weniger CSS Selektoren benötigt. 

Durch die Verwendung von SCSS haben wir in der var.scss einige Variablen für Farben und Schriftgrößen festgesetzt. Dabei unterscheiden wir zwischen Farben für Flächen und Hintergründe, wie $move-grey, und Textfarben wie, $text-color-orange. Außerdem werden die verwendeten Schriftgrößen festgesetzt ($font-size-medium). Diese Variablen werden verwendet, um einheitliche Klassen für die verschiedenen Schriften zu definieren. Da das Design sehr viele Schriftvarianten enthält, die sich durch Schriftgröße, Schriftfarbe und Schriftstil unterscheiden, ist es wichtig, diese global festzulegen, um Übersichtlichkeit sicherzustellen. 

![Screenshot](img/conventions/var.png)

Die Klassen werden zunächst nach dem verwendeten Schriftstil benannt (z.B. font-weight: lighter; --> ".light-"). Durch einen Bindestrich getrennt erfolgt dann ein Buchstabe der die Schriftgröße definiert. Der Buchstabe ergibt sich aus den Variablenbenennungen für die Schriftgröße (z.B. font-size: $font-size-medium --> "-M"). 

Da diese Klassen noch jeweils in verschiedenen Schriftfarben zur Verfügung stehen müssen werden weitere Klassen mit den Schriftfarben als Variablen definiert. Diese Klassen werden dann mit den Angaben zu Schriftstil und Schriftgröße kombiniert. 

Eine Schrift mit der Bennenung ".bold-L blue" besitzt daher den Schriftstil bold, die Schriftgröße Large und die Farbe Blau. 

![Screenshot](img/conventions/schriftkombination.png)

Die var.scss enthält auch eine Klasse ".flex-container" die die Grundeigenschaften einer Flexbox (display: flex; flex-flow: row-wrap;) beinhaltet. Diese wird in den Komponenten wiederverwendet und individuell angepasst. 