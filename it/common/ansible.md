---
layout: default
title: "ansible"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible">
  <a href="/it/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci gruppi di computer da remoto via SSH.
> Usa il file `/etc/ansible/hosts` per aggiungere nuovi gruppi/host.
> Maggiori informazioni: <https://www.ansible.com/>.

#### Lista gli host appartenenti ad un gruppo:
```shell
ansible {{gruppo}} --list-hosts
```
#### Invia un ping ad un gruppo di host invocando il modulo "ping":
```shell
ansible {{gruppo}} -m ping
```
#### Mostra informazioni su di un gruppo di host invocando il modulo "setup":
```shell
ansible {{gruppo}} -m setup
```
#### Esegui un comando su un gruppo di host invocando il modulo "command" con degli argomenti:
```shell
ansible {{gruppo}} -m command -a '{{comando_da_eseguire}}'
```
#### Esegui un comando con privilegi di amministratore:
```shell
ansible {{gruppo}} --become --ask-become-pass -m command -a '{{comando}}'
```
#### Esegui un comando usando un file di inventory personalizzato:
```shell
ansible {{gruppo}} -i {{file_inventory}} -m command -a '{{comando}}'
```
{% endraw %}