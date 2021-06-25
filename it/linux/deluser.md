---
layout: default
title: "deluser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluser">
  <a href="/it/linux/deluser.html">deluser</a> <a href="#deluser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rimuovi un account utente o un utente da un gruppo.
> Maggiori informazioni: <https://manpages.debian.org/latest/adduser/deluser.html>.

#### Rimuovi un utente:
```shell
deluser {{nome}}
```
#### Rimuovi un utente insieme alla sua directory home e raccolta mail:
```shell
deluser -r {{nome}}
```
#### Rimuovi un utente da un gruppo:
```shell
deluser {{nome}} {{gruppo}}
```
{% endraw %}