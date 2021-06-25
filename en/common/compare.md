---
layout: default
title: "compare"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compare">
  <a href="/en/common/compare.html">compare</a> <a href="#compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View the difference between 2 images.
> More information: <https://imagemagick.org/script/compare.php>.

#### Compare 2 images:
```shell
compare {{image1.png}} {{image2.png}} {{diff.png}}
```
#### Compare 2 images using a custom metric:
```shell
compare -verbose -metric {{PSNR}} {{image1.png}} {{image2.png}} {{diff.png}}
```
{% endraw %}