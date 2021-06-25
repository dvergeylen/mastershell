---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/nl/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Voer commando of interactieve shell uit met een speciale hoofdmap.
> Meer informatie: <https://www.gnu.org/software/coreutils/chroot>.

#### Voer commando uit met gegeven hoofdmap:
```shell
chroot {{pad/naar/nieuwe/hoofdmap}} {{commando}}
```
#### Specificeer gebruiker en groep (ID of naam) om te gebruiken:
```shell
chroot --userspec={{gebruiker:groep}}
```
{% endraw %}