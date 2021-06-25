---
layout: default
title: "jar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jar">
  <a href="/zh/common/jar.html">jar</a> <a href="#jar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 应用程序 / 类库打包程序。
> 更多信息见：<https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

#### 将当前目录中的所有文件递归归档到 `.jar` 文件中：
```shell
jar cf {{file.jar}} *
```
#### 将 `.jar` / `.war` 文件解压缩到当前目录：
```shell
jar -xvf {{file.jar}}
```
#### 列出 `.jar` / `.war` 文件内容：
```shell
jar tf {{path/to/file.jar}}
```
#### 列出带有详细输出的 `.jar` / `.war` 文件内容：
```shell
jar tvf {{path/to/file.jar}}
```
{% endraw %}