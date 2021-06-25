---
layout: default
title: "ghc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghc">
  <a href="/en/common/ghc.html">ghc</a> <a href="#ghc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Glasgow Haskell Compiler.
> Compiles and links Haskell source files.
> More information: <https://www.haskell.org/ghc>.

#### Find and compile all modules in the current directory:
```shell
ghc Main
```
#### Compile a single file:
```shell
ghc {{file.hs}}
```
#### Compile using extra optimization:
```shell
ghc -O {{file.hs}}
```
#### Stop compilation after generating object files (.o):
```shell
ghc -c {{file.hs}}
```
#### Run Haskell interactive interpreter (REPL):
```shell
ghci
```
#### Evaluate a single expression:
```shell
ghc -e {{expression}}
```
{% endraw %}