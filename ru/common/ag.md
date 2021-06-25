---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/ru/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Аналог ack, но имеет цель быть быстрее.
> Больше информации: <https://github.com/ggreer/the_silver_searcher>.

#### Найти файлы, содержащие "foo", и вывести подходящие строки в контексте:
```shell
ag {{foo}}
```
#### Найти файлы, содержащие "foo", в заданной папке:
```shell
ag {{foo}} {{путь/до/папки}}
```
#### Найти файлы, содержащие "foo", но вывести только имена файлов:
```shell
ag -l {{foo}}
```
#### Найти файлы, содержащие "FOO", независимо от регистра, и вывести только совпадения, а не строки целиком:
```shell
ag -i -o {{FOO}}
```
#### Найти "foo" в файлах, у которых в имени есть "bar":
```shell
ag {{foo}} -G {{bar}}
```
#### Найти файлы, содержимое которых совпадает с регулярным выражением:
```shell
ag '{{^ba(r|z)$}}'
```
#### Найти файлы, у которых имя совпадает с "foo":
```shell
ag -g {{foo}}
```
{% endraw %}