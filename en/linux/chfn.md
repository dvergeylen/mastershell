---
layout: default
title: "chfn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chfn">
  <a href="/en/linux/chfn.html">chfn</a> <a href="#chfn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update `finger` info for a user.

#### Update a user's "Name" field in the output of `finger`:
```shell
chfn -f {{new_display_name}} {{username}}
```
#### Update a user's "Office Room Number" field for the output of `finger`:
```shell
chfn -o {{new_office_room_number}} {{username}}
```
#### Update a user's "Office Phone Number" field for the output of `finger`:
```shell
chfn -p {{new_office_telephone_number}} {{username}}
```
#### Update a user's "Home Phone Number" field for the output of `finger`:
```shell
chfn -h {{new_home_telephone_number}} {{username}}
```
{% endraw %}