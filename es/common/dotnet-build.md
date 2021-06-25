---
layout: default
title: "dotnet build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-build">
  <a href="/es/common/dotnet-build.html">dotnet build</a> <a href="#dotnet-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compila una aplicación .NET y sus dependencias.
> Más información: <https://docs.microsoft.com/dotnet/core/tools/dotnet-build>.

#### Compila el proyecto o solución en el directorio actual:
```shell
dotnet build
```
#### Compila un proyecto o solución .NET en el modo de depuración:
```shell
dotnet build {{ruta/al/proyecto_o_solución}}
```
#### Compila en modo de lanzamiento:
```shell
dotnet build --configuration {{Release}}
```
#### Compila sin restaurar las dependencias:
```shell
dotnet build --no-restore
```
#### Compila con un nivel específico de verbosidad:
```shell
dotnet build --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
#### Compila para un tiempo de ejecución específico:
```shell
dotnet build --runtime {{identificador_del_tiempo_de_ejecución}}
```
#### Especifica el directorio de salida:
```shell
dotnet build --output {{ruta/al/directorio}}
```
{% endraw %}