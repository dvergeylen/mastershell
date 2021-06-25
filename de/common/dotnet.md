---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/de/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattformübergreifende Kommandozeilenandwendungen für .NET Core.
> Weitere Informationen: <https://docs.microsoft.com/dotnet/core/tools/>.

#### Initialisiere ein neues .NET Projekt:
```shell
dotnet new {{vorlagen_name}}
```
#### Stelle nuget-Pakete wieder her:
```shell
dotnet restore
```
#### Baue des .NET Projekt im aktuellen Ordner und führe es aus:
```shell
dotnet run
```
#### Führe eine gebaute dotnet-Applikation aus (Benötigt nur die Laufzeitumgebung. Die anderen Befehle benötigen auch den Entwicklungsteil):
```shell
dotnet {{pfad/zu/anwendung.dll}}
```
{% endraw %}