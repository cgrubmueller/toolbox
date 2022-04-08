# Programme

Christian Grubmüller, 21.11.2021

## Astah

Astah-uml hab ich mit dem Packagemanager herruntergeladen. Wichtig ist, dass Astah die Version 1.8 von Java benötigt. Am besten ladet man die auch im Packagemanager herrunter (*jdk8-openjdk*). Mit dem Befehl `archlinux-java` kann man seine Java Versionen managen und umändern.

```bash
archlinux-java status # zeigt alle verfügbaren Java Versionen an
archlinux-java get # zeigt die aktuell verwendete Java Version an (default)
archlinux-java set # setzt die zu verwendente Java Version 
```

## R Studio

RStudio kann man mit einem AUR-Tool (yay, yaourt,...) herrunterladen und installieren. Man muss dann aufpassen, damit man das richtige package erwischt.

Damit man dann auch alles gut knitten kann muss man sich Latex im Packagemanager herrunterladen. Ich habe die folgende Packages installieren müssen:

+ *texlive-core*
+ *texlive-latexextra*

## wxMaxima

Maxima kann man einfach über den Packagemanager herrunterladen

## weitere Programme

Mit `yay` kann man sehr viele Programme herrunterladen.

*Signal, Thunderbird, Typora, docker, flutter, etc.*

Mit `snap` kann man *Spotify* und *Teams* installieren.
