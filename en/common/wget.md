---
layout: default
title: "wget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wget">
  <a href="/en/common/wget.html">wget</a> <a href="#wget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download files from the Web.
> Supports HTTP, HTTPS, and FTP.
> More information: <https://www.gnu.org/software/wget>.

#### Download the contents of an URL to a file (named "foo" in this case):
```shell
wget {{https://example.com/foo}}
```
#### Download the contents of an URL to a file (named "bar" in this case):
```shell
wget --output-document {{bar}} {{https://example.com/foo}}
```
#### Download a single web page and all its resources with 3-second intervals between requests (scripts, stylesheets, images, etc.):
```shell
wget --page-requisites --convert-links --wait=3 {{https://example.com/somepage.html}}
```
#### Download all listed files within a directory and its sub-directories (does not download embedded page elements):
```shell
wget --mirror --no-parent {{https://example.com/somepath/}}
```
#### Limit the download speed and the number of connection retries:
```shell
wget --limit-rate={{300k}} --tries={{100}} {{https://example.com/somepath/}}
```
#### Download a file from an HTTP server using Basic Auth (also works for FTP):
```shell
wget --user={{username}} --password={{password}} {{https://example.com}}
```
#### Continue an incomplete download:
```shell
wget --continue {{https://example.com}}
```
#### Download all URLs stored in a text file to a specific directory:
```shell
wget --directory-prefix {{path/to/directory}} --input-file {{URLs.txt}}
```
{% endraw %}