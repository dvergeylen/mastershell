---
layout: default
title: "sox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sox">
  <a href="/en/common/sox.html">sox</a> <a href="#sox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sound eXchange: play, record and convert audio files.
> Audio formats are identified by the extension.
> More information: <http://sox.sourceforge.net>.

#### Merge two audio files into one:
```shell
sox -m {{input_audiofile1}} {{input_audiofile2}} {{output_audiofile}}
```
#### Trim an audio file to the specified times:
```shell
sox {{input_audiofile}} {{output_audiofile}} trim {{start}} {{end}}
```
#### Normalize an audio file (adjust volume to the maximum peak level, without clipping):
```shell
sox --norm {{input_audiofile}} {{output_audiofile}}
```
#### Reverse and save an audio file:
```shell
sox {{input_audiofile}} {{output_audiofile}} reverse
```
#### Print statistical data of an audio file:
```shell
sox {{input_audiofile}} -n stat
```
#### Increase the volume of an audio file by 2x:
```shell
sox -v 2.0 {{input_audiofile}} {{output_audiofile}}
```
{% endraw %}