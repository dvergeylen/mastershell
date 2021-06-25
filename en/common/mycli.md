---
layout: default
title: "mycli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mycli">
  <a href="/en/common/mycli.html">mycli</a> <a href="#mycli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line client for MySQL that can do auto-completion and syntax highlighting.
> More information: <https://mycli.net>.

#### Connect to a local database on port 3306, using the current user's username:
```shell
mycli {{database_name}}
```
#### Connect to a database (user will be prompted for a password):
```shell
mycli -u {{username}} {{database_name}}
```
#### Connect to a database on another host:
```shell
mycli -h {{database_host}} -P {{port}} -u {{username}} {{database_name}}
```
{% endraw %}