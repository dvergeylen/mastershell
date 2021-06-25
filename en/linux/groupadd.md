---
layout: default
title: "groupadd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="groupadd">
  <a href="/en/linux/groupadd.html">groupadd</a> <a href="#groupadd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add user groups to the system.
> More information: <https://manned.org/groupadd>.

#### Create a new Linux group:
```shell
groupadd {{group_name}}
```
#### Create new group with a specific groupid:
```shell
groupadd {{group_name}} -g {{group_id}}
```
{% endraw %}