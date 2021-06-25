---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/it/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumenti .NET da linea di comando multipiattaforma per .NET Core.
> Maggiori informazioni: <https://docs.microsoft.com/dotnet/core/tools>.

#### Inizializza un nuovo progetto .NET:
```shell
dotnet new {{nome_abbreviato_template}}
```
#### Ripristina pacchetti nuget:
```shell
dotnet restore
```
#### Costruisci ed esegui il progetto .NET nella directory corrente:
```shell
dotnet run
```
#### Esegui una applicazione dotnet pacchettizzata (solo il runtime è necessario, il resto dei comandi richiedono .NET Core SDK):
```shell
dotnet {{percorso/a/applicazione.dll}}
```
{% endraw %}