---
layout: default
title: "acme.sh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="acme.sh">
  <a href="/en/common/acme.sh.html">acme.sh</a> <a href="#acme.sh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell script implementing ACME client protocol, an alternative to certbot.
> See also `acme.sh dns`.
> More information: <https://github.com/acmesh-official/acme.sh>.

#### Issue a certificate using webroot mode:
```shell
acme.sh --issue --domain {{example.com}} --webroot {{/path/to/webroot}}
```
#### Issue a certificate for multiple domains using standalone mode using port 80:
```shell
acme.sh --issue --standalone --domain {{example.com}} --domain {{www.example.com}}
```
#### Issue a certificate using standalone TLS mode using port 443:
```shell
acme.sh --issue --alpn --domain {{example.com}}
```
#### Issue a certificate using a working Nginx configuration:
```shell
acme.sh --issue --nginx --domain {{example.com}}
```
#### Issue a certificate using a working Apache configuration:
```shell
acme.sh --issue --apache --domain {{example.com}}
```
#### Issue a wildcard (\*) certificate using an automatic DNS API mode:
```shell
acme.sh --issue --dns {{dns_cf}} --domain {{*.example.com}}
```
#### Install certificate files into the specified locations (useful for automatic certificate renewal):
```shell
acme.sh --install-cert -d {{example.com}} --key-file {{/path/to/example.com.key}} --fullchain-file {{/path/to/example.com.cer}} --reloadcmd {{"systemctl force-reload nginx"}}
```
{% endraw %}