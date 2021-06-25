---
layout: default
title: "case"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="case">
  <a href="/en/common/case.html">case</a> <a href="#case"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Branch based on the value of an expression.
> More information: <https://manned.org/case>.

#### Match a variable against string literals to decide which command to run:
```shell
case {{$tocount}} in {{words}}) {{wc -w README}}; ;; {{lines}}) {{wc -l README}}; ;; esac
```
#### Combine patterns with |, use * as a fallback pattern:
```shell
case {{$tocount}} in {{[wW]|words}}) {{wc -w README}}; ;; {{[lL]|lines}}) {{wc -l README}}; ;; *) {{echo "what?"}}; ;; esac
```
{% endraw %}