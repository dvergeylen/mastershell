---
layout: default
title: "jc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jc">
  <a href="/en/common/jc.html">jc</a> <a href="#jc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to convert the output of multiple commands to JSON.
> More information: <https://github.com/kellyjonbrazil/jc>.

#### Convert command output to JSON via pipe:
```shell
{{ifconfig}} | jc {{--ifconfig}}
```
#### Convert command output to JSON via magic syntax:
```shell
jc {{ifconfig}}
```
#### Output pretty JSON via pipe:
```shell
{{ifconfig}} | jc {{--ifconfig}} -p
```
#### Output pretty JSON via magic syntax:
```shell
jc -p {{ifconfig}}
```
{% endraw %}