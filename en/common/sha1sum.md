---
layout: default
title: "sha1sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha1sum">
  <a href="/en/common/sha1sum.html">sha1sum</a> <a href="#sha1sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate SHA1 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/sha1sum>.

#### Calculate the SHA1 checksum for a file:
```shell
sha1sum {{filename1}}
```
#### Calculate SHA1 checksums for multiple files:
```shell
sha1sum {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA1 checksums to a file:
```shell
sha1sum {{filename1}} {{filename2}} > {{filename.sha1}}
```
#### Read a file of SHA1 sums and verify all files have matching checksums:
```shell
sha1sum --check {{filename.sha1}}
```
#### Only show a message for files for which verification fails:
```shell
sha1sum --check --quiet {{filename.sha1}}
```
{% endraw %}