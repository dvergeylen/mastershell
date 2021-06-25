---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/en/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode or decode file or standard input to/from Base32, to standard output.
> More information: <https://www.gnu.org/software/coreutils/base32>.

#### Encode a file:
```shell
base32 {{filename}}
```
#### Decode a file:
```shell
base32 --decode {{filename}}
```
#### Encode from stdin:
```shell
{{somecommand}} | base32
```
#### Decode from stdin:
```shell
{{somecommand}} | base32 --decode
```
{% endraw %}