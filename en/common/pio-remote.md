---
layout: default
title: "pio remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-remote">
  <a href="/en/common/pio-remote.html">pio remote</a> <a href="#pio-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helper command for PlatformIO Remote Development.
> `pio remote [command]` takes the same arguments as its locally executing counterpart `pio [command]`.
> More information: <https://docs.platformio.org/en/latest/core/userguide/remote/index.html>.

#### List all active Remote Agents:
```shell
pio remote agent list
```
#### Start a new Remote Agent with a specific name and share it with friends:
```shell
pio remote agent start --name {{agent_name}} --share {{example1@example.com}} --share {{example2@example.com}}
```
#### List devices from specified Agents (omit `--agent` to specify all Agents):
```shell
pio remote --agent {{agent_name1}} --agent {{agent_name2}} device list
```
#### Connect to the serial port of a remote device:
```shell
pio remote --agent {{agent_name}} device monitor
```
#### Run all targets on a specified Agent:
```shell
pio remote --agent {{agent_name}} run
```
#### Update installed core packages, development platforms and global libraries on a specific Agent:
```shell
pio remote --agent {{agent_name}} update
```
#### Run all tests in all environments on a specific Agent:
```shell
pio remote --agent {{agent_name}} test
```
{% endraw %}