---
layout: default
title: "airpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airpaste">
  <a href="/pt_br/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compartilhar mensagens e arquivos na mesma rede.
> Mais informações: <https://github.com/mafintosh/airpaste>.

#### Esperar por mensagens e mostrá-las quando recebidas:
```shell
airpaste
```
#### Enviar texto:
```shell
echo {{texto}} | airpaste
```
#### Enviar arquivo:
```shell
airpaste < {{caminho/para/arquivo}}
```
#### Receber arquivo:
```shell
airpaste > {{caminho/para/arquivo}}
```
#### Criar/Entrar em canal:
```shell
airpaste {{nome_do_canal}}
```
{% endraw %}