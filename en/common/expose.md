---
layout: default
title: "expose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expose">
  <a href="/en/common/expose.html">expose</a> <a href="#expose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An open source tunnel application for sharing websites.
> More information: <https://beyondco.de/docs/expose>.

#### Register your authentication token:
```shell
expose token {{token}}
```
#### Share the current working directory:
```shell
expose
```
#### Share the current working directory with a specific subdomain:
```shell
expose --subdomain={{subdomain}}
```
#### Share a local URL:
```shell
expose share {{url}}
```
#### Run the Expose server:
```shell
expose serve
```
#### Run the Expose server with a specific hostname:
```shell
expose serve {{hostname}}
```
{% endraw %}