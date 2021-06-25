---
layout: default
title: "terminalizer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="terminalizer">
  <a href="/en/common/terminalizer.html">terminalizer</a> <a href="#terminalizer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility program which records the terminal and generate animated gifs or share a video.
> More information: <https://terminalizer.com>.

#### Create the global config directory:
```shell
terminalizer init
```
#### Record the terminal and create a recording file:
```shell
terminalizer record {{filename}}
```
#### Play a recorded file on the terminal:
```shell
terminalizer play {{filename}}
```
#### Render a recording file as an animated gif image:
```shell
terminalizer render {{filename}}
```
#### Upload a video to terminalizer.com:
```shell
terminalizer share {{filename}}
```
{% endraw %}