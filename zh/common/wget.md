---
layout: default
title: "wget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wget">
  <a href="/zh/common/wget.html">wget</a> <a href="#wget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从网络上下载文件.
> 支持 HTTP, HTTPS, 和 FTP.
> 更多信息：<https://www.gnu.org/software/wget>.

#### 将该 URL 的内容下载到文件中 （在这个例子中文件名为 "foo"）:
```shell
wget {{https://example.com/foo}}
```
#### 将该 URL 的内容下载到文件中 （在这个例子中文件名为 "bar"）:
```shell
wget --output-document {{bar}} {{https://example.com/foo}}
```
#### 以每三秒一个请求的速度下载一个网页和其所有资源 （脚本，样式表，图片等等）:
```shell
wget --page-requisites --convert-links --wait=3 {{https://example.com/somepage.html}}
```
#### 从一个目录中下载所有列出的文件和其所有子文件夹 （不下载内嵌网页）:
```shell
wget --mirror --no-parent {{https://example.com/somepath/}}
```
#### 限制下载速度和重试次数:
```shell
wget --limit-rate={{300k}} --tries={{100}} {{https://example.com/somepath/}}
```
#### 使用基本授权来从 HTTP/FTP 服务器中下载文件:
```shell
wget --user={{username}} --password={{password}} {{https://example.com}}
```
#### 继续一个未完成的下载任务:
```shell
wget --continue {{https://example.com}}
```
#### 将指定文件中所有列出的 URL 下载到一个目录中:
```shell
wget --directory-prefix {{path/to/directory}} --input-file {{URLs.txt}}
```
{% endraw %}