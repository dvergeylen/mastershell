---
layout: default
title: "particle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="particle">
  <a href="/en/common/particle.html">particle</a> <a href="#particle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for interacting with Particle devices.
> More information: <https://docs.particle.io/tutorials/developer-tools/cli>.

#### Log in or create an account for the Particle CLI:
```shell
particle setup
```
#### Display a list of devices:
```shell
particle list
```
#### Create a new Particle project interactively:
```shell
particle project create
```
#### Compile a Particle project:
```shell
particle compile {{device_type}} {{path/to/source_code.ino}}
```
#### Update a device to use a specific app remotely:
```shell
particle flash {{device_name}} {{path/to/program.bin}}
```
#### Update a device to use the latest firmware via serial:
```shell
particle flash --serial {{path/to/firmware.bin}}
```
#### Execute a function on a device:
```shell
particle call {{device_name}} {{function_name}} {{function_arguments}}
```
{% endraw %}