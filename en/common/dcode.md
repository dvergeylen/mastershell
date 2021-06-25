---
layout: default
title: "dcode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dcode">
  <a href="/en/common/dcode.html">dcode</a> <a href="#dcode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recursively detect and decode strings, supporting hex, decimal, binary, base64, URL, FromChar encodings, Caesar ciphers, and MD5, SHA1, and SHA2 hashes.
> Warning: uses 3rd-party web services for MD5, SHA1 and SHA2 hash lookups. For sensitive data, use `-s` to avoid these services.
> More information: <https://github.com/s0md3v/Decodify>.

#### Recursively detect and decode a string:
```shell
dcode "{{NjM3YTQyNzQ1YTQ0NGUzMg==}}"
```
#### Rotate a string by the specified offset:
```shell
dcode -rot {{11}} "{{spwwz hzcwo}}"
```
#### Rotate a string by all 26 possible offsets:
```shell
dcode -rot {{all}} "{{bpgkta xh qtiitg iwpc sr}}"
```
#### Reverse a string:
```shell
dcode -rev "{{hello world}}"
```
{% endraw %}