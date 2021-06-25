---
layout: default
title: "git pr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pr">
  <a href="/es/common/git-pr.html">git pr</a> <a href="#git-pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comprueba las solicitudes de extracción de cambios (*pull requests*) de GitHub localmente.
> Más información: <https://github.com/tj/git-extras/blob/master/Commands.md#git-pr>.

#### Comprueba una pull request específica:
```shell
git pr {{número_pr}}
```
#### Comprueba una pull request para un remoto específico:
```shell
git pr {{número_pr}} {{remoto}}
```
#### Comprueba una pull request a partir de su URL:
```shell
git pr {{url}}
```
#### Limpia las ramas antiguas de pull requests:
```shell
git pr clean
```
{% endraw %}