---
layout: default
title: "dvc config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-config">
  <a href="/en/common/dvc-config.html">dvc config</a> <a href="#dvc-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Low level command to manage custom configuration options for dvc repositories.
> These configurations can be on project, local, global, or system level.
> More information: <https://dvc.org/doc/command-reference/config>.

#### Get the name of the default remote:
```shell
dvc config core.remote
```
#### Set the project's default remote:
```shell
dvc config core.remote {{remote_name}}
```
#### Unset the project's default remote:
```shell
dvc config --unset core.remote
```
#### Get the config value for a specified key for the current project:
```shell
dvc config {{key}}
```
#### Set the config value for a key on a project level:
```shell
dvc config {{key}} {{value}}
```
#### Unset a project level config value for a given key:
```shell
dvc config --unset {{key}}
```
#### Set a local, global, or system level config value:
```shell
dvc config --local/global/system {{key}} {{value}}
```
{% endraw %}