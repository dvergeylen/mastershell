---
layout: default
title: "apropos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apropos">
  <a href="/en/common/apropos.html">apropos</a> <a href="#apropos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search the manual pages for names and descriptions.
> More information: <https://manned.org/apropos>.

#### Search for a keyword using a regular expression:
```shell
apropos {{regular_expression}}
```
#### Search without restricting the output to the terminal width:
```shell
apropos -l {{regular_expression}}
```
#### Search for pages that contain all of the expressions given:
```shell
apropos {{regular_expression_1}} -a {{regular_expression_2}} -a {{regular_expression_3}}
```
{% endraw %}