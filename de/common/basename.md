---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/de/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Entfernt führende Verzeichniskomponenten in einem Pfad.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/basename>.

#### Ermittle den Dateinamen in einem Pfad:
```shell
basename {{pfad/zu/datei}}
```
#### Ermittle den rechtesten Verzeichnisnamen in einem Pfad:
```shell
basename {{pfad/zu/verzeichnis/}}
```
#### Ermittle den Dateinamen in einem Pfad und entferne den angegebenen Suffix aus diesem:
```shell
basename {{pfad/zu/datei}} {{suffix}}
```
{% endraw %}