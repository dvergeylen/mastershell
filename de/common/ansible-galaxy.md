---
layout: default
title: "ansible-galaxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-galaxy">
  <a href="/de/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mögliche Rollen erstellen und verwalten.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### Installiere eine Rolle:
```shell
ansible-galaxy install {{benutzername.rollenname}}
```
#### Entferne eine Rolle:
```shell
ansible-galaxy remove {{benutzername.rollenname}}
```
#### Installierte Rollen auflisten:
```shell
ansible-galaxy list
```
#### Suche nach einer bestimmten Rolle:
```shell
ansible-galaxy search {{rollenname}}
```
#### Erstelle eine neue Rolle:
```shell
ansible-galaxy init {{rollenname}}
```
{% endraw %}