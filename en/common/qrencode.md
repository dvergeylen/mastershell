---
layout: default
title: "qrencode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qrencode">
  <a href="/en/common/qrencode.html">qrencode</a> <a href="#qrencode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> QR Code generator. Supports PNG and EPS.
> More information: <https://fukuchi.org/works/qrencode>.

#### Convert a string to a QR code and save to an output file:
```shell
qrencode -o {{path/to/output_file.png}} {{string}}
```
#### Convert an input file to a QR code and save to an output file:
```shell
qrencode -o {{path/to/output_file.png}} -r {{path/to/input_file}}
```
#### Convert a string to a QR code and print it in terminal:
```shell
qrencode -t ansiutf8 {{string}}
```
#### Convert input from pipe to a QR code and print it in terminal:
```shell
echo {{string}} | qrencode -t ansiutf8
```
{% endraw %}