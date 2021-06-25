---
layout: default
title: "mkisofs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkisofs">
  <a href="/en/linux/mkisofs.html">mkisofs</a> <a href="#mkisofs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create ISO files from directories.
> Also aliased as `genisoimage`.

#### Create an ISO from a directory:
```shell
mkisofs -o {{filename.iso}} {{path/to/source_directory}}
```
#### Set the disc label when creating an ISO:
```shell
mkisofs -o {{filename.iso}} -V "{{label_name}}" {{path/to/source_directory}}
```
{% endraw %}