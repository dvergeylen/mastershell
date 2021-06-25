---
layout: default
title: "import"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="import">
  <a href="/en/common/import.html">import</a> <a href="#import"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Capture some or all of an X server screen, and save the image to a file.
> Part of the ImageMagick library.

#### Capture the entire X server screen in the PostScript image format:
```shell
import -window root {{output.postscript}}
```
#### Capture contents of a remote X server screen in the PNG image format:
```shell
import -window root -display {{remote_host}}:{screen}.{display} {{output.png}}
```
#### Capture a specific window, given its ID as displayed by `xwininfo`, into the JPEG format:
```shell
import -window {{window_id}} {{output.jpg}}
```
{% endraw %}