---
layout: default
title: "shasum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shasum">
  <a href="/en/common/shasum.html">shasum</a> <a href="#shasum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate or check cryptographic SHA checksums.

#### Calculate the SHA1 checksum for a file:
```shell
shasum {{filename}}
```
#### Calculate the SHA256 checksum for a file:
```shell
shasum --algorithm 256 {{filename}}
```
#### Calculate the SHA512 checksum for multiple files:
```shell
shasum --algorithm 512 {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA256 checksums to a file:
```shell
shasum --algorithm 256 {{filename1}} {{filename2}} > {{filename.sha256}}
```
#### Check a file with a list of sums against the directory's files:
```shell
shasum --check {{list_file}}
```
#### Check a list of sums and only show a message for files for which verification fails:
```shell
shasum --check --quiet {{list_file}}
```
#### Calculate the SHA1 checksum from stdin:
```shell
{{somecommand}} | shasum
```
{% endraw %}