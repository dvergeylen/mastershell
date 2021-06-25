---
layout: default
title: "cargo doc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo-doc">
  <a href="/en/common/cargo-doc.html">cargo doc</a> <a href="#cargo-doc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build and view Rust package documentation offline.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-doc.html>.

#### Build and view the default package documentation in the browser:
```shell
cargo doc --open
```
#### Build documentation without accessing the network:
```shell
cargo doc --offline
```
#### View a particular package's documentation:
```shell
cargo doc --open --package {{package}}
```
#### View a particular package's documentation offline:
```shell
cargo doc --open --offline --package {{package}}
```
{% endraw %}