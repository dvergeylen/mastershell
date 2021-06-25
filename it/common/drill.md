---
layout: default
title: "drill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drill">
  <a href="/it/common/drill.html">drill</a> <a href="#drill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui varie query DNS.
> Maggiori informazioni: <https://manned.org/drill>.

#### Mostra gli IP associati ad un hostname (record A):
```shell
drill {{esempio.com}}
```
#### Lookup the mail server(s) associated with a given domain name (MX record):
```shell
drill mx {{esempio.com}}
```
#### Recupera tutti i tipi di record per un dato dominio:
```shell
drill any {{esempio.com}}
```
#### Specifica un server DNS alternativo da interrogare:
```shell
drill {{esempio.com}} @{{8.8.8.8}}
```
#### Esegui un lookup DNS inverso su di un indirizzo IP (record PTR):
```shell
drill -x {{8.8.8.8}}
```
#### Esegui un tracciamento DNSSEC dai root server fino al dominio:
```shell
drill -TD {{esempio.com}}
```
#### Mostra record DNSKEY per un dominio:
```shell
drill -s dnskey {{esempio.com}}
```
{% endraw %}