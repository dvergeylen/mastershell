---
layout: default
title: "dotnet restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-restore">
  <a href="/en/common/dotnet-restore.html">dotnet restore</a> <a href="#dotnet-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restores the dependencies and tools of a .NET project.
> More information: <https://docs.microsoft.com/dotnet/core/tools/dotnet-restore>.

#### Restore dependencies for a .NET project or solution in the current directory:
```shell
dotnet restore
```
#### Restore dependencies for a .NET project or solution in a specific location:
```shell
dotnet restore {{path/to/project_or_solution}}
```
#### Restore dependencies without caching the HTTP requests:
```shell
dotnet restore --no-cache
```
#### Force all dependencies to be resolved even if the last restore was successful:
```shell
dotnet restore --force
```
#### Restore dependencies using package source failures as warnings:
```shell
dotnet restore --ignore-failed-sources
```
#### Restore dependencies with a specific verbosity level:
```shell
dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
{% endraw %}