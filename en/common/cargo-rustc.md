---
layout: default
title: "cargo rustc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo-rustc">
  <a href="/en/common/cargo-rustc.html">cargo rustc</a> <a href="#cargo-rustc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a Rust package, and pass extra options to the compiler.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-rustc.html>.

#### Build the package or packages defined by the `Cargo.toml` manifest file in the current working directory:
```shell
cargo rustc
```
#### Build artifacts in release mode, with optimizations:
```shell
cargo rustc --release
```
#### Compile with architecture-specific optimizations for the current CPU:
```shell
cargo rustc --release -- -C target-cpu=native
```
#### Compile with speed optimization:
```shell
cargo rustc -- -C opt-level {{1|2|3}}
```
#### Compile with [s]ize optimization (`z` also turns off loop vectorization):
```shell
cargo rustc -- -C opt-level {{s|z}}
```
#### Check if your package uses unsafe code:
```shell
cargo rustc --lib -- -D unsafe-code
```
#### Build a specific package:
```shell
cargo rustc --package {{package}}
```
#### Build only the specified binary:
```shell
cargo --bin {{name}}
```
{% endraw %}