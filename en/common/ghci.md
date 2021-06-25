---
layout: default
title: "ghci"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghci">
  <a href="/en/common/ghci.html">ghci</a> <a href="#ghci"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Glasgow Haskell Compiler's interactive environment.
> More information: <https://downloads.haskell.org/ghc/latest/docs/html/users_guide/ghci.html>.

#### Start a REPL (interactive shell):
```shell
ghci
```
#### Start a REPL and load the specified Haskell source file:
```shell
ghci {{source_file.hs}}
```
#### Start a REPL and enable a language option:
```shell
ghci -X{{language_option}}
```
#### Start a REPL and enable some level of compiler warnings (e.g. `all` or `compact`):
```shell
ghci -W{{warning_level}}
```
#### Start a REPL with a colon-separated list of directories for finding source files:
```shell
ghci -i{{path/to/directory1}}:{{path/to/directory2}}
```
{% endraw %}