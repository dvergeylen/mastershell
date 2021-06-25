---
layout: default
title: "jenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jenv">
  <a href="/en/common/jenv.html">jenv</a> <a href="#jenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to manage the "JAVA_HOME" environment variable.
> More information: <https://www.jenv.be/>.

#### Add a java version to jEnv:
```shell
jenv add {{path/to/jdk_home}}
```
#### Display the current JDK version used:
```shell
jenv version
```
#### Display all managed JDKs:
```shell
jenv versions
```
#### Set the global JDK version:
```shell
jenv global {{java_version}}
```
#### Set the JDK version for the current shell session:
```shell
jenv shell {{java_version}}
```
#### Enable a jEnv plugin:
```shell
jenv enable-plugin {{plugin_name}}
```
{% endraw %}