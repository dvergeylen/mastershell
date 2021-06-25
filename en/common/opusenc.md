---
layout: default
title: "opusenc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opusenc">
  <a href="/en/common/opusenc.html">opusenc</a> <a href="#opusenc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert WAV or FLAC audio to Opus.
> More information: <https://opus-codec.org/docs/opus-tools/opusenc.html>.

#### Convert WAV to Opus using default options:
```shell
opusenc {{path/to/input.wav}} {{path/to/output}}.opus
```
#### Convert stereo audio at the highest quality level:
```shell
opusenc --bitrate {{512}} {{path/to/input.wav}} {{path/to/output}}.opus
```
#### Convert 5.1 surround sound audio at the highest quality level:
```shell
opusenc --bitrate {{1536}} {{path/to/input.flac}} {{path/to/output}}.opus
```
#### Convert speech audio at the lowest quality level:
```shell
opusenc {{path/to/input.wav}} --downmix-mono --bitrate {{6}} {{path/to/out}}.opus
```
{% endraw %}