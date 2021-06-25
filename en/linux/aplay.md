---
layout: default
title: "aplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aplay">
  <a href="/en/linux/aplay.html">aplay</a> <a href="#aplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line sound player for ALSA soundcard driver.
> More information: <https://manned.org/aplay>.

#### Play a specific file (sampling rate, bit depth, etc. will be automatically determined for the file format):
```shell
aplay {{path/to/file}}
```
#### Play the first 10 seconds of a specific file at 2500Hz:
```shell
aplay --duration={{10}} --rate={{2500}} {{path/to/file}}
```
#### Play the raw file as a 22050Hz, mono, 8-bit, Mu-Law `.au` file:
```shell
aplay --channels={{1}} --file-type {{raw}} --rate={{22050}} --format={{mu_law}} {{path/to/file}}
```
{% endraw %}