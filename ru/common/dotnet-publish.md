---
layout: default
title: "dotnet publish"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-publish">
  <a href="/ru/common/dotnet-publish.html">dotnet publish</a> <a href="#dotnet-publish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Публикует .NET-приложение и его зависимости в папку для развёртываения на целевой системе.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-publish>.

#### Скомпилировать проект .NET в режиме release:
```shell
dotnet publish --configuration Release {{путь/до/файла_проекта}}
```
#### Опубликовать ваше приложение с заданной средой исполнения .NET Core:
```shell
dotnet publish --self-contained true --runtime {{идентификатор_среды_исполения}} {{путь/до/файла_проекта}}
```
#### Упаковать приложение в один исполняемый файл для заданной платформы:
```shell
dotnet publish --runtime {{идентификатор_среды_исполения}} -p:PublishSingleFile=true {{путь/до/файла_проекта}}
```
#### Обрезать неиспользуемые библиотеки чтобы уменьшить размер развёртывания приложения:
```shell
dotnet publish --self-contained true --runtime {{идентификатор_среды_исполения}} -p:PublishTrimmed=true {{путь/до/файла_проекта}}
```
#### Скомпилировать проект .NET без восстановления зависимостей:
```shell
dotnet publish --no-restore {{путь/до/файла_проекта}}
```
#### Указать целевую папку:
```shell
dotnet publish --output {{путь/до/папки}} {{путь/до/файла_проекта}}
```
{% endraw %}