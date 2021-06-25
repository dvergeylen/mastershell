---
layout: default
title: "vercel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vercel">
  <a href="/en/common/vercel.html">vercel</a> <a href="#vercel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deploy and manage your Vercel deployments.
> More information: <https://vercel.com/docs/cli>.

#### Deploy the current directory:
```shell
vercel
```
#### Deploy the current directory to production:
```shell
vercel --prod
```
#### Deploy a directory:
```shell
vercel {{path/to/project}}
```
#### Initialize an example project:
```shell
vercel init
```
#### Deploy with Environment Variables:
```shell
vercel --env {{ENV}}={{var}}
```
#### Build with Environment Variables:
```shell
vercel --build-env {{ENV}}={{var}}
```
#### Set default regions to enable the deployment on:
```shell
vercel --regions {{region_id}}
```
#### Remove a deployment:
```shell
vercel remove {{project_name}}
```
{% endraw %}