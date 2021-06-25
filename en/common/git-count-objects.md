---
layout: default
title: "git count-objects"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-count-objects">
  <a href="/en/common/git-count-objects.html">git count-objects</a> <a href="#git-count-objects"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Count the number of unpacked objects and their disk consumption.
> More information: <https://git-scm.com/docs/git-count-objects>.

#### Count all objects and display the total disk usage:
```shell
git count-objects
```
#### Display a count of all objects and their total disk usage, displaying sizes in human readable units:
```shell
git count-objects --human-readable
```
#### Display more verbose information:
```shell
git count-objects --verbose
```
#### Display more verbose information, displaying sizes in human readable units:
```shell
git count-objects --human-readable --verbose
```
{% endraw %}