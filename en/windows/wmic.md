---
layout: default
title: "wmic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wmic">
  <a href="/en/windows/wmic.html">wmic</a> <a href="#wmic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactive shell for detailed information about running processes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/wmic>.

#### Fundamental grammar:
```shell
wmic {{alias}} {{where_clause}} {{verb_clause}}
```
#### Show brief details about the currently running processes:
```shell
wmic process list brief
```
#### Show full details about the currently running processes:
```shell
wmic process list full
```
#### Access specific fields such as process name, process ID and parent process ID:
```shell
wmic process get {{name,processid,parentprocessid}}
```
#### Display information about a specific process:
```shell
wmic process where {{name="example.exe"}} list full
```
#### Display specific fields for a specific process:
```shell
wmic process where processid={{pid}} get {{name,commandline}}
```
#### Kill a process:
```shell
wmic process {{pid}} delete
```
{% endraw %}