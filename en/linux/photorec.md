---
layout: default
title: "photorec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="photorec">
  <a href="/en/linux/photorec.html">photorec</a> <a href="#photorec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deleted file recovery tool.
> It is recommended to write recovered files to a disk separate to the one being recovered from.
> More information: <https://www.cgsecurity.org/wiki/PhotoRec>.

#### Run PhotoRec on a specific device:
```shell
sudo photorec {{/dev/sdb}}
```
#### Run PhotoRec on a disk image (`image.dd`):
```shell
sudo photorec {{path/to/image.dd}}
```
{% endraw %}