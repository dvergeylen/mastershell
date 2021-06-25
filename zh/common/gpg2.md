---
layout: default
title: "gpg2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg2">
  <a href="/zh/common/gpg2.html">gpg2</a> <a href="#gpg2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard 2。
> GNU Privacy Guard 1 请参见`gpg`。
> 更多信息：<https://docs.releng.linuxfoundation.org/en/latest/gpg.html>。

#### 列出导入的密钥（公钥）：
```shell
gpg2 --list-keys
```
#### 为指定的接收者加密指定的文件，将输出结果写到一个新的文件中，并附加`.gpg`：
```shell
gpg2 --encrypt --recipient {{alice@example.com}} {{path/to/doc.txt}}
```
#### 只用密码（对称加密）对指定文件进行加密，将输出结果写入一个附加`.gpg`的新文件：
```shell
gpg2 --symmetric {{path/to/doc.txt}}
```
#### 解密指定的文件，并将结果写入标准输出：
```shell
gpg2 --decrypt {{path/to/doc.txt.gpg}}
```
#### 导入一个公钥：
```shell
gpg2 --import {{path/to/public_key.gpg}}
```
#### 将指定电子邮件地址的公钥导出到标准输出：
```shell
gpg2 --export --armor {{alice@example.com}}
```
#### 将指定电子邮件地址的私钥导出到标准输出：
```shell
gpg2 --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}