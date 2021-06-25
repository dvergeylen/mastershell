---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/de/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Editiere die Repository-Listen.
> Weitere Informationen: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Füge ein neues Repository hinzu:
```shell
apt-add-repository {{repository_spec}}
```
#### Entferne ein Repository:
```shell
apt-add-repository --remove {{repository}}
```
#### Aktualisiere den Cache nachdem das Repository hinzugefügt wurde:
```shell
apt-add-repository --update {{repository}}
```
#### Aktiviere Source Pakete:
```shell
apt-add-repository --enable-source {{repository}}
```
{% endraw %}