---
layout: default
title: "groups"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="groups">
  <a href="/en/common/groups.html">groups</a> <a href="#groups"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print group memberships for a user.
> More information: <https://www.gnu.org/software/coreutils/groups>.

#### Print group memberships for the current user:
```shell
groups
```
#### Print group memberships for a specific user:
```shell
groups {{username}}
```
#### Print group memberships for a list of users:
```shell
groups {{username1}} {{username2}} {{username3}}
```
{% endraw %}