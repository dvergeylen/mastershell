---
layout: default
title: "cradle install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-install">
  <a href="/en/common/cradle-install.html">cradle install</a> <a href="#cradle-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installs the Cradle PHP framework components.
> More information: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#install>.

#### Install Cradle's components (User will be prompted for further details):
```shell
cradle install
```
#### Forcefully overwrite files:
```shell
cradle install --force
```
#### Skip running SQL migrations:
```shell
cradle install --skip-sql
```
#### Skip running package updates:
```shell
cradle install --skip-versioning
```
#### Use specific database details:
```shell
cradle install -h {{hostname}} -u {{username}} -p {{password}}
```
{% endraw %}