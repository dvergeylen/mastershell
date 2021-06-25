---
layout: default
title: "unset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unset">
  <a href="/en/linux/unset.html">unset</a> <a href="#unset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove shell variables or functions.

#### Remove the variable `foo`, or if the variable doesn't exist, remove the function `foo`:
```shell
unset {{foo}}
```
#### Remove the variables foo and bar:
```shell
unset -v {{foo}} {{bar}}
```
#### Remove the function my_func:
```shell
unset -f {{my_func}}
```
{% endraw %}