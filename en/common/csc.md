---
layout: default
title: "csc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csc">
  <a href="/en/common/csc.html">csc</a> <a href="#csc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Microsoft C# Compiler.
> More information: <https://docs.microsoft.com/dotnet/csharp/language-reference/compiler-options/command-line-building-with-csc-exe>.

#### Compile one or more C# files to a CIL executable:
```shell
csc {{path/to/input_file_a.cs}} {{path/to/input_file_b.cs}}
```
#### Specify the output filename:
```shell
csc /out:{{path/to/filename}} {{path/to/input_file.cs}}
```
#### Compile into a `.dll` library instead of an executable:
```shell
csc /target:library {{path/to/input_file.cs}}
```
#### Reference another assembly:
```shell
csc /reference:{{path/to/library.dll}} {{path/to/input_file.cs}}
```
#### Embed a resource:
```shell
csc /resource:{{path/to/resource_file}} {{path/to/input_file.cs}}
```
#### Automatically generate XML documentation:
```shell
csc /doc:{{path/to/output.xml}} {{path/to/input_file.cs}}
```
#### Specify an icon:
```shell
csc /win32icon:{{path/to/icon.ico}} {{path/to/input_file.cs}}
```
#### Strongly-name the resulting assembly with a keyfile:
```shell
csc /keyfile:{{path/to/keyfile}} {{path/to/input_file.cs}}
```
{% endraw %}