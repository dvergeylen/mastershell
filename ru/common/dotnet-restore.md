---
layout: default
title: "dotnet restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-restore">
  <a href="/ru/common/dotnet-restore.html">dotnet restore</a> <a href="#dotnet-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Восстанавливает зависимости и утилиты для проекта .NET.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-restore>.

#### Восстановить зависимости для проекта или решения .NET в текущей директории:
```shell
dotnet restore
```
#### Восстановить зависимости для проекта или решенияs .NET по заданному пути:
```shell
dotnet restore {{путь/до/проекта_или_решения}}
```
#### Восстановить зависимости без кеширования HTTP-запросов:
```shell
dotnet restore --no-cache
```
#### Принудительно восстановить все зависимости, даже если предыдущее восстановление было успешным:
```shell
dotnet restore --force
```
#### Восстановить зависимости, считая что ошибки источника пакетов это предупреждения:
```shell
dotnet restore --ignore-failed-sources
```
#### Восстановить зависимости, используя заданный уровень детализации выводимой информации:
```shell
dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
{% endraw %}