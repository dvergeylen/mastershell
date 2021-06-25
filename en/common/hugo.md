---
layout: default
title: "hugo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hugo">
  <a href="/en/common/hugo.html">hugo</a> <a href="#hugo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Template-based static site generator. Uses modules, components, and themes.
> More information: <https://gohugo.io>.

#### Create a new Hugo site:
```shell
hugo new site {{path/to/site}}
```
#### Create a new Hugo theme (themes may also be downloaded from https://themes.gohugo.io/):
```shell
hugo new theme {{theme_name}}
```
#### Create a new page:
```shell
hugo new {{section_name}}/{{filename}}
```
#### Build a site to the `./public/` directory:
```shell
hugo
```
#### Build a site including pages that are marked as a "draft":
```shell
hugo --buildDrafts
```
#### Build a site to a given directory:
```shell
hugo --destination {{path/to/destination}}
```
#### Build a site, start up a webserver to serve it, and automatically reload when pages are edited:
```shell
hugo server
```
{% endraw %}