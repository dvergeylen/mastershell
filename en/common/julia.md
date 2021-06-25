---
layout: default
title: "julia"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="julia">
  <a href="/en/common/julia.html">julia</a> <a href="#julia"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A high-level, high-performance dynamic programming language for technical computing.
> More information: <https://docs.julialang.org/en/v1/manual/getting-started/>.

#### Start a Julia REPL session:
```shell
julia
```
#### Execute a Julia program and exit:
```shell
julia {{program.jl}}
```
#### Execute a Julia program that takes arguments:
```shell
julia {{program.jl}} {{arguments}}
```
#### Evaluate a string containing Julia code:
```shell
julia -e '{{julia_code}}'
```
#### Evaluate a string of Julia code, passing arguments to it:
```shell
julia -e '{{for x in ARGS; println(x); end}}' {{arguments}}
```
#### Evaluate an expression and print the result:
```shell
julia -E '{{(1 - cos(pi/4))/2}}'
```
#### Start Julia in parallel mode, using N worker processes:
```shell
julia -p {{N}}
```
{% endraw %}