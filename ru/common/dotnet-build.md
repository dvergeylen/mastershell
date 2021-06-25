---
layout: default
title: "dotnet build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-build">
  <a href="/ru/common/dotnet-build.html">dotnet build</a> <a href="#dotnet-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Собирает приложение .NET и все его зависимости.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-build>.

#### Скомпилировать проект или решение в текущей директории:
```shell
dotnet build
```
#### Скомпилировать проект или решение .NET в режиме debug:
```shell
dotnet build {{путь/до/проекта_или_решения}}
```
#### Скомпилировать в режиме release:
```shell
dotnet build --configuration {{Release}}
```
#### Скомпилировать без восстановления зависимостей:
```shell
dotnet build --no-restore
```
#### Скомпилировать с заданным уровнем детализации выводимой информации:
```shell
dotnet build --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
#### Скомпилировать для заданной среды исполнения:
```shell
dotnet build --runtime {{идентификатор_среды_исполения}}
```
#### Указать целевую папку:
```shell
dotnet build --output {{путь/до/папки}}
```
{% endraw %}