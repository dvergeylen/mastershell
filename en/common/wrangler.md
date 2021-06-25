---
layout: default
title: "wrangler"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wrangler">
  <a href="/en/common/wrangler.html">wrangler</a> <a href="#wrangler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cloudflare Workers command-line tool.
> More information: <https://developers.cloudflare.com/workers/>.

#### Initialize a project with a skeleton configuration:
```shell
wrangler init {{project_name}}
```
#### Authenticate with Cloudflare:
```shell
wrangler login
```
#### Start a local development server:
```shell
wrangler dev --host {{hostname}}
```
#### Publish the worker script:
```shell
wrangler publish
```
#### Aggregate logs from the production worker:
```shell
wrangler tail
```
{% endraw %}