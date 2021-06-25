---
layout: default
title: "phpdox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpdox">
  <a href="/en/common/phpdox.html">phpdox</a> <a href="#phpdox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP documentation generator.
> More information: <https://phpdox.net>.

#### Display an annotated skeleton configuration XML file:
```shell
phpdox --skel
```
#### Generate documentation for the current working directory:
```shell
phpdox
```
#### Generate documentation using a specific configuration file:
```shell
phpdox --file {{path/to/phpdox.xml}}
```
#### Only run the metadata collection process:
```shell
phpdox --collector
```
#### Only run the documentation generator process:
```shell
phpdox --generator
```
{% endraw %}