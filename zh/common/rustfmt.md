---
layout: default
title: "rustfmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rustfmt">
  <a href="/zh/common/rustfmt.html">rustfmt</a> <a href="#rustfmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 格式化 Rust 源代码的工具.
> 更多信息: <https://github.com/rust-lang/rustfmt>.

#### 格式化文件，就地覆盖原始文件:
```shell
rustfmt {{source.rs}}
```
#### 检查文件的格式并在控制台上显示所有更改:
```shell
rustfmt --check {{source.rs}}
```
#### 格式化之前，备份所有修改过的文件(原始文件的扩展名为 `.bk`):
```shell
rustfmt --backup {{source.rs}}
```
{% endraw %}