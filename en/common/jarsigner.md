---
layout: default
title: "jarsigner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jarsigner">
  <a href="/en/common/jarsigner.html">jarsigner</a> <a href="#jarsigner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sign and verify Java Archive (JAR) files.
> More information: <https://docs.oracle.com/javase/9/tools/jarsigner.htm>.

#### Sign a JAR file:
```shell
jarsigner {{path/to/file.jar}} {{keystore_alias}}
```
#### Sign a JAR file with a specific algorithm:
```shell
jarsigner -sigalg {{algorithm}} {{path/to/file.jar}} {{keystore_alias}}
```
#### Verify the signature of a JAR file:
```shell
jarsigner -verify {{path/to/file.jar}}
```
{% endraw %}