---
layout: default
title: "arduino"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arduino">
  <a href="/pt_br/common/arduino.html">arduino</a> <a href="#arduino"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arduino Studio - Ambiente de Desenvolvimento Integrado para a plataforma Arduino.
> Mais informações: <https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc>.

#### Compilar um sketch:
```shell
arduino --verify {{caminho/para/arquivo.ino}}
```
#### Compilar e enviar sketch:
```shell
arduino --upload {{caminho/para/arquivo.ino}}
```
#### Compilar e enviar sketch para um Arduino Nano com uma CPU Atmega328p, conectada na porta `/dev/ttyACM0`:
```shell
arduino --board {{arduino:avr:nano:cpu=atmega328p}} --port {{/dev/ttyACM0}} --upload {{caminho/para/arquivo.ino}}
```
#### Definir a preferência `nome` para um determinado `valor`:
```shell
arduino --pref {{nome}}={{valor}}
```
#### Compilar um sketch, colocar o resultado da compilação no diretório de compilação, e reutilizar qualquer resultado pre-existente neste diretório:
```shell
arduino --pref build.path={{caminho/para/diretório}} --verify {{caminho/para/arquivo.ino}}
```
#### Salvar todas as preferências (alteradas) para `preferences.txt`:
```shell
arduino --save-prefs
```
{% endraw %}