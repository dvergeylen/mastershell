---
layout: default
title: "rustfmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rustfmt">
  <a href="/en/common/rustfmt.html">rustfmt</a> <a href="#rustfmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for formatting Rust source code.
> More information: <https://github.com/rust-lang/rustfmt>.

#### Format a file, overwriting the original file in-place:
```shell
rustfmt {{source.rs}}
```
#### Check a file for formatting and display any changes on the console:
```shell
rustfmt --check {{source.rs}}
```
#### Backup any modified files before formatting (the original file is renamed with a `.bk` extension):
```shell
rustfmt --backup {{source.rs}}
```
{% endraw %}