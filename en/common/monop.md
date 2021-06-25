---
layout: default
title: "monop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="monop">
  <a href="/en/common/monop.html">monop</a> <a href="#monop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds and displays signatures of Types and methods inside .NET assemblies.

#### Show the structure of a Type built-in of the .NET Framework:
```shell
monop {{System.String}}
```
#### List the types in an assembly:
```shell
monop -r:{{path/to/assembly.exe}}
```
#### Show the structure of a Type in a specific assembly:
```shell
monop -r:{{path/to/assembly.dll}} {{Namespace.Path.To.Type}}
```
#### Only show members defined in the specified Type:
```shell
monop -r:{{path/to/assembly.dll}} --only-declared {{Namespace.Path.To.Type}}
```
#### Show private members:
```shell
monop -r:{{path/to/assembly.dll}} --private {{Namespace.Path.To.Type}}
```
#### Hide obsolete members:
```shell
monop -r:{{path/to/assembly.dll}} --filter-obsolete {{Namespace.Path.To.Type}}
```
#### List the other assemblies that a specified assembly references:
```shell
monop -r:{{path/to/assembly.dll}} --refs
```
{% endraw %}