---
layout: default
title: "iverilog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iverilog">
  <a href="/en/common/iverilog.html">iverilog</a> <a href="#iverilog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Preprocesses and compiles Verilog HDL (IEEE-1364) code, into executable programs for simulation.
> More information: <http://iverilog.icarus.com/>.

#### Compile a source file into an executable:
```shell
iverilog {{source.v}} -o {{executable}}
```
#### Also display all warnings:
```shell
iverilog {{source.v}} -Wall -o {{executable}}
```
#### Compile and run explicitly using the VVP runtime:
```shell
iverilog -o {{executable}} -tvvp {{source.v}}
```
#### Compile using Verilog library files from a different path:
```shell
iverilog {{source.v}} -o {{executable}} -I{{path/to/library_directory}}
```
#### Preprocess Verilog code without compiling:
```shell
iverilog -E {{source.v}}
```
{% endraw %}