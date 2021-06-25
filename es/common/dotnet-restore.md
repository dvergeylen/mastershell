---
layout: default
title: "dotnet restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-restore">
  <a href="/es/common/dotnet-restore.html">dotnet restore</a> <a href="#dotnet-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restarua las dependencias y herramientas de un proyecto .NET.
> Más información: <https://docs.microsoft.com/dotnet/core/tools/dotnet-restore>.

#### Restaura dependencias para un proyecto o solución .NET en el directorio actual:
```shell
dotnet restore
```
#### Restaura dependencias para un proyecto o solución .NET en una ubicación específica:
```shell
dotnet restore {{ruta/al/proyecto_o_solución}}
```
#### Restaura depedencias sin almacenar las solicitudes HTTP en caché:
```shell
dotnet restore --no-cache
```
#### Obliga a todas las dependencias a ser resueltas incluso si la última restauración fue exitosa:
```shell
dotnet restore --force
```
#### Restaura dependencias usando los orígenes con error como advertencias:
```shell
dotnet restore --ignore-failed-sources
```
#### Restaura dependencias con un nivel específico de verbosidad:
```shell
dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
{% endraw %}