---
layout: default
title: "xxd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xxd">
  <a href="/en/common/xxd.html">xxd</a> <a href="#xxd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a hexadecimal representation (hexdump) from a binary file, or vice-versa.

#### Generate a hexdump from a binary file and display the output:
```shell
xxd {{input_file}}
```
#### Generate a hexdump from a binary file and save it as a text file:
```shell
xxd {{input_file}} {{output_file}}
```
#### Display a more compact output, replacing consecutive zeros (if any) with a star:
```shell
xxd -a {{input_file}}
```
#### Display the output with 10 columns of one octet (byte) each:
```shell
xxd -c {{10}} {{input_file}}
```
#### Display output only up to a length of 32 bytes:
```shell
xxd -l {{32}} {{input_file}}
```
#### Display the output in plain mode, without any gaps between the columns:
```shell
xxd -p {{input_file}}
```
#### Revert a plaintext hexdump back into binary, and save it as a binary file:
```shell
xxd -r -p {{input_file}} {{output_file}}
```
{% endraw %}