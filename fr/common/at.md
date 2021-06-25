---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/fr/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Planifie l'exécution d'une commande une fois à un moment donné.
> Le service atd (ou atrun) doit être actif pour l'exécution des commandes planifiées.
> Plus d'informations : <https://man.archlinux.org/man/at.1>.

#### Planifie l'exécution de la commande donnée dans l'entrée standard dans 5 minutes (Appuyer sur `Ctrl + D` une fois la commande inscrite) :
```shell
at now + 5 minutes
```
#### Planifie l'exécution d'une commande depuis l'entrée standard (impression echo redirigée dans un tube) aujourd'hui à 10h00 :
```shell
echo "{{./ma_commande.sh}}" | at 1000
```
#### Planifie l'exécution des commandes inclues dans un [f]ichier pour mardi prochain 21h30 :
```shell
at -f {{chemin/vers/fichier}} 9:30 PM Tue
```
{% endraw %}