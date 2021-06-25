---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/nl/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vind een gespecificieerde string in een bestand.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Vind de lijnen dat een specifieke string bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}}
```
#### Laat lijnen zie die de string niet bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /v
```
#### Toon het aantal lijnen dat de string bevat:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /c
```
#### Laat het aantal lijnen zien samen met de lijnen:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /n
```
{% endraw %}