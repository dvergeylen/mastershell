---
layout: default
title: "cradle deploy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-deploy">
  <a href="/it/common/cradle-deploy.html">cradle deploy</a> <a href="#cradle-deploy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci distribuzioni Cradle.
> Maggiori informazioni: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#deploy>.

#### Distribuisci Cradle su un server:
```shell
cradle deploy production
```
#### Distribuisci assets statici ad Amazon S3:
```shell
cradle deploy s3
```
#### Distribuisci assets statici, inclusa la directory "components" di Yarn:
```shell
cradle deploy s3 --include-yarn
```
#### Distribuisci assets statici, includendo la directory "upload":
```shell
cradle deploy s3 --include-upload
```
{% endraw %}