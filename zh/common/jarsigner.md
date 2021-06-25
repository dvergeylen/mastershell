---
layout: default
title: "jarsigner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jarsigner">
  <a href="/zh/common/jarsigner.html">jarsigner</a> <a href="#jarsigner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 签名并验证 Java 存档（JAR）文件。
> 更多信息见：<https://docs.oracle.com/javase/9/tools/jarsigner.htm>.

#### 签名一个 `JAR` 文件：
```shell
jarsigner {{path/to/file.jar}} {{keystore_alias}}
```
#### 使用特定算法对 `JAR` 文件进行签名：
```shell
jarsigner -sigalg {{algorithm}} {{path/to/file.jar}} {{keystore_alias}}
```
#### 验证 `JAR` 文件的签名：
```shell
jarsigner -verify {{path/to/file.jar}}
```
{% endraw %}