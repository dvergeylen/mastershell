---
layout: default
title: "uuencode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uuencode">
  <a href="/en/common/uuencode.html">uuencode</a> <a href="#uuencode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode binary files into ASCII for transport via mediums that only support simple ASCII encoding.
> More information: <https://manned.org/uuencode>.

#### Encode a file and print the result to stdout:
```shell
uuencode {{path/to/input_file}} {{output_file_name_after_decoding}}
```
#### Encode a file and and write the result to a file:
```shell
uuencode -o {{path/to/output_file}} {{path/to/input_file}} {{output_file_name_after_decoding}}
```
#### Encode a file using Base64 instead of the default uuencode encoding and and write the result to a file:
```shell
uuencode -m -o {{path/to/output_file}} {{path/to/input_file}} {{output_file_name_after_decoding}}
```
{% endraw %}