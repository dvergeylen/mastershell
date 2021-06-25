---
layout: default
title: "arduino-builder"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arduino-builder">
  <a href="/pt_br/common/arduino-builder.html">arduino-builder</a> <a href="#arduino-builder"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uma ferramenta de linha de comando para compilar sketches do arduino.
> AVIDO DE OBSOLESCÊNCIA: Esta ferramenta está sendo descontinuada e substituida pelo `arduino`.
> Mais informações: <https://github.com/arduino/arduino-builder>.

#### Compilar um sketch:
```shell
arduino-builder -compile {{caminho/para/sketch.ino}}
```
#### Definir o nível de debug (1 a 10, o padrão é 5):
```shell
arduino-builder -debug-level {{nivel}}
```
#### Definir um diretório de compilação customizado:
```shell
arduino-builder -build-path {{caminho/para/diretorio}}
```
#### Usar um arquivo com as opções de compilação, em vez de especificar `--hardware`, `--tools`, etc. manualmente toda hora:
```shell
arduino-builder -build-options-file {{caminho/para/build.options.json}}
```
#### Habilitar o modo verboso:
```shell
arduino-builder -verbose {{true}}
```
{% endraw %}