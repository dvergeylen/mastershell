---
layout: default
title: "radeontop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="radeontop">
  <a href="/en/linux/radeontop.html">radeontop</a> <a href="#radeontop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show utilisation of AMD GPUs.
> More information: <https://github.com/clbr/radeontop>.

#### Show the utilisation of the default AMD GPU:
```shell
sudo radeontop
```
#### Enable colourised output:
```shell
sudo radeontop --colour
```
#### Select a specific GPU (the bus number is the first number in the output of `lspci`):
```shell
sudo radeontop --bus {{bus_number}}
```
#### Specify the display refresh rate (higher means more GPU overhead):
```shell
sudo radeontop --ticks {{samples_per_second}}
```
{% endraw %}