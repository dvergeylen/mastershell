---
layout: default
title: "cradle deploy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-deploy">
  <a href="/en/common/cradle-deploy.html">cradle deploy</a> <a href="#cradle-deploy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Cradle deployments.
> More information: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#deploy>.

#### Deploy Cradle to a server:
```shell
cradle deploy production
```
#### Deploy static assets to Amazon S3:
```shell
cradle deploy s3
```
#### Deploy static assets including the Yarn "components" directory:
```shell
cradle deploy s3 --include-yarn
```
#### Deploy static assets including the "upload" directory:
```shell
cradle deploy s3 --include-upload
```
{% endraw %}