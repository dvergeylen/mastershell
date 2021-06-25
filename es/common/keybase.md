---
layout: default
title: "keybase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="keybase">
  <a href="/es/common/keybase.html">keybase</a> <a href="#keybase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Directorio de claves que conecta identidades en redes sociales a claves encriptadas de una manera públicamente auditable.
> Más información: <https://keybase.io/docs/command_line>.

#### Sigue a otro usuario:
```shell
keybase follow {{nombre_de_usuario}}
```
#### Añade una nueva prueba:
```shell
keybase prove {{servicio}} {{nombre_de_usuario_en_el_servicio}}
```
#### Firma un archivo:
```shell
keybase sign --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Verifica un archivo firmado:
```shell
keybase verify --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Encripta un archivo:
```shell
keybase encrypt --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}} {{receptor}}
```
#### Desencripta un archivo:
```shell
keybase decrypt --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Revoca el dispositivo actual, se desconecta y borra los datos locales:
```shell
keybase deprovision
```
{% endraw %}