---
layout: default
title: "usermod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="usermod">
  <a href="/en/linux/usermod.html">usermod</a> <a href="#usermod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifies a user account.
> More information: <https://manned.org/usermod>.

#### Change a user's name:
```shell
usermod -l {{newname}} {{user}}
```
#### Add user to supplementary groups (mind the whitespace):
```shell
usermod -a -G {{group1,group2}} {{user}}
```
#### Create a new home directory for a user and move their files to it:
```shell
usermod -m -d {{path/to/home}} {{user}}
```
{% endraw %}