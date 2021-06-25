---
layout: default
title: "git bisect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bisect">
  <a href="/es/common/git-bisect.html">git bisect</a> <a href="#git-bisect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utiliza la búsqueda binaria para encontrar el commit que introdujo un error.
> Git salta de un lado a otro del gráfico de commits para hasta alcanzar progresivamente el commit defectuoso.
> Más información: <https://git-scm.com/docs/git-bisect>.

#### Comienza un sesión de bisecado en un rango de commits delimitada por un commit erróneo conocido y por uno sano conocido (normalmente más antiguo):
```shell
git bisect start {{commit_erroneo}} {{commit_bueno}}
```
#### Para cada commit que `git bisect` selecciona, marcarlo como "malo" o "bueno" después de probarlo para el problema:
```shell
git bisect {{bueno|malo}}
```
#### Después de que `git bisect` determine con precisión el commit defectuoso, termina la sesión de bisecado y vuelve a la rama anterior:
```shell
git bisect reset
```
#### Salta un commit durante una sesión de bisecado (p. ej., uno que falla las pruebas debido a un problema diferente):
```shell
git bisect skip
```
{% endraw %}