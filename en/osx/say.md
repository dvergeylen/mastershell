---
layout: default
title: "say"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="say">
  <a href="/en/osx/say.html">say</a> <a href="#say"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts text to speech.

#### Say a phrase aloud:
```shell
say "{{I like to ride my bike.}}"
```
#### Read a file aloud:
```shell
say -f {{filename.txt}}
```
#### Say a phrase with a custom voice and speech rate:
```shell
say -v {{voice}} -r {{words_per_minute}} "{{I'm sorry Dave, I can't let you do that.}}"
```
#### List the available voices:
```shell
say -v "?"
```
#### Create an audio file of the spoken text:
```shell
say -o {{filename.aiff}} "{{Here's to the Crazy Ones.}}"
```
{% endraw %}