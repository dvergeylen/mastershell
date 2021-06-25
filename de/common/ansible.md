---
layout: default
title: "ansible"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible">
  <a href="/de/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Computergruppen per Fernzugriff über SSH.
> Verwende die Datei `/etc/ansible/hosts`, um neue Gruppen/Hosts hinzuzufügen.
> Weitere Informationen: <https://www.ansible.com/>.

#### Liste Hosts auf, die zu einer Gruppe gehören:
```shell
ansible {{gruppe}} --list-hosts
```
#### Pinge eine Gruppe von Hosts an:
```shell
ansible {{gruppe}} -m ping
```
#### Zeige Informationen über eine Gruppe von Hosts an:
```shell
ansible {{gruppe}} -m setup
```
#### Führe einen Befehl auf einer Gruppe von Hosts aus:
```shell
ansible {{gruppe}} -m command -a '{{befehl}}'
```
#### Führe einen Befehl mit administrativen Privilegien aus:
```shell
ansible {{gruppe}} --become --ask-become-pass -m command -a '{{befehl}}'
```
#### Führe einen Befehl mit einer benutzerdefinierten Inventardatei aus:
```shell
ansible {{Gruppe}} -i {{inventardatei}} -m command -a '{{befehl}}'
```
#### Liste alle Gruppen eines Inventars auf:
```shell
ansible localhost -m debug -a '{{var=groups.keys()}}'
```
{% endraw %}