---
layout: default
title: "mesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mesg">
  <a href="/en/common/mesg.html">mesg</a> <a href="#mesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check or set a terminal's ability to receive messages from other users, usually from the write command.
> See also `write`.

#### Check terminal's openness to write messages:
```shell
mesg
```
#### Disable receiving messages from the write command:
```shell
mesg n
```
#### Enable receiving messages from the write command:
```shell
mesg y
```
{% endraw %}