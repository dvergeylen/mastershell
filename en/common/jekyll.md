---
layout: default
title: "jekyll"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jekyll">
  <a href="/en/common/jekyll.html">jekyll</a> <a href="#jekyll"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple, blog-aware, static site generator.
> More information: <https://jekyllrb.com>.

#### Generate a development server that will run at http://localhost:4000/:
```shell
jekyll serve
```
#### Enable incremental regeneration:
```shell
jekyll serve --incremental
```
#### Enable verbose output:
```shell
jekyll serve --verbose
```
#### Generate the current directory into `./_site`:
```shell
jekyll build
```
#### Clean the site (removes site output and `cache` directory) without building:
```shell
jekyll clean
```
{% endraw %}