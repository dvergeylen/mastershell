---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/ru/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Кросс-платформенная утилита командной строки .NET для .NET Core.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools>.

#### Инициализировать новый проект .NET:
```shell
dotnet new {{короткое_имя_шаблона}}
```
#### Восстановить пакеты nuget:
```shell
dotnet restore
```
#### Собрать и запустить проект .NET в текущей папке:
```shell
dotnet run
```
#### Запустить собранное приложение .NET (требуется только среда исполнения, для остальных команд требуется установленный .NET Core SDK):
```shell
dotnet {{путь/до/приложения.dll}}
```
{% endraw %}