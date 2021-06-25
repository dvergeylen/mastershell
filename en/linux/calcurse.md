---
layout: default
title: "calcurse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calcurse">
  <a href="/en/linux/calcurse.html">calcurse</a> <a href="#calcurse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based calendar and scheduling application for the command-line.
> More information: <https://calcurse.org>.

#### Start calcurse on interactive mode:
```shell
calcurse
```
#### Print the appointments and events for the current day and exit:
```shell
calcurse --appointment
```
#### Remove all local calcurse items and import remote objects:
```shell
calcurse-caldav --init=keep-remote
```
#### Remove all remote objects and push local calcurse items:
```shell
calcurse-caldav --init=keep-local
```
#### Copy local objects to the CalDAV server and vice versa:
```shell
calcurse-caldav --init=two-way
```
{% endraw %}