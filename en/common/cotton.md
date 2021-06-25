---
layout: default
title: "cotton"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cotton">
  <a href="/en/common/cotton.html">cotton</a> <a href="#cotton"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Markdown test specification runner.
> More information: <https://github.com/chonla/cotton>.

#### Use a specific base URL:
```shell
cotton -u {{base_url}} {{file}}.md
```
#### Disable certificate verification (insecure mode):
```shell
cotton -u {{base_url}} -i {{file}}.md
```
#### Stop running when a test fails:
```shell
cotton -u {{base_url}} -s {{file}}.md
```
{% endraw %}