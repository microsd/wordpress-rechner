# wordpress-rechner
Einfachen Online-Rechner für Wordpress erstellen. [Website](http://microsd.github.io/wordpress-rechner/)

Diese Anleitung erklärt, wie man in Wordpress einen einfachen Online-Rechner erstellen kann. Ein solcher Rechner ist Beispielhaft auf der Seite http://www.micro-sd.net/kapazitaetsrechner/ zu sehen. Es gibt dort mehrere Eingabefelder, aus denen der Benutzer die umzurechnenden Größen bestimmt. Das Ausgabefeld wird automatisch aus den Eingaben errechnet. Das Tool führt dabei eine Syntaxprüfung durch und es wird die deutsche Schreibweise mit Komma als Dezimaltrennzeichen sowie Punkt zur 1.000er Gruppierung verwendet. Es wird eine funktionierende Wordpress-Installation vorausgesetzt.
Für einfache Online-Rechner eignet sich das kostenlose Plugin [Calculated Fields Form](https://wordpress.org/plugins/calculated-fields-form/):
![Plugin installieren](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/calculated_fields_form.jpg)
Nach dem Installieren und Aktivieren bitte auf Plugins->Installierte Plugins->Calculated Fields Form->Einstellungen Klicken. Dann unter "New Form" einen Namen eintragen und ein neues Formular erstellen:
![Neues Formular Erstellen](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/new_form.jpg)
Mit "Settings" öffnet sich das Forms Menü. Dort kann man per Drag & Drop eigene Formulare erstellen, verschieben und Logik einprogrammieren. Das Beispielformular gibt schon die wichtigsten Hinweise, wie das Tool funktioniert. Es gibt Einfabefelder, in denen der Nutzer Werte einträgt. Ein Ergebnis wird in dem Feld "Calculated Field" errechnet. Die Logik dazu findet sich unter "Set Equation", nachdem man das Feld markiert hat. Um z.B. das Quadrat des Eingabewertes zu Berechnen, geben wir dort fieldname2*fieldname2 ein.
![Formel eingeben](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/calculated_field.jpg)
Nun haben wir bereits und funktionierendes Formulat. Mittels "Save&Preview" können wir uns es anschauen. Was jetzt noch fehlt sind die deutschen Einstellungen für das Zahlenformat:
![Deutsche Einstellungen Zahlenformat](https://raw.githubusercontent.com/microsd/wordpress-rechner/master/images/german_settings.jpg)
Bei Number-Format bitte "number" auswählen. Bei "Decimals seperator symbol" ein Komme "," eingeben, bei Symbol for grouping thousands einen Punkt "." eingeben. Nun werden die Zahlen im deutschen Format dargestellt. Letztes Finetuning sind nun die Settings unten auf der Seite "Validation Settings". Dort können die englischsprachigen Fehlermeldungen bei falscher Benutzereingabe auf Deutsch manuell übersetzt werden. 
(http://www.oszilloskope.net)
