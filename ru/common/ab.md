---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/ru/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита бенчмаркинга Apache. Самая простая утилита для проведения нагрузочного тестирования.
> Больше информации: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Запустить 100 запросов HTTP GET по заданному URL:
```shell
ab -n {{100}} {{url}}
```
#### Запустить 100 запросов HTTP GET, обрабатывая до 10 одновременно, по заданному URL:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Использовать постоянное соединение (keep-alive):
```shell
ab -k {{url}}
```
#### Задать максимальное число секунд, которое можно затратить на бенчмаркинг:
```shell
ab -t {{60}} {{url}}
```
#### Запустить 100 запросов HTTP POST по заданному URL, используя в качестве полезной нагрузки JSON из файла:
```shell
ab -n {{100}} -T {{application/json}} -p {{путь/до/файла.json}} {{url}}
```
{% endraw %}