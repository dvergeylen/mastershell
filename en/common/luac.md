---
layout: default
title: "luac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="luac">
  <a href="/en/common/luac.html">luac</a> <a href="#luac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lua bytecode compiler.
> More information: <https://www.lua.org>.

#### Compile a Lua source file to Lua bytecode:
```shell
luac -o {{byte_code.luac}} {{source.lua}}
```
#### Do not include debug symbols in the output:
```shell
luac -s -o {{byte_code.luac}} {{source.lua}}
```
{% endraw %}