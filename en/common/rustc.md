---
layout: default
title: "rustc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rustc">
  <a href="/en/common/rustc.html">rustc</a> <a href="#rustc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Rust compiler.
> Processes, compiles and links Rust language source files.
> More information: <https://doc.rust-lang.org/rustc>.

#### Compile a single file:
```shell
rustc {{file.rs}}
```
#### Compile with high optimization:
```shell
rustc -O {{file.rs}}
```
#### Compile with debugging information:
```shell
rustc -g {{file.rs}}
```
#### Compile with architecture-specific optimizations for the current CPU:
```shell
rustc -C target-cpu=native {{path/to/file.rs}}
```
#### Display architecture-specific optimizations for the current CPU:
```shell
rustc -C target-cpu=native --print cfg
```
#### Display target list:
```shell
rustc --print target-list
```
#### Compile for a specific target:
```shell
rustc --target {{target_triple}} {{path/to/file.rs}}
```
{% endraw %}