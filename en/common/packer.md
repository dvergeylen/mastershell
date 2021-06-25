---
layout: default
title: "packer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="packer">
  <a href="/en/common/packer.html">packer</a> <a href="#packer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build automated machine images.
> More information: <https://www.packer.io/>.

#### Build an image:
```shell
packer build {{path/to/config.json}}
```
#### Check the syntax of a Packer image config:
```shell
packer validate {{path/to/config.json}}
```
{% endraw %}