---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/pl/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zarządzaj obrazami Dockera.
> Więcej informacji: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Wyświetl wszystkie obrazy Docker:
```shell
docker images
```
#### Wyświetl wszystkie obrazy Dockera, w tym intermediates:
```shell
docker images -a
```
#### Wyświetl dane wyjściowe w trybie quiet (tylko identyfikatory numeryczne):
```shell
docker images -q
```
#### Wyświetl wszystkie obrazy Docker nieużywane przez żaden kontener:
```shell
docker images --filter dangling=true
```
{% endraw %}