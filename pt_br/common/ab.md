---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/pt_br/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta da Apache para realizar benchmarking e testes de carga em servidores web.
> Mais informações: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Executar 100 requisições HTTP do tipo GET para uma determinada URL:
```shell
ab -n {{100}} {{url}}
```
#### Executar 100 requisições HTTP do tipo GET para uma determinada URL, executando 10 requisições simultâneas de cada vez:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Utilizar a funcionalidade HTTP Keep Alive, permitindo que várias requisições sejam feitas em uma sessão HTTP:
```shell
ab -k {{url}}
```
#### Definir o tempo total do benchmarking, em segundos:
```shell
ab -t {{60}} {{url}}
```
{% endraw %}