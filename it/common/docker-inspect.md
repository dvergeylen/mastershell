---
layout: default
title: "docker inspect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-inspect">
  <a href="/it/common/docker-inspect.html">docker inspect</a> <a href="#docker-inspect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra informazioni a basso livello di oggetti Docker.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/inspect/>.

#### Mostra aiuto:
```shell
docker inspect
```
#### Mostra informazioni su un container, immagine o volume usando un nome o un identificativo (ID):
```shell
docker inspect {{nome_container|nome_immagine|ID}}
```
#### Mostra l'indirizzo IP di un container:
```shell
docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{nome_container}}
```
#### Mostra il percorso dei file di log di un container:
```shell
docker inspect --format='{{.LogPath}}' {{nome_container}}
```
#### Mostra il nome dell'immagine di un container:
```shell
docker inspect --format='{{.Config.Image}}' {{nome_container}}
```
#### Mostra le informazioni di configurazione in formato JSON:
```shell
docker inspect --format='{{json .Config}}' {{nome_container}}
```
#### Mostra il binding di tutte le porte:
```shell
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{nome_container}}
```
{% endraw %}