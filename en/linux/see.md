---
layout: default
title: "see"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="see">
  <a href="/en/linux/see.html">see</a> <a href="#see"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alias to `run-mailcap`'s view.
> An alias to a `run-mailcap`'s action print.

#### See action can be used to view any file (usually image) on default mailcap explorer:
```shell
see {{filename}}
```
#### Using with `run-mailcap`:
```shell
run-mailcap --action=view {{filename}}
```
{% endraw %}