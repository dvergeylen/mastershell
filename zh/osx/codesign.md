---
layout: default
title: "codesign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="codesign">
  <a href="/zh/osx/codesign.html">codesign</a> <a href="#codesign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 为 macOS 的应用程序签名.

#### 用证书签名:
```shell
codesign -s "{{公司名称}}" {{路径 / 应用名.app}}
```
#### 验证应用程序的签名:
```shell
codesign -v {{路径 / 应用名.app}}
```
{% endraw %}