---
layout: default
title: "airpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airpaste">
  <a href="/it/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Condividi messaggi e file nella stessa rete.
> Maggiori informazioni: <https://github.com/mafintosh/airpaste>.

#### Aspetta un messaggo e mostralo una volta ricevuto:
```shell
airpaste
```
#### Invia un messaggio di testo:
```shell
echo {{messaggio}} | airpaste
```
#### Invia un file:
```shell
airpaste < {{percorso/al/file}}
```
#### Ricevi un file:
```shell
airpaste > {{percorso/al/file}}
```
#### Crea o entra in un canale:
```shell
airpaste {{nome_canale}}
```
{% endraw %}