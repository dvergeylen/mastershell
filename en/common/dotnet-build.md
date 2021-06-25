---
layout: default
title: "dotnet build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-build">
  <a href="/en/common/dotnet-build.html">dotnet build</a> <a href="#dotnet-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Builds a .NET application and its dependencies.
> More information: <https://docs.microsoft.com/dotnet/core/tools/dotnet-build>.

#### Compile the project or solution in the current directory:
```shell
dotnet build
```
#### Compile a .NET project or solution in debug mode:
```shell
dotnet build {{path/to/project_or_solution}}
```
#### Compile in release mode:
```shell
dotnet build --configuration {{Release}}
```
#### Compile without restoring dependencies:
```shell
dotnet build --no-restore
```
#### Compile with a specific verbosity level:
```shell
dotnet build --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
#### Compile for a specific runtime:
```shell
dotnet build --runtime {{runtime_identifier}}
```
#### Specify the output directory:
```shell
dotnet build --output {{path/to/directory}}
```
{% endraw %}