---
layout: default
title: "sha512sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha512sum">
  <a href="/en/common/sha512sum.html">sha512sum</a> <a href="#sha512sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate SHA512 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Calculate the SHA512 checksum for a file:
```shell
sha512sum {{filename1}}
```
#### Calculate SHA512 checksums for multiple files:
```shell
sha512sum {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA512 checksums to a file:
```shell
sha512sum {{filename1}} {{filename2}} > {{filename.sha512}}
```
#### Read a file of SHA512 sums and verify all files have matching checksums:
```shell
sha512sum --check {{filename.sha512}}
```
#### Only show a message for files for which verification fails:
```shell
sha512sum --check --quiet {{filename.sha512}}
```
{% endraw %}