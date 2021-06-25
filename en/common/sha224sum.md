---
layout: default
title: "sha224sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha224sum">
  <a href="/en/common/sha224sum.html">sha224sum</a> <a href="#sha224sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate SHA224 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Calculate the SHA224 checksum for a file:
```shell
sha224sum {{filename1}}
```
#### Calculate SHA224 checksums for multiple files:
```shell
sha224sum {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA224 checksums to a file:
```shell
sha224sum {{filename1}} {{filename2}} > {{filename.sha224}}
```
#### Read a file of SHA224 sums and verify all files have matching checksums:
```shell
sha224sum --check {{filename.sha224}}
```
#### Only show a message for files for which verification fails:
```shell
sha224sum --check --quiet {{filename.sha224}}
```
{% endraw %}