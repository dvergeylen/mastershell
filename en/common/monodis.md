---
layout: default
title: "monodis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="monodis">
  <a href="/en/common/monodis.html">monodis</a> <a href="#monodis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Mono Common Intermediate Language (CIL) disassembler.
> More information: <https://www.mono-project.com/docs/tools+libraries/tools/monodis/>.

#### Disassemble an assembly to textual CIL:
```shell
monodis {{path/to/assembly.exe}}
```
#### Save the output to a file:
```shell
monodis --output={{path/to/output.il}} {{path/to/assembly.exe}}
```
#### Show information about an assembly:
```shell
monodis --assembly {{path/to/assembly.dll}}
```
#### List the references of an assembly:
```shell
monodis --assemblyref {{path/to/assembly.exe}}
```
#### List all the methods in an assembly:
```shell
monodis --method {{path/to/assembly.exe}}
```
#### Show a list of resources embedded within an assembly:
```shell
monodis --manifest {{path/to/assembly.dll}}
```
#### Extract all the embedded resources to the current directory:
```shell
monodis --mresources {{path/to/assembly.dll}}
```
{% endraw %}