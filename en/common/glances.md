---
layout: default
title: "glances"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="glances">
  <a href="/en/common/glances.html">glances</a> <a href="#glances"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A cross-platform system monitoring tool.
> More information: <https://nicolargo.github.io/glances/>.

#### Run in terminal:
```shell
glances
```
#### Run in web server mode to show results in browser:
```shell
glances -w
```
#### Run in server mode to allow connections from other Glances clients:
```shell
glances -s
```
#### Connect to a Glances server:
```shell
glances -c {{hostname}}
```
#### Require a password in (web) server mode:
```shell
glances -s --password
```
{% endraw %}