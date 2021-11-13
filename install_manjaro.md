# Installing Manjaro alongside Windows 10

Christian Grubmüller, 13.11.2021

#### Herrunterladen und USB-Stick erstellen

.iso-Datei von https://manjaro.org/download/ herrunterladen und mit Wind32DiskImager auf einen USB-Stick spielen.

#### Speicherplatz frei machen

Dann verkleinert man eine Partition auf der Festplatte, auf der man Manjaro installieren will. (ungeführ 50GB sollten reichen ich hab 300GB verwendet)

#### Festplatten-Modus umstellen

Falls die Festplatte im BIOS nicht auf AHIC gestellt, ist muss man das im BIOS umstellen. Es wird empfohlen davor den Sicherheits-Modus in Windows 10 einzuschalten und danach auszuschalten, aber ich weiß nicht wieso. Bei mir war die Festplatte auf *RAID ON* gestellt und deshalb wurde sie nicht im Manjaro-Installer erkannt. (Das Problem tritt auch bei Ubuntu Systemen auf.)

#### Mit USB-Stick booten und testen

Dann bootet man vom USB-Stick aus und kann Manjaro testen. Wenn man mag was man sieht, kann man auf *install manjaro* drücken und stellt alles nach belieben ein.

#### Installieren

Wenn man aussuchen muss wo man Manjaro installiert, muss man *manual partitioning* auswählen und wählt im Dropdown-Menu oben die richtige Festplatte aus.

Dann kann man im nächsten Schritt die notwendigen Partitionen für Manjaro erstellen.

##### Boot Parition

Die Boot Parition braucht das Filesystem `fat32`, der mounting point muss auf `/boot/efi` gesetzt sein und man muss die Flags `boot` und `bios-grub` auswählen und auf *ok* drücken. Die Größe dieser Parition sollte ungefähr 300MB sein (ich hab 500MB genommen).

##### Swap Partition

Die Swap Parition wird verwendet, wenn der ganze Arbeitsspeicher beansprucht wird, allerdings noch mehr benötigt wird. Dazu wählt man wieder den *free space* aus und erstellt eine neue Partition. Dort wählt man ungefähr die Hälfte des momentanen echten Arbeitsspeicher aus, wählt das Filesystem `linuxswap` und drückt auf ok.

##### 'normale' Partition

Für die normale Parition wählt man den rest des freien Speicherplatzes aus. Das Filesystem habe ich auf `ext4` gesetzt und den *mount point* auf `/`. Dann hab ich auf *ok* gedrückt.

Anschließend muss man einfach immer auf *next* drücken, bis die Installation startet. Die Installation an sich sollte nicht länger als ein paar Minuten dauern.

