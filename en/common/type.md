---
layout: default
title: "type"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="type">
  <a href="/en/common/type.html">type</a> <a href="#type"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the kind of command the shell will execute.

#### Display the kind of a command:
```shell
type {{command}}
```
#### Display all locations containing the specified executable:
```shell
type -a {{command}}
```
#### Display the name of the disk file that would be executed:
```shell
type -p {{command}}
```
{% endraw %}