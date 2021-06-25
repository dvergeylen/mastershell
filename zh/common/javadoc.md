---
layout: default
title: "javadoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="javadoc">
  <a href="/zh/common/javadoc.html">javadoc</a> <a href="#javadoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从源代码以 HTML 格式生成 Java API 文档。
> 更多信息见：https://docs.oracle.com/javase/9/javadoc/javadoc-command.htm>.

#### 生成 Java 源代码的文档并将结果保存在文件夹中：
```shell
javadoc -d {{path/to/directory/}} {{path/to/java_source_code}}
```
#### 生成指定编码的文档：
```shell
javadoc -docencoding {{UTF-8}} {{path/to/java_source_code}}
```
#### 生成文档时，排除掉某些软件包：
```shell
javadoc -exclude {{package_list}} {{path/to/java_source_code}}
```
{% endraw %}