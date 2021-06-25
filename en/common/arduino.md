---
layout: default
title: "arduino"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arduino">
  <a href="/en/common/arduino.html">arduino</a> <a href="#arduino"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arduino Studio - Integrated Development Environment for the Arduino platform.
> More information: <https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc>.

#### Build a sketch:
```shell
arduino --verify {{path/to/file.ino}}
```
#### Build and upload a sketch:
```shell
arduino --upload {{path/to/file.ino}}
```
#### Build and upload a sketch to an Arduino Nano with an Atmega328p CPU, connected on port `/dev/ttyACM0`:
```shell
arduino --board {{arduino:avr:nano:cpu=atmega328p}} --port {{/dev/ttyACM0}} --upload {{path/to/file.ino}}
```
#### Set the preference `name` to a given `value`:
```shell
arduino --pref {{name}}={{value}}
```
#### Build a sketch, put the build results in the build directory, and reuse any previous build results in that directory:
```shell
arduino --pref build.path={{path/to/build_directory}} --verify {{path/to/file.ino}}
```
#### Save any (changed) preferences to `preferences.txt`:
```shell
arduino --save-prefs
```
{% endraw %}