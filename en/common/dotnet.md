---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/en/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross platform .NET command-line tools for .NET Core.
> More information: <https://docs.microsoft.com/dotnet/core/tools>.

#### Initialize a new .NET project:
```shell
dotnet new {{template_short_name}}
```
#### Restore nuget packages:
```shell
dotnet restore
```
#### Build and execute the .NET project in the current directory:
```shell
dotnet run
```
#### Run a packaged dotnet application (only needs the runtime, the rest of the commands require the .NET Core SDK installed):
```shell
dotnet {{path/to/application.dll}}
```
{% endraw %}