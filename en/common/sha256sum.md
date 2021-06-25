---
layout: default
title: "sha256sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha256sum">
  <a href="/en/common/sha256sum.html">sha256sum</a> <a href="#sha256sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate SHA256 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Calculate the SHA256 checksum for a file:
```shell
sha256sum {{filename1}}
```
#### Calculate SHA256 checksums for multiple files:
```shell
sha256sum {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA256 checksums to a file:
```shell
sha256sum {{filename1}} {{filename2}} > {{filename.sha256}}
```
#### Read a file of SHA256 sums and verify all files have matching checksums:
```shell
sha256sum --check {{filename.sha256}}
```
#### Only show a message for files for which verification fails:
```shell
sha256sum --check --quiet {{filename.sha256}}
```
{% endraw %}