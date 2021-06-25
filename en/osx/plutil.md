---
layout: default
title: "plutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="plutil">
  <a href="/en/osx/plutil.html">plutil</a> <a href="#plutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, convert, validate, or edit property list ("plist") files.

#### Display the contents of one or more plist files in human-readable format:
```shell
plutil -p {{file1.plist file2.plist ...}}
```
#### Convert one or more plist files to XML format, overwriting the original files in-place:
```shell
plutil -convert xml1 {{file1.plist file2.plist ...}}
```
#### Convert one or more plist files to binary format, overwriting the original files in-place:
```shell
plutil -convert binary1 {{file1.plist file2.plist ...}}
```
#### Convert a plist file to a different format, writing to a new file:
```shell
plutil -convert {{xml1|binary1|json|swift|objc}} {{path/to/file.plist}} -o {{path/to/new_file.plist}}
```
#### Convert a plist file to a different format, writing to stdout:
```shell
plutil -convert {{xml1|binary1|json|swift|objc}} {{path/to/file.plist}} -o -
```
{% endraw %}