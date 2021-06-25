---
layout: default
title: "duti"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="duti">
  <a href="/en/osx/duti.html">duti</a> <a href="#duti"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set default applications for document types and URL schemes on macOS.

#### Set Safari as the default handler for HTML documents:
```shell
duti -s {{com.apple.Safari}} {{public.html}} all
```
#### Set VLC as the default viewer for files with `.m4v` extensions:
```shell
duti -s {{org.videolan.vlc}} {{m4v}} viewer
```
#### Set Finder as the default handler for the ftp:// URL scheme:
```shell
duti -s {{com.apple.Finder}} {{ftp}}
```
#### Display information about the default application for a given extension:
```shell
duti -x {{ext}}
```
#### Display the default handler for a given UTI:
```shell
duti -d {{uti}}
```
#### Display all handlers of a given UTI:
```shell
duti -l {{uti}}
```
{% endraw %}