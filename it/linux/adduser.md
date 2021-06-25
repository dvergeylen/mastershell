---
layout: default
title: "adduser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adduser">
  <a href="/it/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio per aggiungere utenti.
> Maggiori informazioni: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Crea un nuovo utente con una home directory predefinita e richiede all'utente di impostare una password:
```shell
adduser {{nome_utente}}
```
#### Crea un utente senza una home directory:
```shell
adduser --no-create-home {{nome_utente}}
```
#### Crea un utente con una home directory nel percorso specificato:
```shell
adduser --home {{percorso/all/home}} {{nome_utente}}
```
#### Crea un nuovo utente con l'interprete di comandi(shell) specificato come shell di accesso:
```shell
adduser --shell {{percorso/alla/shell}} {{nome_utente}}
```
#### Crea un nuovo utente appartenente al gruppo specificato:
```shell
adduser --ingroup {{gruppo}} {{nome_utente}}
```
#### Aggiunge un utente esistente al gruppo specificato:
```shell
adduser {{nome_utente}} {{gruppo}}
```
{% endraw %}