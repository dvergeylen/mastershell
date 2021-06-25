---
layout: default
title: "jar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jar">
  <a href="/en/common/jar.html">jar</a> <a href="#jar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Applications/Libraries Packager.
> More information: <https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

#### Recursively archive all files in the current directory into a .jar file:
```shell
jar cf {{file.jar}} *
```
#### Unzip .jar/.war file to the current directory:
```shell
jar -xvf {{file.jar}}
```
#### List a .jar/.war file content:
```shell
jar tf {{path/to/file.jar}}
```
#### List a .jar/.war file content with verbose output:
```shell
jar tvf {{path/to/file.jar}}
```
{% endraw %}