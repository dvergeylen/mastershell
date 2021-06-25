---
layout: default
title: "tslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tslint">
  <a href="/en/common/tslint.html">tslint</a> <a href="#tslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pluggable linting utility for TypeScript.
> More information: <https://palantir.github.io/tslint>.

#### Create tslint config:
```shell
tslint --init
```
#### Lint on a given set of files:
```shell
tslint {{filename}}.js {{filename1}}.js
```
#### Fix lint issues:
```shell
tslint --fix
```
#### Lint with the config file in the project root:
```shell
tslint --project {{path/to/project_root}}
```
{% endraw %}