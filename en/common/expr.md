---
layout: default
title: "expr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expr">
  <a href="/en/common/expr.html">expr</a> <a href="#expr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Evaluate expressions and manipulate strings.
> More information: <https://www.gnu.org/software/coreutils/expr>.

#### Get string length:
```shell
expr length {{string}}
```
#### Evaluate logical or math expression with an operator ('+', '-', '*', '&', '|', etc.). Special symbols should be escaped:
```shell
expr {{first_argument}} {{operator}} {{second_argument}}
```
#### Get position of the first character in 'string' that matches 'substring':
```shell
echo $(expr index {{string}} {{substring}})
```
#### Extract part of the string:
```shell
echo $(expr substr {{string}} {{position_to_start}} {{number_of_characters}}
```
#### Extract part of the string which matches a regular expression:
```shell
echo $(expr {{string}} : '\({{regular_expression}}\)')
```
{% endraw %}