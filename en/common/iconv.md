---
layout: default
title: "iconv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iconv">
  <a href="/en/common/iconv.html">iconv</a> <a href="#iconv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts text from one encoding to another.

#### Convert file to a specific encoding, and print to stdout:
```shell
iconv -f {{from_encoding}} -t {{to_encoding}} {{input_file}}
```
#### Convert file to the current locale's encoding, and output to a file:
```shell
iconv -f {{from_encoding}} {{input_file}} > {{output_file}}
```
#### List supported encodings:
```shell
iconv -l
```
{% endraw %}