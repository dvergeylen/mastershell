---
layout: default
title: "cradle deploy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-deploy">
  <a href="/de/common/cradle-deploy.html">cradle deploy</a> <a href="#cradle-deploy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Cradle Implementierungen.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#deploy>.

#### Implementiere Cradle auf einem Server:
```shell
cradle deploy production
```
#### Implementiere statische Anlagen zu Amazon S3:
```shell
cradle deploy s3
```
#### Implementiere statische Anlagen inklusive den Yarn Komponenten:
```shell
cradle deploy s3 --include-yarn
```
#### Implementiere statische Anlagen inklusive dem "upload" Verzeichnis:
```shell
cradle deploy s3 --include-upload
```
{% endraw %}