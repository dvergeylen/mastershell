---
layout: default
title: "sponge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sponge">
  <a href="/en/common/sponge.html">sponge</a> <a href="#sponge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Soak up the input before writing the output file.
> More information: <https://manned.org/sponge>.

#### Append file content to the source file:
```shell
cat {{path/to/file}} | sponge -a {{path/to/file}}
```
#### Remove all lines starting with # in a file:
```shell
grep -v '^{{#}}' {{path/to/file}} | sponge {{path/to/file}}
```
{% endraw %}