---
layout: default
title: "solo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="solo">
  <a href="/en/common/solo.html">solo</a> <a href="#solo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with Solo hardware security keys.
> More information: <https://github.com/solokeys/solo-python>.

#### List connected Solos:
```shell
solo ls
```
#### Update the currently connected Solo's firmware to the latest version:
```shell
solo key update
```
#### Blink the led of a specific Solo:
```shell
solo key wink --serial {{serial_number}}
```
#### Generate random bytes using the currently connected Solo's secure random number generator:
```shell
solo key rng raw
```
#### Monitor the serial output of a Solo:
```shell
solo monitor {{path/to/serial_port}}
```
{% endraw %}