---
layout: default
title: "mkcert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkcert">
  <a href="/en/common/mkcert.html">mkcert</a> <a href="#mkcert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for making locally-trusted development certificates.
> More information: <https://github.com/FiloSottile/mkcert>.

#### Install the local CA in the system trust store:
```shell
mkcert -install
```
#### Generate certificate and private key for a given domain:
```shell
mkcert {{example.org}}
```
#### Generate certificate and private key for multiple domains:
```shell
mkcert {{example.org}} {{myapp.dev}} {{127.0.0.1}}
```
#### Generate wildcard certificate and private key for a given domain and its subdomains:
```shell
mkcert "{{*.example.it}}"
```
#### Uninstall the local CA:
```shell
mkcert -uninstall
```
{% endraw %}