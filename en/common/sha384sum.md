---
layout: default
title: "sha384sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha384sum">
  <a href="/en/common/sha384sum.html">sha384sum</a> <a href="#sha384sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate SHA384 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Calculate the SHA384 checksum for a file:
```shell
sha384sum {{filename1}}
```
#### Calculate SHA384 checksums for multiple files:
```shell
sha384sum {{filename1}} {{filename2}}
```
#### Calculate and save the list of SHA384 checksums to a file:
```shell
sha384sum {{filename1}} {{filename2}} > {{filename.sha384}}
```
#### Read a file of SHA384 sums and verify all files have matching checksums:
```shell
sha384sum --check {{filename.sha384}}
```
#### Only show a message for files for which verification fails:
```shell
sha384sum --check --quiet {{filename.sha384}}
```
{% endraw %}