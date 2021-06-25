---
layout: default
title: "apache2ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apache2ctl">
  <a href="/fr/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> L'outil d'Interface en Lignes de Commandes (ILC) pour administrer le serveur web HTTP Apache.
> Cette commande est disponible sur une distribution Debian. Pour les distributions basées Red Hat, voir `httpd`.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/apache2ctl.8.en.html>.

#### Démarre le démon Apache. Envoie un message s'il est déjà actif :
```shell
sudo apache2ctl start
```
#### Arrête le démon Apache :
```shell
sudo apache2ctl stop
```
#### Re-démarre le démon Apache :
```shell
sudo apache2ctl restart
```
#### Teste la syntaxe du fichier de configuration :
```shell
sudo apache2ctl -t
```
#### Liste les modules chargés :
```shell
sudo apache2ctl -M
```
{% endraw %}