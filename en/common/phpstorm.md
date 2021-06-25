---
layout: default
title: "phpstorm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpstorm">
  <a href="/en/common/phpstorm.html">phpstorm</a> <a href="#phpstorm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A cross-platform IDE for PHP based on the JetBrains IntelliJ platform.
> More information: <https://jetbrains.com/phpstorm>.

#### Open a specific directory:
```shell
phpstorm {{path/to/directory}}
```
#### Open a file:
```shell
phpstorm {{path/to/file}}
```
#### Open a file at a specific line:
```shell
phpstorm --line {{line_number}} {{path/to/file}}
```
#### View the differences between two files:
```shell
phpstorm diff {{path/to/left_file}} {{path/to/right_file}}
```
{% endraw %}