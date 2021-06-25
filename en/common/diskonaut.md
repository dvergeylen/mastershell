---
layout: default
title: "diskonaut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diskonaut">
  <a href="/en/common/diskonaut.html">diskonaut</a> <a href="#diskonaut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal disk space navigator, written in Rust.
> More information: <https://github.com/imsnif/diskonaut>.

#### Start diskonaut in the current directory:
```shell
diskonaut
```
#### Start diskonaut in a specific directory:
```shell
diskonaut {{path/to/directory}}
```
#### Show file sizes rather than their block usage on the disk:
```shell
diskonaut --apparent-size {{path/to/directory}}
```
#### Disable deletion confirmation:
```shell
diskonaut --disable-delete-confirmation
```
{% endraw %}