---
layout: default
title: "anbox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="anbox">
  <a href="/en/linux/anbox.html">anbox</a> <a href="#anbox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run Android applications on any GNU/Linux operating system.
> More information: <https://manned.org/anbox>.

#### Launch Anbox into the app manager:
```shell
anbox launch --package={{org.anbox.appmgr}} --component={{org.anbox.appmgr.AppViewActivity}}
```
{% endraw %}