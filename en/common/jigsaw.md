---
layout: default
title: "jigsaw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jigsaw">
  <a href="/en/common/jigsaw.html">jigsaw</a> <a href="#jigsaw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Laravel-based static site builder for PHP.
> More information: <https://jigsaw.tighten.co>.

#### Initialise a project:
```shell
jigsaw init
```
#### Initialise a project using a starter template:
```shell
jigsaw init {{template_name}}
```
#### Build the site for development:
```shell
jigsaw build
```
#### Preview the site from the "build_local" directory:
```shell
jigsaw serve
```
#### Build the site for production:
```shell
jigsaw build production
```
#### Preview the site from the "build_production" directory:
```shell
jigsaw serve {{build_production}}
```
{% endraw %}