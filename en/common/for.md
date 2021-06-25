---
layout: default
title: "for"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="for">
  <a href="/en/common/for.html">for</a> <a href="#for"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell loop over parameters.
> More information: <https://man.archlinux.org/man/for.n>.

#### Perform a command with different arguments:
```shell
for argument in 1 2 3; do {{command $argument}}; done
```
#### Perform a command in every directory:
```shell
for d in *; do (cd $d; {{command}}); done
```
{% endraw %}