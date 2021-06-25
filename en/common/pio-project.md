---
layout: default
title: "pio project"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-project">
  <a href="/en/common/pio-project.html">pio project</a> <a href="#pio-project"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manage PlatformIO projects.
> More information: <https://docs.platformio.org/en/latest/core/userguide/project/>.

#### Initialize a new PlatformIO project:
```shell
pio project init
```
#### Initialize a new PlatformIO project in a specific directory:
```shell
pio project init --project-dir {{path/to/project_directory}}
```
#### Initialize a new PlatformIO project, specifying a board ID:
```shell
pio project init --board {{ATmega328P|uno|...}}
```
#### Initialize a new PlatformIO based project, specifying one or more project options:
```shell
pio project init --project-option="{{option}}={{value}}" --project-option="{{option}}={{value}}"
```
#### Print the configuration of a project:
```shell
pio project config
```
{% endraw %}