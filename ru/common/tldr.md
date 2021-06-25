---
layout: default
title: "tldr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr">
  <a href="/ru/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Показывает простые страницы помощи для инструментов коммандной строки из проекта tldr-pages.
> Больше информации: <https://tldr.sh>.

#### Показывает типичное использование комманды (подсказка: то как вы попали сюда!):
```shell
tldr {{комманда}}
```
#### Показывает tldr страницу для комманды tar для Linux:
```shell
tldr -p {{linux}} {{tar}}
```
#### Получить помощь по подкоманде Git:
```shell
tldr {{git-checkout}}
```
#### Обновить локальные tldr страницы (если клиент поддерживает кэширование):
```shell
tldr -u
```
{% endraw %}