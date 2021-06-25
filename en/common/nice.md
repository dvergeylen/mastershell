---
layout: default
title: "nice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nice">
  <a href="/en/common/nice.html">nice</a> <a href="#nice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a program with a custom scheduling priority (niceness).
> Niceness values range from -20 (the highest priority) to 19 (the lowest).
> More information: <https://www.gnu.org/software/coreutils/nice>.

#### Launch a program with altered priority:
```shell
nice -n {{niceness_value}} {{command}}
```
{% endraw %}