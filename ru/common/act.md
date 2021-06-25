---
layout: default
title: "act"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="act">
  <a href="/ru/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Запуск GitHub Actions локально с использованием Docker.
> Больше информации: <https://github.com/nektos/act>.

#### Вывести список доступных actions:
```shell
act -l
```
#### Запустить событие по умолчанию:
```shell
act
```
#### Запустить заданное событие:
```shell
act {{тип_события}}
```
#### Запустить заданный action:
```shell
act -a {{action_id}}
```
#### Не производить реальный запуск actions (пробный прогон):
```shell
act -n
```
#### Отображать расширенный лог:
```shell
act -v
```
{% endraw %}