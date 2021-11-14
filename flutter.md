# Flutter installieren auf Manjaro

Christian Grubmüller, 14.11.2021

#### Flutter an sich installieren

Mit folgendem Befehl kann man flutter an sich und die Dart SDK installieren.

```bash
sudo snap install flutter --classic
```

#### Intellij Ultimate installieren

Um IntelliJ zu installieren kann man *snap* verwenden.

```bash
sudo snap install intellij-idea-ultimate --classic
```

#### AndroidSDK installieren 

Die AndroidSDK installiert man am am Besten über IntelliJ. Dazu muss man in `File>Settings>Appearance & Behavior>Andorid SDK` die AndroidSDK herrunterladen. Diese wird in Manjaro unter `/home/christian/Android/Sdk` abgespeichert. Diesen Pfad muss man dann auch noch für Flutter setzten. Das kann man mit folgendem Befehl machen.

```bash
flutter config --android-sdk /home/christian/Andorid/Sdk
```

#### Chrome installieren

Chrome kann man über das AUR (Arch User Repository) herrunterladen und installieren. Das kann man mit dem Packetmanagement *yay* erledigen. Wie man yay installiert findet man [hier](./yay.md).

