---
layout: default
title: "ghdl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghdl">
  <a href="/en/common/ghdl.html">ghdl</a> <a href="#ghdl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-source simulator for the VHDL language.
> More information: <http://ghdl.free.fr>.

#### Analyze a VHDL source file and produce an object file:
```shell
ghdl -a {{filename.vhdl}}
```
#### Elaborate a design (where `{{design}}` is the name of a configuration unit, entity unit or architecture unit):
```shell
ghdl -e {{design}}
```
#### Run an elaborated design:
```shell
ghdl -r {{design}}
```
#### Run an elaborated design and dump output to a waveform file:
```shell
ghdl -r {{design}} --wave={{output.ghw}}
```
#### Check the syntax of a VHDL source file:
```shell
ghdl -s {{filename.vhdl}}
```
#### Display the help page:
```shell
ghdl --help
```
{% endraw %}