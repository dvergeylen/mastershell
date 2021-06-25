---
layout: default
title: "ssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh">
  <a href="/fr/common/ssh.html">ssh</a> <a href="#ssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure Shell est un protocole utilisé pour se connecter de façon sécurisée à des systèmes distants.
> On peut l'utiliser pour se connecter ou exécuter des commandes sur un serveur distant.

#### Se connecter à un serveur distant :
```shell
ssh {{utilisateur}}@{{hote_distant}}
```
#### Se connecter à un serveur distant en utilisant une identité spécifique (clé privée) :
```shell
ssh -i {{chemin/vers/fichier_clef}} {{utilisateur}}@{{hote_distant}}
```
#### Se connecter à un serveur distant en utilisant un port spécifique :
```shell
ssh {{utilisateur}}@{{hote_distant}} -p {{2222}}
```
#### Exécuter une commande sur un serveur distant :
```shell
ssh {{hote_distant}} {{commande -avec -options}}
```
#### Tunnel SSH : Transfert par port dynamique (le SOCKS proxy se trouve sur localhost:1080) :
```shell
ssh -D {{1080}} {{utilisateur}}@{{hote_distant}}
```
#### Tunnel SSH : Transfère un port spécifique (localhost:9999 vers example.org:80) en désactivant l'allocation de pseudo-[t]ty et l'exécution de commandes distantes :
```shell
ssh -L {{9999}}:{{exemple.org}}:{{80}} -N -T {{utilisateur}}@{{hote_distant}}
```
#### Saut SSH : Se connecter sur un serveur distant à travers une machine de rebond (plusieurs machines de rebond peuvent être définies en les séparant par des virgules) :
```shell
ssh -J {{utilisateur}}@{{hote_de_rebond}} {{utilisateur}}@{{hote_distant}}
```
#### Transfert d'agent : Transfère les informations d'authentification vers la machine distante (voir `man ssh_config` pour les options disponibles) :
```shell
ssh -A {{utilisateur}}@{{hote_distant}}
```
{% endraw %}