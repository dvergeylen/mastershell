---
layout: default
title: "pio debug"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-debug">
  <a href="/en/common/pio-debug.html">pio debug</a> <a href="#pio-debug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debug PlatformIO projects.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_debug.html>.

#### Debug the PlatformIO project in the current directory:
```shell
pio debug
```
#### Debug a specific PlatformIO project:
```shell
pio debug --project-dir {{path/to/platformio_project}}
```
#### Debug a specific environment:
```shell
pio debug --environment {{environment}}
```
#### Debug a PlatformIO project using a specific configuration file:
```shell
pio debug --project-conf {{path/to/platformio.ini}}
```
#### Debug a PlatformIO project using the `gdb` debugger:
```shell
pio debug --interface={{gdb}} {{gdb_options}}
```
{% endraw %}