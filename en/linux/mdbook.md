---
layout: default
title: "mdbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdbook">
  <a href="/en/linux/mdbook.html">mdbook</a> <a href="#mdbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create online books by writing makrdown files.
> More information: <https://rust-lang.github.io/mdBook/>.

#### Create a mdbook project in the current directory:
```shell
mdbook init
```
#### Create a mdbook project in a specific directory:
```shell
mdbook init {{path/to/directory}}
```
#### Clean the directory with the generated book:
```shell
mdbook clean
```
#### Serve a book at `http://localhost:3000`, auto build when file changes:
```shell
mdbook serve
```
#### Watch a set of Markdown files and automatically build when a file is changed:
```shell
mdbook watch
```
{% endraw %}