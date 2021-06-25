---
layout: default
title: "git format-patch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-format-patch">
  <a href="/es/common/git-format-patch.html">git format-patch</a> <a href="#git-format-patch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prepara archivos .patch. Es útil cuando se envían commits por correo electrónico.
> Véase también `git-am`, comando que puede aplicar los archivos .patch generados.
> Más información: <https://git-scm.com/docs/git-format-patch>.

#### Crea un archivo `.patch` con nombre automático para todos los cambios que no están en el push:
```shell
git format-patch {{origen}}
```
#### Escribe un archivo `.patch` para todos los commits entre dos revisiones a stdout:
```shell
git format-patch {{revisión_1}}..{{revisión_2}}
```
#### Escribe un archivo `.patch` para los 3 últimos commits:
```shell
git format-patch -{{3}}
```
{% endraw %}