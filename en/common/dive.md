---
layout: default
title: "dive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dive">
  <a href="/en/common/dive.html">dive</a> <a href="#dive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for exploring a Docker image, layer contents, and discovering ways to shrink it.
> More information: <https://github.com/wagoodman/dive>.

#### Analyze a Docker image:
```shell
dive {{your_image_tag}}
```
#### Build an image and start analyzing it:
```shell
dive build -t {{some_tag}}
```
{% endraw %}