---
layout: default
title: "arch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arch">
  <a href="/en/osx/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the name of the system architecture, or run a command under a different architecture.
> See also `uname`.

#### Display the system's architecture:
```shell
arch
```
#### Run a command using x86_64:
```shell
arch -x86_64 {{command}}
```
{% endraw %}