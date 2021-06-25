---
layout: default
title: "pickle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pickle">
  <a href="/en/common/pickle.html">pickle</a> <a href="#pickle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP extension installer based on Composer.
> More information: <https://github.com/FriendsOfPHP/pickle>.

#### Install a specific PHP extension:
```shell
pickle install {{extension_name}}
```
#### Convert an existing PECL extension configuration to a Pickle configuration file:
```shell
pickle convert {{path/to/directory}}
```
#### Validate a PECL extension:
```shell
pickle validate {{path/to/directory}}
```
#### Package a PECL extension for release:
```shell
pickle release {{path/to/directory}}
```
{% endraw %}