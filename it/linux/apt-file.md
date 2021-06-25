---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/it/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cerca un file dentro un pacchetto apt, includendo quelli non ancora installati.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Aggiorna il database dei metadati:
```shell
sudo apt update
```
#### Cerca i pacchetti che contengono un file o un percorso specificato:
```shell
apt-file search {{parte/del/filename}}
```
#### Elenca i contenuti di un pacchetto specifico:
```shell
apt-file list {{nome_del_pacchetto}}
```
{% endraw %}