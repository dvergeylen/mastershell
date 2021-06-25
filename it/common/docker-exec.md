---
layout: default
title: "docker exec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-exec">
  <a href="/it/common/docker-exec.html">docker exec</a> <a href="#docker-exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui un comando su un Docker container in esecuzione.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/exec/>.

#### Avvia una shell interattiva all'interno di un container in esecuzione:
```shell
docker exec --interactive --tty {{nome_container}} {{/bin/bash}}
```
#### Esegui un commando in background ("detached") su un container in esecuzione:
```shell
docker exec --detach {{nome_container}} {{comando}}
```
#### Seleziona la directory di lavoro in cui eseguire un dato comando:
```shell
docker exec --interactive -tty --workdir {{percorso/alla/directory}} {{nome_container}} {{comando}}
```
#### Esegui un comando in background su un container esistente, mantenendo aperto stdin:
```shell
docker exec --interactive --detach {{nome_container}} {{comando}}
```
#### Imposta una variabile d'ambiente in una sessione bash in esecuzione:
```shell
docker exec --interactive --tty --env {{nome_variabile}}={{valore}} {{nome_container}} {{/bin/bash}}
```
#### Specifica l'utente da usare per eseguire un comando:
```shell
docker exec --user {{utente}} {{nome_container}} {{comando}}
```
{% endraw %}