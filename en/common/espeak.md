---
layout: default
title: "espeak"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="espeak">
  <a href="/en/common/espeak.html">espeak</a> <a href="#espeak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uses text-to-speech to speak through the default sound device.
> More information: <http://espeak.sourceforge.net>.

#### Speak a phrase aloud:
```shell
espeak "I like to ride my bike."
```
#### Speak a file aloud:
```shell
espeak -f {{filename}}
```
#### Save output to a WAV audio file, rather than speaking it directly:
```shell
espeak -w {{filename.wav}} "It's GNU plus Linux"
```
#### Use a different voice:
```shell
espeak -v {{voice}}
```
{% endraw %}