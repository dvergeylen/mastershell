---
layout: default
title: "nativefier"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nativefier">
  <a href="/en/common/nativefier.html">nativefier</a> <a href="#nativefier"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to create a desktop app for any web site with minimal configuration.
> More information: <https://github.com/jiahaog/nativefier>.

#### Make a desktop app for a website:
```shell
nativefier {{url}}
```
#### Create a desktop app with a custom name:
```shell
nativefier --name {{name}} {{url}}
```
#### Use a custom icon, should be a PNG:
```shell
nativefier --icon {{path/to/icon.png}} {{url}}
```
{% endraw %}