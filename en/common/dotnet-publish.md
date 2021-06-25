---
layout: default
title: "dotnet publish"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet-publish">
  <a href="/en/common/dotnet-publish.html">dotnet publish</a> <a href="#dotnet-publish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Publish a .NET application and its dependencies to a directory for deployment to a hosting system.
> More information: <https://docs.microsoft.com/dotnet/core/tools/dotnet-publish>.

#### Compile a .NET project in release mode:
```shell
dotnet publish --configuration Release {{path/to/project_file}}
```
#### Publish the .NET Core runtime with your application for the specified runtime:
```shell
dotnet publish --self-contained true --runtime {{runtime_identifier}} {{path/to/project_file}}
```
#### Package the application into a platform-specific single-file executable:
```shell
dotnet publish --runtime {{runtime_identifier}} -p:PublishSingleFile=true {{path/to/project_file}}
```
#### Trim unused libraries to reduce the deployment size of an application:
```shell
dotnet publish --self-contained true --runtime {{runtime_identifier}} -p:PublishTrimmed=true {{path/to/project_file}}
```
#### Compile a .NET project without restoring dependencies:
```shell
dotnet publish --no-restore {{path/to/project_file}}
```
#### Specify the output directory:
```shell
dotnet publish --output {{path/to/directory}} {{path/to/project_file}}
```
{% endraw %}