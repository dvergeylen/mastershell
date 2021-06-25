---
layout: default
title: "printenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="printenv">
  <a href="/en/common/printenv.html">printenv</a> <a href="#printenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print values of all or specific environment variables.
> More information: <https://www.gnu.org/software/coreutils/printenv>.

#### Display key-value pairs of all environment variables:
```shell
printenv
```
#### Display the value of a specific variable:
```shell
printenv {{HOME}}
```
#### Display the value of a variable and end with NUL instead of newline:
```shell
printenv --null {{HOME}}
```
{% endraw %}