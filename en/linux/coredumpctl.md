---
layout: default
title: "coredumpctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="coredumpctl">
  <a href="/en/linux/coredumpctl.html">coredumpctl</a> <a href="#coredumpctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retrieve and process saved core dumps and metadata.
> More information: <https://www.freedesktop.org/software/systemd/man/coredumpctl.html>.

#### List all captured core dumps:
```shell
coredumpctl list
```
#### List captured core dumps for a program:
```shell
coredumpctl list {{program}}
```
#### Show information about the core dumps matching a program with `PID`:
```shell
coredumpctl info {{PID}}
```
#### Invoke debugger using the last core dump of a program:
```shell
coredumpctl debug {{program}}
```
#### Extract the last core dump of a program to a file:
```shell
coredumpctl --output={{path/to/file}} dump {{program}}
```
{% endraw %}