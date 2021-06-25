---
layout: default
title: "zopflipng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zopflipng">
  <a href="/en/common/zopflipng.html">zopflipng</a> <a href="#zopflipng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PNG image compression utility.
> More information: <https://github.com/google/zopfli>.

#### Optimize a PNG image:
```shell
zopflipng {{input.png}} {{output.png}}
```
#### Optimize several PNG images and save with given prefix:
```shell
zopflipng --prefix={{prefix}} {{image1.png}} {{image2.png}} {{image3.png}}
```
{% endraw %}