---
layout: default
title: "asr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asr">
  <a href="/it/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ripristina (copia) un'immagine disco dentro a un volume.
> Il nome del comando sta per Apple Software Restore (software di ripristino Apple).

#### Ripristina un'immagine disco su un volume specifico:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}}
```
#### Distruggi il volume specifico prima di ripristinare:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}} --erase
```
#### Salta la verifica dopo il ripristino:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}} --noverify
```
#### Clona i volumi senza utilizzare un'immagine disco intermedia:
```shell
sudo asr restore --source {{percorso/del/volume}} --target {{percorso/del/volume/clonato}}
```
{% endraw %}