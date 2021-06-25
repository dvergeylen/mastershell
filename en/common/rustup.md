---
layout: default
title: "rustup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rustup">
  <a href="/en/common/rustup.html">rustup</a> <a href="#rustup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust toolchain installer.
> Install, manage, and update Rust toolchains.
> More information: <https://github.com/rust-lang/rustup.rs>.

#### Install the nightly toolchain for your system:
```shell
rustup install nightly
```
#### Switch the default toolchain to nightly so that the `cargo` and `rustc` commands will use it:
```shell
rustup default nightly
```
#### Use the nightly toolchain when inside the current project, but leave global settings unchanged:
```shell
rustup override set nightly
```
#### Update all toolchains:
```shell
rustup update
```
#### List installed toolchains:
```shell
rustup show
```
#### Run cargo build with a certain toolchain:
```shell
rustup run {{toolchain_name}} cargo build
```
{% endraw %}