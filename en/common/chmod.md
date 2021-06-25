---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/en/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the access permissions of a file or directory.
> More information: <https://www.gnu.org/software/coreutils/chmod>.

#### Give the [u]ser who owns a file the right to e[x]ecute it:
```shell
chmod u+x {{file}}
```
#### Give the [u]ser rights to [r]ead and [w]rite to a file/directory:
```shell
chmod u+rw {{file_or_directory}}
```
#### Remove e[x]ecutable rights from the [g]roup:
```shell
chmod g-x {{file}}
```
#### Give [a]ll users rights to [r]ead and e[x]ecute:
```shell
chmod a+rx {{file}}
```
#### Give [o]thers (not in the file owner's group) the same rights as the [g]roup:
```shell
chmod o=g {{file}}
```
#### Remove all rights from [o]thers:
```shell
chmod o= {{file}}
```
#### Change permissions recursively giving [g]roup and [o]thers the ability to [w]rite:
```shell
chmod -R g+w,o+w {{directory}}
```
{% endraw %}