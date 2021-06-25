---
layout: default
title: "amixer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amixer">
  <a href="/en/linux/amixer.html">amixer</a> <a href="#amixer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mixer for ALSA soundcard driver.

#### Turn up the master volume by 10%:
```shell
amixer -D pulse sset Master {{10%+}}
```
#### Turn down the master volume by 10%:
```shell
amixer -D pulse sset Master {{10%-}}
```
{% endraw %}