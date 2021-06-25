---
layout: default
title: "ctest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctest">
  <a href="/it/common/ctest.html">ctest</a> <a href="#ctest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programma per eseguire test in progetti CMake.
> Maggiori informazioni: <https://gitlab.kitware.com/cmake/community/wikis/doc/ctest/Testing-With-CTest>.

#### Esegui tutti i test definiti nel progetto CMakw, eseguendo 4 job allo stesso tempo in parallelo:
```shell
ctest -j{{4}} --output-on-failure
```
#### Mostra una lista dei test disponibili:
```shell
ctest -N
```
#### Esegui un singolo test in base al suo nome, o filtrando con una espressione regolare:
```shell
ctest --output-on-failure -R '^{{nome_test}}$'
```
{% endraw %}