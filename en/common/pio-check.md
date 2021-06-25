---
layout: default
title: "pio check"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-check">
  <a href="/en/common/pio-check.html">pio check</a> <a href="#pio-check"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform a static analysis check on a PlatformIO project.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_check.html>.

#### Perform a basic analysis check on the current project:
```shell
pio check
```
#### Perform a basic analysis check on a specific project:
```shell
pio check --project-dir {{project_dir}}
```
#### Perform an analysis check for a specific environment:
```shell
pio check --environment {{environment}}
```
#### Perform an analysis check and only report a specified defect severity type:
```shell
pio check --severity {{low|medium|high}}
```
#### Perform an analysis check and show detailed information when processing environments:
```shell
pio check --verbose
```
{% endraw %}