---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/pl/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wieloplatformowe narzędzia wiersza polecenia .NET dla platformy .NET Core.
> Więcej informacji: <https://docs.microsoft.com/dotnet/core/tools>.

#### Zainicjuj nowy projekt .NET:
```shell
dotnet new {{szablon_krotka_nazwa}}
```
#### Przywróć pakiety nuget:
```shell
dotnet restore
```
#### Zbuduj i uruchom projekt .NET w bieżącym katalogu:
```shell
dotnet run
```
#### Uruchom pakietową aplikację dotnet (wymaga tylko środowiska wykonawczego, pozostałe polecenia wymagają zainstalowanego zestawu .NET Core SDK):
```shell
dotnet {{sciezka/do/aplikacji.dll}}
```
{% endraw %}