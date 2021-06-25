---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/de/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Docker Container und Images.
> Weitere Informationen: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Liste zur Zeit laufende Container auf:
```shell
docker ps
```
#### Liste laufende und gestoppte Container auf:
```shell
docker ps -a
```
#### Erzeuge einen Container aus einem Image und benenne ihn:
```shell
docker run --name {{container_name}} {{pfad/zu/image}}
```
#### Stoppe oder starte einen existierenden Container:
```shell
docker {{start|stop}} {{container_name}}
```
#### Lade ein Image herunter:
```shell
docker pull {{pfad/zu/image}}
```
#### Öffne eine Konsole innerhalb eines bereits laufenden Containers:
```shell
docker exec -it {{container_name}} {{sh}}
```
#### Lösche einen gestoppten Container:
```shell
docker rm {{container_name}}
```
#### Zeige die Logs eines Containers an und aktualisiere sie automatisch:
```shell
docker logs -f {{container_name}}
```
{% endraw %}