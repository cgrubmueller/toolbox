# Display Manager

Christian Grubmüller, 30.11.2021

Wie ich Manjaro neu installiert habe, habe ich *wayland* Displaymanager gehabt. Das kann man mit `inxi -G` nachschauen. Wie ich *wayland* verwendet habe, hat screensharing grunstäzlich eher nicht funktioniert. Irgendwie hab ich es fensterweise mit Teams in Chrome zum Laufen bringen können, aber nicht wirklich gut.



## Wayland

Wayland ist ein neuerer Display Manager für *Gnome*. Grundsätzlich wird das Screensharing vom ganzen Screen (noch) nicht unterstützt. Angeblich soll es irgenwelche Tools (pipewire) geben, mit denen man es zum laufen bringen könnte, aber das war mir zu mühsam.



## X11 

Ist ein älterer Displaymanager, der schon sehr gut getestet ist. Wie gesagt ist er allerdings alt und das merkt man manchmal. Das ist aber nicht wirklich störend. Wichtig war für mich, dass das Screensharing funtkioniert hat.



## Wechseln

Wenn ich zwischen Wayland und X11 wechseln will, muss ich meinen Rechner **herunterfahren**. Wenn ich mich dann neueinloggen will und meinen User aussuche, kann ich unten rechts bei dem Zahnrad verschiedenen "Gnome-Arten" auswählen. Diese Auswahl bestimmt dann ob ich Wayland oder X11 verwende.

