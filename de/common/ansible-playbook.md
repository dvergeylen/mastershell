---
layout: default
title: "ansible-playbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-playbook">
  <a href="/de/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> In Playbook definierte Aufgaben auf entfernten Rechnern über SSH ausführen.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### Führe Aufgaben im Playbook aus:
```shell
ansible-playbook {{playbook}}
```
#### Führe Aufgaben im Playbook mit benutzerdefiniertem Host-Bestand aus:
```shell
ansible-playbook {{playbook}} -i {{inventory_datei}}
```
#### Führe Aufgaben im Playbook aus, wobei zusätzliche Variablen über die Befehlszeile definiert werden:
```shell
ansible-playbook {{playbook}} -e "{{variable1}}={{wert1}} {{variable2}}={{wert2}}"
```
#### Führe Aufgaben in Playbook mit zusätzlichen Variablen aus, die in einer JSON-Datei definiert sind:
```shell
ansible-playbook {{playbook}} -e "@{{variablen.json}}"
```
#### Führe Aufgaben im Playbook für die angegebenen Tags aus:
```shell
ansible-playbook {{playbook}} --tags {{tag1,tag2}}
```
#### Führe Aufgaben in einem Playbook aus, die mit einer bestimmten Aufgabe beginnen:
```shell
ansible-playbook {{playbook}} --start-at {{aufgabenname}}
```
{% endraw %}