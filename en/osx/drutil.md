---
layout: default
title: "drutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drutil">
  <a href="/en/osx/drutil.html">drutil</a> <a href="#drutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with DVD burners.

#### Eject a disk from the drive:
```shell
drutil eject
```
#### Burn a directory as an ISO9660 filesystem onto a DVD. Don't verify and eject when complete:
```shell
drutil burn -noverify -eject -iso9660
```
{% endraw %}