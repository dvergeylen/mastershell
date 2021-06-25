---
layout: default
title: "now"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="now">
  <a href="/en/common/now.html">now</a> <a href="#now"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cloud platform for serverless deployment.
> This command is deprecated. See `vercel`, the updated version of this tool.
> More information: <https://zeit.co/now>.

#### Deploy the current directory:
```shell
now
```
#### Display a list of deployments:
```shell
now list
```
#### Display information related to a deployment:
```shell
now inspect {{deployment_url}}
```
#### Remove a deployment:
```shell
now remove {{deployment_id}}
```
#### Log in into an account or create a new one:
```shell
now login
```
#### Initialize an example project (a new directory will be created):
```shell
now init
```
{% endraw %}