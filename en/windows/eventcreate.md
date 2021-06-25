---
layout: default
title: "eventcreate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eventcreate">
  <a href="/en/windows/eventcreate.html">eventcreate</a> <a href="#eventcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create custom entries in the event log.
> Event IDs can be any number between 1 and 1000.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/eventcreate>.

#### Create a new event with a given id (1-1000) in the log:
```shell
eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{message}}"
```
#### Create an event in a specific event log:
```shell
eventcreate /l {{log_name}} /t {{type}} /id {{id}} /d "{{message}}"
```
#### Create an event with a specific source:
```shell
eventcreate /so {{source_name}} /t {{type}} /id {{id}} /d "{{message}}"
```
#### Create an event in a remote machine's event log:
```shell
eventcreate /s {{hostname}} /u {{username}} /p {{password}} /t {{type}} /id {{id}} /d "{{message}}"
```
{% endraw %}