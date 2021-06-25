---
layout: default
title: "scheme"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scheme">
  <a href="/en/common/scheme.html">scheme</a> <a href="#scheme"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MIT Scheme language interpreter and REPL (interactive shell).
> More information: <https://www.gnu.org/software/mit-scheme>.

#### Open an interactive shell (REPL):
```shell
scheme
```
#### Run a scheme program (with no REPL output):
```shell
scheme --quiet < {{script.scm}}
```
#### Load a scheme program into the REPL:
```shell
scheme --load {{script.scm}}
```
#### Load scheme expressions into the REPL:
```shell
scheme --eval "{{(define foo 'x)}}"
```
#### Open the REPL in quiet mode:
```shell
scheme --quiet
```
{% endraw %}