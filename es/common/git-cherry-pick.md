---
layout: default
title: "git cherry-pick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry-pick">
  <a href="/es/common/git-cherry-pick.html">git cherry-pick</a> <a href="#git-cherry-pick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aplica los cambios introducidos por commits existentes a la rama actual.
> Para aplicar cambios a otra rama, primero utiliza `git checkout` para cambiar a la rama deseada.
> Más información: <https://git-scm.com/docs/git-cherry-pick>.

#### Aplica un commit a la rama actual:
```shell
git cherry-pick {{commit}}
```
#### Aplica un rango de commits de la rama actual (véase también `git rebase --onto`):
```shell
git cherry-pick {{commit_inicial}}~..{{commit_final}}
```
#### Aplica múltiples commits no secuenciales a la rama actual:
```shell
git cherry-pick {{commit_1}} {{commit_2}}
```
#### Añade los cambios de un commit al directorio de trabajo, sin crear un commit:
```shell
git cherry-pick -n {{commit}}
```
{% endraw %}