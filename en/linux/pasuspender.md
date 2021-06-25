---
layout: default
title: "pasuspender"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pasuspender">
  <a href="/en/linux/pasuspender.html">pasuspender</a> <a href="#pasuspender"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Temporarily suspends `pulseaudio` while another command is running to allow access to alsa.

#### Suspend pulseaudio while running `jackd`:
```shell
pasuspender -- {{jackd -d alsa --device hw:0}}
```
{% endraw %}