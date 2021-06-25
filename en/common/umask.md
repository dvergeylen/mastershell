---
layout: default
title: "umask"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="umask">
  <a href="/en/common/umask.html">umask</a> <a href="#umask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the read/write/execute permissions that are masked out (i.e. restricted) for newly created files by the user.

#### Display the current mask in octal notation:
```shell
umask
```
#### Display the current mask in symbolic (human-readable) mode:
```shell
umask -S
```
#### Change the mask symbolically to allow read permission for all users (the rest of the mask bits are unchanged):
```shell
umask {{a+r}}
```
#### Set the mask (using octal) to restrict no permissions for the file's owner, and restrict all permissions for everyone else:
```shell
umask {{077}}
```
{% endraw %}