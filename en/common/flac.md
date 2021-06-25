---
layout: default
title: "flac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flac">
  <a href="/en/common/flac.html">flac</a> <a href="#flac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encodes, decodes and tests flac files.
> More information: <https://xiph.org/flac>.

#### Encode a wav file to flac (this will create a flac file in the same location as the wav file):
```shell
flac {{path/to/file.wav}}
```
#### Encode a wav file to flac, specifying the output file:
```shell
flac -o {{path/to/output.flac}} {{path/to/file.wav}}
```
#### Decode a flac file to wav, specifying the output file:
```shell
flac -d -o {{path/to/output.wav}} {{path/to/file.flac}}
```
#### Test a flac file for the correct encoding:
```shell
flac -t {{path/to/file.flac}}
```
{% endraw %}