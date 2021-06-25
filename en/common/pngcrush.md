---
layout: default
title: "pngcrush"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pngcrush">
  <a href="/en/common/pngcrush.html">pngcrush</a> <a href="#pngcrush"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PNG image compression utility.
> More information: <https://pmt.sourceforge.io/pngcrush>.

#### Compress a PNG file:
```shell
pngcrush {{in.png}} {{out.png}}
```
#### Compress all PNGs and output to directory:
```shell
pngcrush -d {{path/to/output}} *.png
```
#### Compress PNG file with all 114 available algorithms and pick the best result:
```shell
pngcrush -rem allb -brute -reduce {{in.png}} {{out.png}}
```
{% endraw %}