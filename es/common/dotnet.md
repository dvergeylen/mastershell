---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/es/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta multiplataforma de línea de comandos para .NET Core.
> Más información: <https://docs.microsofot.com/dotnet/core/tools>.

#### Inicializa un proyecto .NET nuevo:
```shell
dotnet new {{nombre_de_la_plantilla}}
```
#### Restaura los paquetes NuGet:
```shell
dotnet restore
```
#### Compila y ejectura el proyecto .NET en el directorio actual:
```shell
dotnet run
```
#### Ejecuta una aplicación dotnet empaquetada (solo necesita el entorno en tiempo de ejecución, el resto de los comandos requieren el SDK de .NET Core instalado):
```shell
dotnet {{ruta/a/la/aplicación.dll}}
```
{% endraw %}