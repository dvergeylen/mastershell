---
layout: default
title: "scanimage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scanimage">
  <a href="/en/linux/scanimage.html">scanimage</a> <a href="#scanimage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan images with the Scanner Access Now Easy API.
> More information: <http://sane-project.org/man/scanimage.1.html>.

#### List available scanners to ensure the target device is connected and recognized:
```shell
scanimage -L
```
#### Scan an image and save it to a file:
```shell
scanimage --format={{pnm|tiff|png|jpeg}} > {{path/to/new_image}}
```
{% endraw %}