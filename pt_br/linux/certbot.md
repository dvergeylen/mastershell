---
layout: default
title: "certbot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="certbot">
  <a href="/pt_br/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> O agente da Let's Encrypt para obtenção e renovação de certificados TLS automaticamente.
> Sucessor do `letsencrypt`.

#### Obter um novo certificado via autorização webroot, porém sem instalá-lo automaticamente:
```shell
sudo certbot certonly --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}}
```
#### Obter um novo certificado via autorização nginx e instalá-lo automaticamente:
```shell
sudo certbot --nginx --domain {{subdominio.dominio.com}}
```
#### Obter um novo certificado via autorização apache e instalá-lo automaticamente:
```shell
sudo certbot --apache --domain {{subdominio.dominio.com}}
```
#### Renovar todos os certificados que expirarão em 30 dias ou menos (não esqueça de reiniciar todos os servidores que usam os certificados):
```shell
sudo certbot renew
```
#### Simular a obtenção de um novo certificado, porém sem salvá-lo no disco rígido:
```shell
sudo certbot --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}} --dry-run
```
#### Obter um certificado não confiável para testes:
```shell
sudo certbot --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}} --test-cert
```
{% endraw %}