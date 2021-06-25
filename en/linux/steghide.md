---
layout: default
title: "steghide"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="steghide">
  <a href="/en/linux/steghide.html">steghide</a> <a href="#steghide"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Steganography tool for JPEG, BMP, WAV and AU file formats.
> More information: <https://github.com/StefanoDeVuono/steghide>.

#### Embed data in a PNG image, prompting for a passphrase:
```shell
steghide embed --coverfile {{path/to/image.png}} --embedfile {{path/to/data.txt}}
```
#### Extract data from a WAV audio file:
```shell
steghide extract --stegofile {{path/to/sound.wav}}
```
#### Display file information, trying to detect an embedded file:
```shell
steghide info {{path/to/file.jpg}}
```
#### Embed data in a JPEG image, using maximum compression:
```shell
steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --compress {{9}}
```
#### Get the list of supported encryption algorithms and modes:
```shell
steghide encinfo
```
#### Embed encrypted data in a JPEG image, e.g. with Blowfish in CBC mode:
```shell
steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --encryption {{blowfish|...}} {{cbc|...}}
```
{% endraw %}