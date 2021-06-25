---
layout: default
title: "guetzli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="guetzli">
  <a href="/en/common/guetzli.html">guetzli</a> <a href="#guetzli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JPEG image compression utility.
> More information: <https://github.com/google/guetzli>.

#### Compress a JPEG image:
```shell
guetzli {{input.jpg}} {{output.jpg}}
```
#### Create compressed JPEG image from PNG image:
```shell
guetzli {{input.png}} {{output.jpg}}
```
#### Compress a JPEG image with desired visual quality (84-100):
```shell
guetzli --quality {{quality_value}} {{input.jpg}} {{output.jpg}}
```
{% endraw %}