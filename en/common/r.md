---
layout: default
title: "R"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="r">
  <a href="/en/common/r.html">R</a> <a href="#r"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> R language interpreter.
> More information: <https://www.r-project.org>.

#### Start an R interactive shell (REPL):
```shell
R
```
#### Check R version:
```shell
R --version
```
#### Start R in vanilla mode (i.e. a blank session that doesn't save the workspace at the end):
```shell
R --vanilla
```
#### Execute a file:
```shell
R -f {{path/to/file.R}}
```
#### Execute an R expression and then exit:
```shell
R -e {{expr}}
```
#### Run R with a debugger:
```shell
R -d {{debugger}}
```
#### Check R packages from package sources:
```shell
R CMD check {{path/to/package_source}}
```
{% endraw %}