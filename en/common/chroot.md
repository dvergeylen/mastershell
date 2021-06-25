---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/en/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run command or interactive shell with special root directory.
> More information: <https://www.gnu.org/software/coreutils/chroot>.

#### Run command as new root directory:
```shell
chroot {{path/to/new/root}} {{command}}
```
#### Specify user and group (ID or name) to use:
```shell
chroot --userspec={{user:group}}
```
{% endraw %}