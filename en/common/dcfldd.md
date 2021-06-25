---
layout: default
title: "dcfldd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dcfldd">
  <a href="/en/common/dcfldd.html">dcfldd</a> <a href="#dcfldd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enhanced version of dd for forensics and security.
> More information: <http://dcfldd.sourceforge.net/>.

#### Copy a disk to a raw image file and hash the image using SHA256:
```shell
dcfldd if=/dev/{{disk_device}} of={{file.img}} hash=sha256 hashlog={{file.hash}}
```
#### Copy a disk to a raw image file, hashing each 1GB chunk:
```shell
dcfldd if=/dev/{{disk_device}} of={{file.img}} hash={{sha512|sha384|sha256|sha1|md5}} hashlog={{file.hash}} hashwindow={{1G}}
```
{% endraw %}