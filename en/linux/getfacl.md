---
layout: default
title: "getfacl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getfacl">
  <a href="/en/linux/getfacl.html">getfacl</a> <a href="#getfacl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get file access control lists.

#### Display the file access control list:
```shell
getfacl {{path/to/file_or_directory}}
```
#### Display the file access control list with numeric user and group IDs:
```shell
getfacl -n {{path/to/file_or_directory}}
```
#### Display the file access control list with tabular output format:
```shell
getfacl -t {{path/to/file_or_directory}}
```
{% endraw %}