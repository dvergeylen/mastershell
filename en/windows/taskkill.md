---
layout: default
title: "taskkill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="taskkill">
  <a href="/en/windows/taskkill.html">taskkill</a> <a href="#taskkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminate a process by its process id or name.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/taskkill>.

#### Terminate a process by its id:
```shell
taskkill /pid {{process_id}}
```
#### Terminate a process by its name:
```shell
taskkill /im {{process_name}}
```
#### Forcefully terminate a specified process:
```shell
taskkill /pid {{process_id}} /f
```
#### Terminate a process and its child processes:
```shell
taskkill /im {{process_name}} /t
```
#### Terminate a process on a remote machine:
```shell
taskkill /pid {{process_id}} /s {{remote_name}}
```
#### Display information about the usage of the command:
```shell
taskkill /?
```
{% endraw %}