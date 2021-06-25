---
layout: default
title: "cargo test"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo-test">
  <a href="/en/common/cargo-test.html">cargo test</a> <a href="#cargo-test"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute the unit and integration tests of a Rust package.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-test.html>.

#### Only run tests containing a specific string in their names:
```shell
cargo test {{testname}}
```
#### Set the number of simultaneous running test cases:
```shell
cargo test -- --test-threads={{count}}
```
#### Require that `Cargo.lock` is up to date:
```shell
cargo test --locked
```
#### Test artifacts in release mode, with optimizations:
```shell
cargo test --release
```
#### Test all packages in the workspace:
```shell
cargo test --workspace
```
#### Run tests for a package:
```shell
cargo test --package {{package}}
```
{% endraw %}