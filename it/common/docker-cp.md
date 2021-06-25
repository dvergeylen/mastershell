---
layout: default
title: "docker cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-cp">
  <a href="/it/common/docker-cp.html">docker cp</a> <a href="#docker-cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia file o directory tra il filesystem di un container e quello locale (host).
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/cp>.

#### Copia un file o una directory dall'host a un container:
```shell
docker cp {{percorso/al/file_o_directory_su_host}} {{nome_container}}:{{percorso/al/file_o_directory_su_container}}
```
#### Copia un file o una directory da un container all'host:
```shell
docker cp {{nome_container}}:{{percorso/al/file_o_directory_su_container}} {{percorso/al/file_o_directory_su_host}}
```
#### Copia un file o una directory dall'host a un container, seguendo un link simbolico (non copiare il link simbolico, ma direttamente il file da lui referenziato):
```shell
docker cp --follow-link {{percorso/al/link_simbolico_su_host}} {{nome_container}}:{{percorso/al/file_o_directory_su_container}}
```
{% endraw %}