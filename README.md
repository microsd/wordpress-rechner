# wordpress-rechner
Einfachen Online-Rechner für Wordpress erstellen.

Diese Anleitung erklärt, wie man in Wordpress einen einfachen Online-Rechner erstellen kann. Ein solcher Rechner ist Beispielhaft auf der Seite http://www.micro-sd.net/kapazitaetsrechner/ zu sehen. Es gibt dort mehrere Eingabefelder, aus denen der Benutzer die umzurechnenden Größen bestimmt. Das Ausgabefeld wird automatisch aus den Eingaben errechnet. Das Tool führt dabei eine Syntaxprüfung durch und es wird die deutsche Schreibweise mit Komma als Dezimaltrennzeichen sowie Punkt zur 1.000er Gruppierung verwendet. Es wird eine funktionierende Wordpress-Installation vorausgesetzt.
Für einfache Online-Rechner eignet sich das kostenlose Plugin [Calculated Fields Form](https://wordpress.org/plugins/calculated-fields-form/):
![Plugin installieren](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/calculated_fields_form.jpg)
Nach dem Installieren und Aktivieren bitte auf Plugins->Installierte Plugins->Calculated Fields Form->Einstellungen Klicken. Dann unter "New Form" einen Namen eintragen und ein neues Formular erstellen:
![Neues Formular Erstellen](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/new_form.jpg)
Mit "Settings" öffnet sich das Forms Menü. Dort kann man per Drag & Drop eigene Formulare erstellen, verschieben und Logik einprogrammieren. Das Beispielformular gibt schon die wichtigsten Hinweise, wie das Tool funktioniert. Es gibt Einfabefelder, in denen der Nutzer Werte einträgt. Ein Ergebnis wird in dem Feld "Calculated Field" errechnet. Die Logik dazu findet sich unter "Set Equation", nachdem man das Feld markiert hat. Um z.B. das Quadrat des Eingabewertes zu Berechnen, geben wir dort fieldname2*fieldname2 ein.
