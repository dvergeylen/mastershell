---
layout: default
title: "tee"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tee">
  <a href="/es/common/tee.html">tee</a> <a href="#tee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lee desde la entrada estándar y escribe a la salida estándar a la vez que a archivos o comandos.
> Más información: <https://www.gnu.org/software/coreutils/tee>

#### Copia la entrada estándar al archivo, reemplazando su contenido, y también a la salida estándar:
```shell
echo {{ejemplo}} | tee {{ruta/al/archivo}}
```
#### Anexa la entrada estándar al archivo, sin reemplazar:
```shell
echo {{ejemplo}} | tee -a {{ruta/al/archivo}}
```
#### Imprime la entrada estándar a la terminal, y también lo reenvía a otro programa para posterior procesamiento:
```shell
echo {{ejemplo}} | tee {{/dev/tty}} | {{xargs printf "[%s]"}}
```
{% endraw %}