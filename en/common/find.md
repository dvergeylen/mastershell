---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/en/common/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find files or directories under the given directory tree, recursively.
> More information: <https://manned.org/find>.

#### Find files by extension:
```shell
find {{root_path}} -name '{{*.ext}}'
```
#### Find files matching multiple path/name patterns:
```shell
find {{root_path}} -path '{{**/path/**/*.ext}} -or -name '{{*pattern*}}'
```
#### Find directories matching a given name, in case-insensitive mode:
```shell
find {{root_path}} -type d -iname '{{*lib*}}'
```
#### Find files matching a given pattern, excluding specific paths:
```shell
find {{root_path}} -name '{{*.py}}' -not -path '{{*/site-packages/*}}'
```
#### Find files matching a given size range:
```shell
find {{root_path}} -size {{+500k}} -size {{-10M}}
```
#### Run a command for each file (use `{}` within the command to access the filename):
```shell
find {{root_path}} -name '{{*.ext}}' -exec {{wc -l {} }}\;
```
#### Find files modified in the last 7 days and delete them:
```shell
find {{root_path}} -mtime -{{7}} -delete
```
#### Find empty (0 byte) files and delete them:
```shell
find {{root_path}} -type {{f}} -empty -delete
```
{% endraw %}