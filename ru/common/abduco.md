---
layout: default
title: "abduco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="abduco">
  <a href="/ru/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Менеджер сессий терминала.
> Больше информации: <http://www.brain-dump.org/projects/abduco/>.

#### Вывести список сеансов:
```shell
abduco
```
#### Подключиться к сеансу, и создать его, если он не существует:
```shell
abduco -A {{имя}} {{bash}}
```
#### Подключиться к сеансу с `dvtm`, и создать его, если он не существует:
```shell
abduco -A {{имя}}
```
#### Отключиться от сеанса:
```shell
Ctrl + \
```
#### Подключиться к сеансу в режиме только для чтения:
```shell
abduco -Ar {{имя}}
```
{% endraw %}