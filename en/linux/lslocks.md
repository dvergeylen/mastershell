---
layout: default
title: "lslocks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lslocks">
  <a href="/en/linux/lslocks.html">lslocks</a> <a href="#lslocks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List local system locks.

#### List all local system locks:
```shell
lslocks
```
#### List locks with defined column headers:
```shell
lslocks --output {{PID}},{{COMMAND}},{{PATH}}
```
#### List locks producing a raw output (no columns), and without column headers:
```shell
lslocks --raw --noheadings
```
#### List locks by PID input:
```shell
lslocks --pid {{PID}}
```
#### List locks with json output to stdout:
```shell
lslocks --json
```
{% endraw %}