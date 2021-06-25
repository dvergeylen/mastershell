---
layout: default
title: "csslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csslint">
  <a href="/en/common/csslint.html">csslint</a> <a href="#csslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A linter for CSS code.
> More information: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

#### Lint a single CSS file:
```shell
csslint {{file.css}}
```
#### Lint multiple CSS files:
```shell
csslint {{file1.css}} {{file2.css}} {{file3.css}}
```
#### List all possible style rules:
```shell
csslint --list-rules
```
#### Specify certain rules as errors (which result in a non-zero exit code):
```shell
csslint --errors={{errors,universal-selector,imports}} {{file.css}}
```
#### Specify certain rules as warnings:
```shell
csslint --warnings={{box-sizing,selector-max,floats}} {{file.css}}
```
#### Specify certain rules to completely ignore:
```shell
csslint --ignore={{ids,rules-count,shorthand}} {{file.css}}
```
{% endraw %}