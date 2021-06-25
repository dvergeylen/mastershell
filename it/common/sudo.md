---
layout: default
title: "sudo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sudo">
  <a href="/it/common/sudo.html">sudo</a> <a href="#sudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegue un singolo comando come superuser o come un altro utente.

#### Esegui un comando come superuser:
```shell
sudo {{less /var/log/syslog}}
```
#### Modifica un file come superuser con il tuo editor di default:
```shell
sudo -e {{/etc/fstab}}
```
#### Esegui un comando come un altro utente e/o gruppo:
```shell
sudo -u {{utente}} -g {{gruppo}} {{id -a}}
```
#### Ripeti l'ultimo comando prefissandolo con "sudo" (funziona solo in bash, zsh, ecc):
```shell
sudo !!
```
#### Fai partire la shell di default con i privilegi da superuser:
```shell
sudo -i
```
{% endraw %}