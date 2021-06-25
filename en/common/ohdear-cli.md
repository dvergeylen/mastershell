---
layout: default
title: "ohdear-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ohdear-cli">
  <a href="/en/common/ohdear-cli.html">ohdear-cli</a> <a href="#ohdear-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An unofficial Oh Dear CLI written with Laravel Zero.
> More information: <https://github.com/nunomaduro/ohdear-cli>.

#### Display details about the currently authenticated user:
```shell
ohdear-cli me
```
#### Add a new site to Oh Dear:
```shell
ohdear-cli sites:add {{url}}
```
#### Display a list of sites and their current status:
```shell
ohdear-cli sites:list
```
#### Display details about a specific site:
```shell
ohdear-cli sites:show {{site_id}}
```
{% endraw %}