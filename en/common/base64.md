---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/en/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode or decode file or standard input to/from Base64, to standard output.
> More information: <https://www.gnu.org/software/coreutils/base64>.

#### Encode the contents of a file as base64 and write the result to stdout:
```shell
base64 {{filename}}
```
#### Decode the base64 contents of a file and write the result to stdout:
```shell
base64 --decode {{filename}}
```
#### Encode from stdin:
```shell
{{somecommand}} | base64
```
#### Decode from stdin:
```shell
{{somecommand}} | base64 --decode
```
{% endraw %}