---
layout: default
title: "doctum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doctum">
  <a href="/en/common/doctum.html">doctum</a> <a href="#doctum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP API documentation generator.
> More information: <https://github.com/code-lts/doctum>.

#### Parse a project:
```shell
doctum parse
```
#### Render a project:
```shell
doctum render
```
#### Parse then render a project:
```shell
doctum update
```
#### Parse and render only a specific version of a project:
```shell
doctum update --only-version={{version}}
```
#### Parse and render a project using a specific configuration:
```shell
doctum update {{path/to/config.php}}
```
{% endraw %}