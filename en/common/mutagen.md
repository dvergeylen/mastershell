---
layout: default
title: "mutagen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mutagen">
  <a href="/en/common/mutagen.html">mutagen</a> <a href="#mutagen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Real-time file synchronization and network forwarding tool.
> More information: <https://mutagen.io>.

#### Start a synchronization session between a local directory and a remote host:
```shell
mutagen sync create --name={{session_name}} {{/path/to/local/directory/}} {{user}}@{{host}}:{{/path/to/remote/directory/}}
```
#### Start a synchronization session between a local directory and a Docker container:
```shell
mutagen sync create --name={{session_name}} {{/path/to/local/directory/}} docker://{{user}}@{{container_name}}{{/path/to/remote/directory/}}
```
#### Stop a running session:
```shell
mutagen sync terminate {{session_name}}
```
#### Start a project:
```shell
mutagen project start
```
#### Stop a project:
```shell
mutagen project terminate
```
#### List running sessions for the current project:
```shell
mutagen project list
```
{% endraw %}