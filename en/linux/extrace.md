---
layout: default
title: "extrace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="extrace">
  <a href="/en/linux/extrace.html">extrace</a> <a href="#extrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trace exec() calls.
> More information: <https://github.com/chneukirchen/extrace>.

#### Trace all program executions occurring on the system:
```shell
sudo extrace
```
#### Run a command and only trace descendants of this command:
```shell
sudo extrace {{command}}
```
#### Print the current working directory of each process:
```shell
sudo extrace -d
```
#### Resolve the full path of each executable:
```shell
sudo extrace -l
```
#### Display the user running each process:
```shell
sudo extrace -u
```
{% endraw %}