---
layout: default
title: "weasyprint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="weasyprint">
  <a href="/ru/common/weasyprint.html">weasyprint</a> <a href="#weasyprint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Переводить HTML в PDF или PNG.
> Больше информации: <https://weasyprint.org/>.

#### Перевести HTML файл в PDF:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.pdf}}
```
#### Перевести HTML файл в PNG, включая дополнительные пользовательские таблицы стилей:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --stylesheet {{путь/до/таблицы-стилей.css}}
```
#### При переводе выводить дополнительную отладочную информацию:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.pdf}} --verbose
```
#### При выводе в PNG указать нестандартное разрешение:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --resolution {{300}}
```
#### Во входном HTML файле указать базовый URL для относительных URLs:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --base-url {{url_или_имя-файла}}
```
{% endraw %}