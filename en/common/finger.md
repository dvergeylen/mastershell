---
layout: default
title: "finger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="finger">
  <a href="/en/common/finger.html">finger</a> <a href="#finger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> User information lookup program.
> More information: <https://manned.org/finger>.

#### Display information about currently logged in users:
```shell
finger
```
#### Display information about a specific user:
```shell
finger {{username}}
```
#### Display the user's login name, real name, terminal name, and other information:
```shell
finger -s
```
#### Produce multiline output format displaying same information as `-s` as well as user's home directory, home phone number, login shell, mail status, etc.:
```shell
finger -l
```
#### Prevent matching against user's names and only use login names:
```shell
finger -m
```
{% endraw %}