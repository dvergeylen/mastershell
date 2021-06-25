---
layout: default
title: "unzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unzip">
  <a href="/ru/common/unzip.html">unzip</a> <a href="#unzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Извлекает сжатые файлы из архива zip.

#### Распаковать файл(ы) zip (для нескольких файлов укажите пути через пробел):
```shell
unzip {{архив(ы)}}
```
#### Распаковать файл(ы) по нужному пути:
```shell
unzip {{архив(ы)}} -d {{/путь/куда/положить/извлечённый_файл(ы)}}
```
#### Вывести список файлов в архиве zip, не распаковывая их:
```shell
unzip -l {{архив.zip}}
```
#### Извлечь содержимое файла в stdout вместе с именами распакованных файлов:
```shell
unzip -c {{архив.zip}}
```
#### Распаковать архив zip, который был создан на windows и содержит не-ascii имена файлов (напр. кириллица):
```shell
unzip -O {{gbk}} {{архив.zip}}
```
{% endraw %}