---
layout: default
title: "git am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-am">
  <a href="/es/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aplica archivos de parche. Útil cuando se reciben commits por correo electrónico.
> Véase también `git format-patch`, comando que genera archivo de parche.
> Más información: <https://git-scm.com/docs/git-am>.

#### Aplica un archivo de parche:
```shell
git am {{ruta/al/archivo.patch}}
```
#### Aborta el proceso de aplicar un archivo de parche:
```shell
git am --abort
```
#### Aplica todo lo posible de un archivo de parche y guarda los fragmentos fallidos para rechazar archivos:
```shell
git am --reject {{ruta/al/archivo.patch}}
```
{% endraw %}