---
layout: default
title: "uudecode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uudecode">
  <a href="/en/common/uudecode.html">uudecode</a> <a href="#uudecode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Decode files encoded by `uuencode`.
> More information: <https://manned.org/uudecode>.

#### Decode a file that was encoded with `uuencode` and print the result to stdout:
```shell
uudecode {{path/to/encoded_file}}
```
#### Decode a file that was encoded with `uuencode` and write the result to a file:
```shell
uudecode -o {{path/to/decoded_file}} {{path/to/encoded_file}}
```
{% endraw %}