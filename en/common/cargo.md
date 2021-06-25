---
layout: default
title: "cargo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo">
  <a href="/en/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust package manager.
> Manage Rust projects and their module dependencies (crates).
> More information: <https://crates.io/>.

#### Search for crates:
```shell
cargo search {{search_string}}
```
#### Install a crate:
```shell
cargo install {{crate_name}}
```
#### List installed crates:
```shell
cargo install --list
```
#### Create a new binary or library Rust project in the current directory:
```shell
cargo init --{{bin|lib}}
```
#### Create a new binary or library Rust project in the specified directory:
```shell
cargo new {{path/to/directory}} --{{bin|lib}}
```
#### Build the Rust project in the current directory:
```shell
cargo build
```
#### Build using a specific number of threads (default is the number of CPU cores):
```shell
cargo build -j {{jobs}}
```
{% endraw %}