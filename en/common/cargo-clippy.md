---
layout: default
title: "cargo clippy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo-clippy">
  <a href="/en/common/cargo-clippy.html">cargo clippy</a> <a href="#cargo-clippy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A collection of lints to catch common mistakes and improve your Rust code.
> More information: <https://github.com/rust-lang/rust-clippy>.

#### Run checks over the code in the current directory:
```shell
cargo clippy
```
#### Require that `Cargo.lock` is up to date:
```shell
cargo clippy --locked
```
#### Run checks on all packages in the workspace:
```shell
cargo clippy --workspace
```
#### Run checks for a package:
```shell
cargo clippy --package {{package}}
```
#### Treat warnings as errors:
```shell
RUSTFLAGS="-Dwarnings" cargo clippy -- -D warnings
```
#### Run checks and ignore warnings:
```shell
cargo clippy -- -A warnings
```
#### Apply Clippy suggestion automatically (experimental and only supported on the nightly channel):
```shell
cargo clippy --fix -Z unstable-options
```
{% endraw %}