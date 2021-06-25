---
layout: default
title: "yes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yes">
  <a href="/fr/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envoie un message à répétition en sortie console.
> Cette commande est souvent utilisée pour éviter de devoir accepter des opérations successives (par exemple des installations via la commande `apt-get`).
> Plus d'informations : <https://www.gnu.org/software/coreutils/yes>.

#### Envoyer « message » à répétition :
```shell
yes {{message}}
```
#### Envoyer « y » à répétition :
```shell
yes
```
#### Répondre « oui » à toutes les questions posées par la commande `apt-get` :
```shell
yes | sudo apt-get install {{program}}
```
{% endraw %}