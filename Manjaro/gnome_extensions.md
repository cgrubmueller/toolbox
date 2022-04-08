# gnome-extensions

Christian Grubmüller, 15.11.2021

### Extensions an sich

Generell kann man viele Extensions für Gnome verwenden. Am besten kann man diese mit https://extensions.gnome.org/ und der entsprechenden Browserextension herrunterladen/installieren. Offline kann man die gnome-extensions mit dem Programm *Extensions* verwalten.

Wenn man die Extensions über Firefox herunterlädt muss man ein Programm im Packetmanager herunterladen. Das sollte man sofort nach dem installieren der extensions wieder deinstallieren, weil sonst wird Firefox extrem langsam!!!

#### Enable

```bash
gsettings set org.gnome.shell disable-user-extensions false
```

#### Disable

```bash
gsettings set org.gnome.shell disable-user-extensions true
```

#### Sound Indicator switch

Um schnell und konfortabel zwischen *Build-In Audio* und *Headset* wechseln zu können, kann man diese Extension verwenden. [sound-output-device-chooser](https://extensions.gnome.org/extension/906/sound-output-device-chooser/)

Hier zu muss man einfach auf den Link drücken und anschließend den *Toggle-Button* auf ***On*** setzen

