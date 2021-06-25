---
layout: default
title: "groupmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="groupmod">
  <a href="/en/linux/groupmod.html">groupmod</a> <a href="#groupmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modify existing user groups in the system.
> More information: <https://manned.org/groupmod>.

#### Change the group name:
```shell
groupmod -n {{new_group_name}} {{old_group_name}}
```
#### Change the group id:
```shell
groupmod -g {{new_group_id}} {{old_group_name}}
```
{% endraw %}