---
layout: default
title: "amixer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amixer">
  <a href="/zh/linux/amixer.html">amixer</a> <a href="#amixer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ALSA 声卡驱动程序的混合器。

#### 增加 10% 的主音量：
```shell
amixer -D pulse sset Master {{10%+}}
```
#### 降低 10% 的主音量：
```shell
amixer -D pulse sset Master {{10%-}}
```
{% endraw %}