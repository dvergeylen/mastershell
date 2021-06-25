---
layout: default
title: "md5sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="md5sum">
  <a href="/zh/common/md5sum.html">md5sum</a> <a href="#md5sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算 MD5 加密校验和.
> 更多信息： <https://www.gnu.org/software/coreutils/md5sum>.

#### 计算文件的 MD5 校验和:
```shell
md5sum {{filename1}}
```
#### 计算多个文件的 MD5 校验和:
```shell
md5sum {{filename1}} {{filename2}}
```
#### 读取 MD5SUM 的文件并验证所有文件是否具有匹配的校验和:
```shell
md5sum -c {{filename.md5}}
```
{% endraw %}