---
layout: default
title: "id"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="id">
  <a href="/en/common/id.html">id</a> <a href="#id"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display current user and group identity.
> More information: <https://www.gnu.org/software/coreutils/id>.

#### Display current user's id (UID), group id (GID) and groups to which they belong:
```shell
id
```
#### Display the current user identity as a number:
```shell
id -u
```
#### Display the current group identity as a number:
```shell
id -g
```
#### Display an arbitrary user's id (UID), group id (GID) and groups to which they belong:
```shell
id {{username}}
```
{% endraw %}