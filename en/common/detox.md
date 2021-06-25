---
layout: default
title: "detox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="detox">
  <a href="/en/common/detox.html">detox</a> <a href="#detox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Renames files to make them easier to work with.
> It removes spaces and other such annoyances like duplicate underline characters.
> More information: <https://github.com/dharple/detox>.

#### Remove spaces and other undesirable characters from a file's name:
```shell
detox {{file}}
```
#### Show how detox would rename all of the files in a directory tree:
```shell
detox --dry-run -r {{directory}}
```
#### Remove spaces and other undesirable characters from all files in a directory tree:
```shell
detox -r {{directory}}
```
{% endraw %}