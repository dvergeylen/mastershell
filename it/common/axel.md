---
layout: default
title: "axel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="axel">
  <a href="/it/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Downloader accelerato.
> Supporta HTTP, HTTPS e FTP.
> Maggiori informazioni: <https://github.com/axel-download-accelerator/axel>.

#### Scarica un file da un URL:
```shell
axel {{url}}
```
#### Scarica specificando il nome del file da creare:
```shell
axel {{url}} -o {{filename}}
```
#### Scarica sfruttando connessioni multiple:
```shell
axel -n {{numero_connessioni}} {{url}}
```
#### Cerca dei mirror:
```shell
axel -S {{numero_mirror}} {{url}}
```
#### Limita la velocità di download (in bytes al secondo):
```shell
axel -s {{limite_velocità}} {{url}}
```
{% endraw %}