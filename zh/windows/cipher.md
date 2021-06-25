---
layout: default
title: "cipher"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cipher">
  <a href="/zh/windows/cipher.html">cipher</a> <a href="#cipher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 加密或解密 NTFS 驱动器上的文件.

#### 加密文件或目录:
```shell
cipher /e:{{路径/文件或目录}}
```
#### 解密文件或目录:
```shell
cipher /d:{{路径/文件或目录}}
```
#### 安全地删除文件或目录:
```shell
cipher /w:{{路径/文件或目录}}
```
{% endraw %}