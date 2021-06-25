---
layout: default
title: "ansible-galaxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-galaxy">
  <a href="/it/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea e gestisci ruoli di Ansible.
> Maggiori informazioni: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### Installa un ruolo:
```shell
ansible-galaxy install {{utente.ruolo}}
```
#### Rimuovi un ruolo:
```shell
ansible-galaxy remove {{utente.ruolo}}
```
#### Elenca i ruoli installati:
```shell
ansible-galaxy list
```
#### Cerca un determinato ruolo:
```shell
ansible-galaxy search {{nome_ruolo}}
```
#### Crea un nuovo ruolo:
```shell
ansible-galaxy init {{nome_nuovo_ruolo}}
```
{% endraw %}