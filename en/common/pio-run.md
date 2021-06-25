---
layout: default
title: "pio run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-run">
  <a href="/en/common/pio-run.html">pio run</a> <a href="#pio-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run PlatformIO project targets.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_run.html>.

#### List all available project targets:
```shell
pio run --list-targets
```
#### List all available project targets of a specific environment:
```shell
pio run --list-targets --environment {{environment}}
```
#### Run all targets:
```shell
pio run
```
#### Run all targets of specified environments:
```shell
pio run --environment {{environment1}} --environment {{environment2}}
```
#### Run specified targets:
```shell
pio run --target {{target1}} --target {{target2}}
```
#### Run the targets of a specified configuration file:
```shell
pio run --project-conf {{path/to/platformio.ini}}
```
{% endraw %}