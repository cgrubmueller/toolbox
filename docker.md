# Docker

Christian Grubmüller, 23.11.2021

## Installieren

Sollte man eigentlich mit yay machen. `docker-compose` funktioniert beispielsweise nicht wenn man es über snap installiert.

```shell
sudo snap install docker
```

## Docker Daemon starten

Bevor man Docker verwenden kann, muss man den Daemon starten. Man könnte ihn auch standardmäßig beim start des Computer laufen lassen, aber das ist nicht empfolen.

```bash
sudo systemctl start docker
```





## Docker ohne sudo

```bash
# falls die Docker-Gruppe noch nicht existiert
sudo groupadd docker
# momentanen User zur Docker-Gruppe hinzufügen
sudo gpasswd -a $USER docker
# testen
docker run hello-world
```

## Contianer anzeigen

```bash
# running Container
docker ps
# alle Contianer 
docker ps -a
```

## Image builden

Der Punk `.` ist das aktuelle Verzeichnis (mit `Dockerfile`). (Kann auch was anderes sein)

```bash
docker build --tag <name> .
```

## Image runnen

```bash
docker run --name rest -p <host-port>:<container-port> <name>
```

## Images anzeigen

```bash
docker images
```

## Images löschen

```bash
# Alle Images löschen
docker image prune
# Einzelnes Image Löschen
docker rmi <id>
# Einzelnes Image löschen (forcen)
docker rmi -f <id>
```

## IP von Containern

```bash
# Neue Syntax
docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <container_name_or_id>
# Alte Syntax
docker inspect --format '{{ .NetworkSettings.IPAddress }}' container_name_or_id
```

[Quelle](https://stackoverflow.com/questions/17157721/how-to-get-a-docker-containers-ip-address-from-the-host)

## Logs

```bash
docker logs <container id>
```

