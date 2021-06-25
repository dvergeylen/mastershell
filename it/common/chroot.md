---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/it/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui un comando o una shell interattiva con una speciale root directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/chroot>.

#### Esegui un comando con una diversa root directory:
```shell
chroot {{/percorso/alla/nuova/root}} {{comando}}
```
#### Specifica utente e gruppo (ID o nome) da usare:
```shell
chroot --userspec={{utente:gruppo}}
```
{% endraw %}