---
layout: default
title: "cargo build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo-build">
  <a href="/en/common/cargo-build.html">cargo build</a> <a href="#cargo-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a local package and all of its dependencies.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-build.html>.

#### Build the package or packages defined by the `Cargo.toml` manifest file in the local path:
```shell
cargo build
```
#### Build artifacts in release mode, with optimizations:
```shell
cargo build --release
```
#### Require that `Cargo.lock` is up to date:
```shell
cargo build --locked
```
#### Build all packages in the workspace:
```shell
cargo build --workspace
```
#### Build a specific package:
```shell
cargo build --package {{package}}
```
#### Build only the specified binary:
```shell
cargo build --bin {{name}}
```
#### Build only the specified test target:
```shell
cargo build --test {{testname}}
```
{% endraw %}