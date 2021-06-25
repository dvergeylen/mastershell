---
layout: default
title: "virt-sparsify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virt-sparsify">
  <a href="/en/common/virt-sparsify.html">virt-sparsify</a> <a href="#virt-sparsify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Make virtual machine drive images thin-provisioned.
> NOTE: Use only for offline machines to avoid data corruption.
> Home page: <https://libguestfs.org/>.

#### Create a sparsified compressed image without snapshots from an unsparsified one:
```shell
virt-sparsify --compress {{path/to/image.qcow2}} {{path/to/image_new.qcow2}}
```
#### Sparsify an image in-place:
```shell
virt-sparsify --in-place {{path/to/image.img}}
```
{% endraw %}