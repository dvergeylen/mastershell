---
layout: default
title: "ansible"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible">
  <a href="/fr/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestionnaire de groupes d'ordinateurs à distance depuis SSH.
> Utiliser le fichier `/etc/ansible/hosts` pour ajouter de nouveaux groupes/hôtes.
> Plus d'informations : <https://www.ansible.com>.

#### Lister les hôtes appartenant à un groupe :
```shell
ansible {{groupe}} --list-hosts
```
#### Ping d'un groupe d'hôtes en invoquant le [m]odule "ping" :
```shell
ansible {{groupe}} -m ping
```
#### Afficher des informations sur un groupe d'hôtes en invoquant le [m]odule "setup" :
```shell
ansible {{groupe}} -m setup
```
#### Exécuter une commande sur un groupe d'hôtes en invoquant le [m]odule "command" avec en paramètre (a) cette commande :
```shell
ansible {{groupe}} -m command -a '{{ma_commande}}'
```
#### Exécuter une commande avec des droits administrateur :
```shell
ansible {{groupe}} --become --ask-become-pass -m command -a '{{ma_commande}}'
```
#### Exécuter une commande en utilisant un fichier d'inventaire personnalisé :
```shell
ansible {{groupe}} -i {{fichier_d'inventaire}} -m command -a '{{ma_commande}}'
```
#### Lister les groupes d'un inventaire :
```shell
ansible localhost -m debug -a '{{var=groups.keys()}}'
```
{% endraw %}