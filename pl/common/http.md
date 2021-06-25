---
layout: default
title: "http"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="http">
  <a href="/pl/common/http.html">http</a> <a href="#http"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTTPie: HTTP client, ma być łatwiejszy w użyciu niż cURL.
> Więcej informacji: <https://httpie.org>.

#### Pobierz adres URL do pliku:
```shell
http --download {{przyklad.org}}
```
#### Wyślij dane zakodowane w formularzu:
```shell
http --form {{przyklad.org}} {{nazwa='bob'}} {{zdjecie_profilowe@'bob.png'}}
```
#### Wyślij obiekt JSON:
```shell
http {{przyklad.org}} {{name='bob'}}
```
#### Określ metodę HTTP:
```shell
http {{HEAD}} {{przyklad.org}}
```
#### Dołącz dodatkowy nagłówek:
```shell
http {{przyklad.org}} {{X-MyHeader:123}}
```
#### Podaj nazwę użytkownika i hasło do uwierzytelnienia serwera:
```shell
http --auth {{nazwauzytkownika:haslo}} {{przyklad.org}}
```
#### Określ surowe ciało żądania za pośrednictwem stdin:
```shell
cat {{dane.txt}} | http PUT {{przyklad.org}}
```
{% endraw %}