---
layout: default
title: "certbot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="certbot">
  <a href="/de/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Let's Encrypt Agent zum automatischen Erhalten und Erneuern von TLS-Zertifikaten.
> Nachfolger von `letsencrypt`.
> Weitere Informationen: <https://certbot.eff.org/docs/using.html>.

#### Beziehe ein neues Zertifikat über die webroot-Autorisierung, aber ohne dieses automatisch zu installieren:
```shell
sudo certbot certonly --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}}
```
#### Beziehe ein neues Zertifikat über die nginx-Autorisierung und automatische Installation des neuen Zertifikats:
```shell
sudo certbot --nginx --domain {{subdomain.beispiel.de}}
```
#### Beziehe ein neues Zertifikat über die apache-Autorisierung und automatische Installation des neuen Zertifikats:
```shell
sudo certbot --apache --domain {{subdomain.beispiel.de}}
```
#### Erneuere alle Let's Encrypt Zertifikate die in 30 Tagen oder weniger auslaufen (nicht vergessen alle Server, die diese nutzen, neu zu starten):
```shell
sudo certbot renew
```
#### Simuliere die Zertifikatserneuerung, ohne diese zu speichern:
```shell
sudo certbot --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}} --dry-run
```
#### Beziehe eine Test-Zertifikat:
```shell
sudo certbot --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}} --test-cert
```
{% endraw %}