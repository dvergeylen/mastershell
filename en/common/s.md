---
layout: default
title: "s"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="s">
  <a href="/en/common/s.html">s</a> <a href="#s"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web search from the terminal.

#### Search for a query on Google(default provider):
```shell
s {{query}}
```
#### List all providers:
```shell
s --list-providers
```
#### Search for a query with a given provider:
```shell
s --provider {{provider}} {{query}}
```
#### Use a specified binary to perform the search query:
```shell
s --binary "{{binary}} {{arguments}}" {{query}}
```
{% endraw %}