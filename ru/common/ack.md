---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/ru/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита для поиска, подобная grep, оптимизировання для программистов.
> Больше информации: <https://beyondgrep.com/documentation/>.

#### Найти файлы, содержащие "foo":
```shell
ack {{foo}}
```
#### Найти файлы заданного типа:
```shell
ack --ruby {{foo}}
```
#### Подсчитать общее число совпадений для термина "foo":
```shell
ack -ch {{foo}}
```
#### Показать имен файлов, содержащие "foo" и число совпадений в каждом файле:
```shell
ack -cl {{foo}}
```
#### Поиск заданной строки в файле:
```shell
ack bar "{{foo bar}}" {{путь/до/файла}}
```
#### Поиск в файле по заданному регулярному выражению:
```shell
ack bar "{{[bB]ar \d+}}" {{путь/до/файла}}
```
#### Вывести список всех допустимых типов:
```shell
ack --help-types
```
{% endraw %}