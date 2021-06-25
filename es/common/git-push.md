---
layout: default
title: "git push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-push">
  <a href="/es/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enviar (*push*) los commits al repositorio remoto.
> Más información: <https://git-scm.com/docs/git-push>.

#### Envia los cambios locales en la rama actual a la misma rama en el remoto:
```shell
git push
```
#### Envia los cambios locales de una rama específica a la misma rama en el remoto:
```shell
git push {{nombre_remoto}} {{rama_local}}
```
#### Publica la rama actual en el repositorio remoto y establece el nombre remoto de la rama:
```shell
git push {{nombre_remoto}} -u {{rama_remota}}
```
#### Envia los cambios de todas las ramas locales a sus respectivas ramas en el repositorio remoto:
```shell
git push --all {{nombre_remoto}}
```
#### Elimina una rama en el repositorio remoto:
```shell
git push {{nombre_remoto}} --delete {{rama_remota}}
```
#### Elimina las ramas remotas que no están en el repositorio local:
```shell
git push --prune {{nombre_remoto}}
```
#### Publica las etiquetas que aún no están en el repositorio remoto:
```shell
git push --tags
```
{% endraw %}