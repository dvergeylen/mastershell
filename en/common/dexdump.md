---
layout: default
title: "dexdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dexdump">
  <a href="/en/common/dexdump.html">dexdump</a> <a href="#dexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Android DEX files.
> More information: <https://manpages.ubuntu.com/manpages/latest/en/man1/dexdump.1.html>.

#### Extract classes and methods from an APK file:
```shell
dexdump {{path/to/file.apk}}
```
#### Display header information of DEX files contained in an APK file:
```shell
dexdump -f {{path/to/file.apk}}
```
#### Display the dis-assembled output of executable sections:
```shell
dexdump -d {{path/to/file.apk}}
```
#### Output results to a file:
```shell
dexdump -o {{path/to/file}} {{path/to/file.apk}}
```
{% endraw %}