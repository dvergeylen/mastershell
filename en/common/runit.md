---
layout: default
title: "runit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runit">
  <a href="/en/common/runit.html">runit</a> <a href="#runit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 3-stage init system.
> More information: <https://wiki.archlinux.org/index.php/Runit>.

#### Start runit's 3-stage init scheme:
```shell
runit
```
#### Shut down runit:
```shell
kill --CONT {{runit_pid}}
```
{% endraw %}