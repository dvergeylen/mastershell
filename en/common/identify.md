---
layout: default
title: "identify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="identify">
  <a href="/en/common/identify.html">identify</a> <a href="#identify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line utility of Image Magick project to describe the format and characteristics of one or more image files.
> More information: <https://imagemagick.org/script/identify.php>.

#### Collect dimensions of all jpeg files under current directory:
```shell
identify -format "%f,%w,%h\n" *.{{jpg}} > {{filelist.csv}}
```
{% endraw %}