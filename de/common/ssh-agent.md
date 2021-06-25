---
layout: default
title: "ssh-agent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-agent">
  <a href="/de/common/ssh-agent.html">ssh-agent</a> <a href="#ssh-agent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle einen SSH Agenten-Prozess.
> Ein SSH Agent behält die hinzugefügten SSH Schlüssel solange verschlüsselt im Arbeitsspeicher, bis diese entfernt werden oder der Agenten-Prozess beendet wird.
> Siehe auch `ssh-add`, um Schlüssel zu verwalten.

#### Starte einen SSH Agenten-Prozesses für die aktuelle Shell:
```shell
eval $(ssh-agent)
```
#### Beende den aktuell laufenden SSH Agenten-Prozesses:
```shell
ssh-agent -k
```
{% endraw %}