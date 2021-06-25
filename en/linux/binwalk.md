---
layout: default
title: "binwalk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="binwalk">
  <a href="/en/linux/binwalk.html">binwalk</a> <a href="#binwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Firmware Analysis Tool.
> More information: <https://github.com/ReFirmLabs/binwalk>.

#### Scan a binary file:
```shell
binwalk {{path/to/binary}}
```
#### Extract files from a binary, specifying the output directory:
```shell
binwalk --extract --directory {{output_directory}} {{path/to/binary}}
```
#### Recursively extract files from a binary limiting the recursion depth to 2:
```shell
binwalk --extract --matryoshka --depth {{2}} {{path/to/binary}}
```
#### Extract files from a binary with the specified file signature:
```shell
binwalk --dd '{{png image:png}}' {{path/to/binary}}
```
#### Analyze the entropy of a binary, saving the plot with the same name as the binary and `.png` extension appended:
```shell
binwalk --entropy --save {{path/to/binary}}
```
#### Combine entropy, signature and opcodes analysis in a single command:
```shell
binwalk --entropy --signature --opcodes {{path/to/binary}}
```
{% endraw %}