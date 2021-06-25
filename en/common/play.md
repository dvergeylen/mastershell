---
layout: default
title: "play"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="play">
  <a href="/en/common/play.html">play</a> <a href="#play"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Audio player of SoX - Sound eXchange.
> Plays any audio from the command-line, with audio formats identified by the extension.
> More information: <http://sox.sourceforge.net>.

#### Play the given audio file:
```shell
play {{audiofile}}
```
#### Play the given audio files:
```shell
play {{audiofile1}} {{audiofile2}}
```
#### Play the given audio at twice the speed:
```shell
play {{audiofile}} speed 2.0
```
#### Play the given audio in reverse:
```shell
play {{audiofile}} reverse
```
{% endraw %}