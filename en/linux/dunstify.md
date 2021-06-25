---
layout: default
title: "dunstify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dunstify">
  <a href="/en/linux/dunstify.html">dunstify</a> <a href="#dunstify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A notification tool that is an extension of notify-send, but has more features based around dunst.
> Works with all options that work for notify-send.

#### Show a notification with a given title and message:
```shell
dunstify "{{Title}}" "{{Message}}"
```
#### Show a notification with specified urgency:
```shell
dunstify "{{Title}}" "{{Message}}" -u {{low|normal|critical}}
```
#### Specify a message ID (overwrites any previous messages with the same ID):
```shell
dunstify "{{Title}}" "{{Message}}" -r {{123}}
```
#### To see other possible options:
```shell
notify-send --help
```
{% endraw %}