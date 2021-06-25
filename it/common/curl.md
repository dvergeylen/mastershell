---
layout: default
title: "curl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="curl">
  <a href="/it/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trasferisci dati da o ad un server.
> Supporta molti protocollo, tra cui HTTP, FTP e POP3.
> Maggiori informazioni: <https://curl.se>.

#### Scarica il contenuto di un URL in un file:
```shell
curl {{http://example.com}} --output {{nome_file}}
```
#### Scarica un file, salvando l'output con lo stesso nome indicato nell'URL:
```shell
curl --remote-name {{http://example.com/nome_file}}
```
#### Scarica un file, seguendo reindirizzamenti, e continuando automaticamente (riprendendo) un trasferimento precedente:
```shell
curl --remote-name --location --continue-at - {{http://example.com/nome_file}}
```
#### Invia dati form-encoded (richiesta POST di tipo `application/x-www-form-urlencoded`):
```shell
curl --data {{'nome=mario'}} {{http://example.com/form}}
```
#### Invia una richiesta con un header aggiuntivo, utilizzando un metodo HTTP personalizzato:
```shell
curl --header {{'X-Mio-Header: 123'}} --request {{PUT}} {{http://example.com}}
```
#### Invia dati in formato JSON, specificando l'header content-type appropriato:
```shell
curl --data {{'{"nome":"mario"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/utenti/1234}}
```
#### Utilizza un nome utente ed una password per l'autenticazione con il server:
```shell
curl --user utente:password {{http://example.com}}
```
#### Utilizza un certificato ed una chiave per una risorsa, ignorando la validazione dei certificati:
```shell
curl --cert {{client.pem}} --key {{chiave.pem}} --insecure {{https://example.com}}
```
{% endraw %}