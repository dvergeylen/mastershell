---
layout: default
title: "xattr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xattr">
  <a href="/en/osx/xattr.html">xattr</a> <a href="#xattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to work with extended filesystem attributes.

#### List key:value extended attributes for a given file:
```shell
xattr -l {{file}}
```
#### Write an attribute for a given file:
```shell
xattr -w {{attribute_key}} {{attribute_value}} {{file}}
```
#### Delete an attribute from a given file:
```shell
xattr -d {{com.apple.quarantine}} {{file}}
```
#### Delete all extended attributes from a given file:
```shell
xattr -c {{file}}
```
#### Recursively delete an attribute in a given directory:
```shell
xattr -rd {{attribute_key}} {{directory}}
```
{% endraw %}