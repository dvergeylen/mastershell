---
layout: default
title: "pup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pup">
  <a href="/en/common/pup.html">pup</a> <a href="#pup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line HTML parsing tool.
> More information: <https://github.com/ericchiang/pup>.

#### Transform a raw HTML file into a cleaned, indented, and colored format:
```shell
cat {{index.html}} | pup --color
```
#### Filter HTML by element tag name:
```shell
cat {{index.html}} | pup '{{tag}}'
```
#### Filter HTML by id:
```shell
cat {{index.html}} | pup '{{div#id}}'
```
#### Filter HTML by attribute value:
```shell
cat {{index.html}} | pup '{{input[type="text"]}}'
```
#### Print all text from the filtered HTML elements and their children:
```shell
cat {{index.html}} | pup '{{div}} text{}'
```
#### Print HTML as JSON:
```shell
cat {{index.html}} | pup '{{div}} json{}'
```
{% endraw %}