---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/de/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Führe einen Befehl oder eine interaktive Shell mit einem speziellen root-Verzeichnis aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chroot>.

#### Führe einen Befehl mit einem neuen root-Verzeichnis aus:
```shell
chroot {{pfad/zu/root_verzeichnis}} {{befehl}}
```
#### Lege einen Benutzer und eine Gruppe (ID oder Name) fest, der benutzt werden soll:
```shell
chroot --userspec={{benutzer:gruppe}}
```
{% endraw %}