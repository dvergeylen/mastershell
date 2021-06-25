---
layout: default
title: "certbot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="certbot">
  <a href="/en/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Let's Encrypt Agent for automatically obtaining and renewing TLS certificates.
> Successor to `letsencrypt`.
> More information: <https://certbot.eff.org/docs/using.html>.

#### Obtain a new certificate via webroot authorization, but do not install it automatically:
```shell
sudo certbot certonly --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}}
```
#### Obtain a new certificate via nginx authorization, installing the new certificate automatically:
```shell
sudo certbot --nginx --domain {{subdomain.example.com}}
```
#### Obtain a new certificate via apache authorization, installing the new certificate automatically:
```shell
sudo certbot --apache --domain {{subdomain.example.com}}
```
#### Renew all Let's Encrypt certificates that expire in 30 days or less (don't forget to restart any servers that use them afterwards):
```shell
sudo certbot renew
```
#### Simulate the obtaining of a new certificate, but don't actually save any new certificates to disk:
```shell
sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --dry-run
```
#### Obtain an untrusted test certificate instead:
```shell
sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --test-cert
```
{% endraw %}