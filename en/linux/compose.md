---
layout: default
title: "compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compose">
  <a href="/en/linux/compose.html">compose</a> <a href="#compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action compose.
> Originally `run-mailcap` is used to mime-type/file.

#### Compose action can be used to compose any existing file or new on default mailcap edit tool:
```shell
compose {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=compose {{filename}}
```
{% endraw %}