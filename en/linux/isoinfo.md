---
layout: default
title: "isoinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="isoinfo">
  <a href="/en/linux/isoinfo.html">isoinfo</a> <a href="#isoinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility programs for dumping and verifying ISO disk images.

#### List all the files included in an ISO image:
```shell
isoinfo -f -i {{path/to/image.iso}}
```
#### E[x]tract a specific file from an ISO image and send it out stdout:
```shell
isoinfo -i {{path/to/image.iso}} -x {{/PATH/TO/FILE/INSIDE/ISO.EXT}}
```
#### Show header information for an ISO disk image:
```shell
isoinfo -d -i {{path/to/image.iso}}
```
{% endraw %}