---
layout: default
title: "gpgv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpgv">
  <a href="/zh/common/gpgv.html">gpgv</a> <a href="#gpgv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 验证 OpenPGP 签名。
> 更多信息：<https://www.gnupg.org/documentation/manuals/gnupg/gpgv.html>。

#### 验证签名文件：
```shell
gpgv {{path/to/file}}
```
#### 使用分离式签名验证已签名的文件：
```shell
gpgv {{path/to/signature}} {{path/to/file}}
```
#### 在 keyrings 列表中添加一个文件（一个导出的钥匙也算作一个 keyring）：
```shell
gpgv --keyring {{path/to/keyring_file}} {{path/to/signature}} {{path/to/file}}
```
{% endraw %}