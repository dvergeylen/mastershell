---
layout: default
title: "valgrind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="valgrind">
  <a href="/en/common/valgrind.html">valgrind</a> <a href="#valgrind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wrapper for a set of expert tools for profiling, optimizing and debugging programs.
> Commonly used tools include `memcheck`, `cachegrind`, `callgrind`, `massif`, `helgrind`, and `drd`.
> More information: <http://www.valgrind.org>.

#### Use the (default) Memcheck tool to show a diagnostic of memory usage by `program`:
```shell
valgrind {{program}}
```
#### Use Memcheck to report all possible memory leaks of `program` in full detail:
```shell
valgrind --leak-check=full --show-leak-kinds=all {{program}}
```
#### Use the Cachegrind tool to profile and log CPU cache operations of `program`:
```shell
valgrind --tool=cachegrind {{program}}
```
#### Use the Massif tool to profile and log heap memory and stack usage of `program`:
```shell
valgrind --tool=massif --stacks=yes {{program}}
```
{% endraw %}