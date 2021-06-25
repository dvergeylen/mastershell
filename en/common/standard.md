---
layout: default
title: "standard"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="standard">
  <a href="/en/common/standard.html">standard</a> <a href="#standard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The JavaScript Standard Style tool for linting and fixing JavaScript code.
> More information: <https://standardjs.com>.

#### Lint all JavaScript source files in the current directory:
```shell
standard
```
#### Lint specific JavaScript file(s):
```shell
standard {{path/to/file(s)}}
```
#### Apply automatic fixes during linting:
```shell
standard --fix
```
#### Declare any available global variables:
```shell
standard --global {{variable}}
```
#### Use a custom ESLint plugin when linting:
```shell
standard --plugin {{plugin}}
```
#### Use a custom JS parser when linting:
```shell
standard --parser {{parser}}
```
#### Use a custom ESLint environment when linting:
```shell
standard --env {{environment}}
```
{% endraw %}