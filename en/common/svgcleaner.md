---
layout: default
title: "svgcleaner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svgcleaner">
  <a href="/en/common/svgcleaner.html">svgcleaner</a> <a href="#svgcleaner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SVG image optimizing utility.
> More information: <https://github.com/RazrFalcon/svgcleaner>.

#### Optimize an SVG image:
```shell
svgcleaner {{input.svg}} {{output.svg}}
```
#### Optimize an SVG image multiple times:
```shell
svgcleaner --multipass {{input.svg}} {{output.svg}}
```
{% endraw %}