---
layout: default
title: "gpg-zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg-zip">
  <a href="/zh/common/gpg-zip.html">gpg-zip</a> <a href="#gpg-zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用`GPG`加密存档中的文件和目录。
> 更多信息： <https://www.gnupg.org/documentation/manuals/gnupg/gpg_002dzip.html>.

#### 使用密码将一个目录加密为`archive.gpg`：
```shell
gpg-zip --symmetric --output {{archive.gpg}} {{path/to/directory}}
```
#### 将`archive.gpg`解密到同名目录中：
```shell
gpg-zip --decrypt {{path/to/archive.gpg}}
```
#### 列出加密的`archive.gpg`的内容：
```shell
gpg-zip --list-archive {{path/to/archive.gpg}}
```
{% endraw %}