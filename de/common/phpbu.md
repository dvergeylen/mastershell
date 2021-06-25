---
layout: default
title: "phpbu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpbu">
  <a href="/de/common/phpbu.html">phpbu</a> <a href="#phpbu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Backup framework für PHP.
> Weitere Informationen: <https://phpbu.de>.

#### Führe ein Backup mit der Standard `phpbu.xml` Konfigurationsdatei aus:
```shell
phpbu
```
#### Führe ein Backup mit einer bestimmten Konfigurationsdatei aus:
```shell
phpbu --configuration={{pfad/zu/konfiguration.xml}}
```
#### Führe nur die angegebenen Backups aus:
```shell
phpbu --limit={{backup_art}}
```
#### Simuliere Aktionen die ausgeführt werden würden:
```shell
phpbu --simulate
```
{% endraw %}