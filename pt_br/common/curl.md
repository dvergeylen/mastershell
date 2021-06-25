---
layout: default
title: "curl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="curl">
  <a href="/pt_br/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transfere dados entre o computador local e um servidor remoto.
> Suporta a maioria dos protocolos de comunicação, incluindo HTTP, FTP e POP3.
> Mais informações: <https://curl.se>.

#### Descarregar os conteúdos de um URL para um arquivo:
```shell
curl {{http://example.com}} --output {{arquivo}}
```
#### Descarregar um arquivo, gravando o resultado sob o nome do arquivo indicado pelo URL:
```shell
curl --remote-name {{http://example.com/arquivo}}
```
#### Descarregar um arquivo, seguindo redirecionamentos e automaticamente continuando transferências idênticas que tenham sido interrompidas:
```shell
curl --remote-name --location --continue-at - {{http://example.com/arquivo}}
```
#### Enviar dados codificados por formulário (pedido POST do tipo `application/x-www-form-urlencoded`):
```shell
curl --data {{'nome=maria'}} {{http://example.com/formulario}}
```
#### Enviar um pedido com um cabeçalho adicional, usando um método HTTP personalizado:
```shell
curl --header {{'X-Meu-Cabecalho: 123'}} --request {{PUT}} {{http://example.com}}
```
#### Enviar dados no formato JSON, especificando o cabeçalho de tipo de conteúdo (content-type) apropriado:
```shell
curl --data {{'{"nome":"maria"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/usuarios/123}}
```
#### Passar ao pedido o nome de usuário e senha para autenticação no servidor:
```shell
curl -u usuario:senha {{http://example.com}}
```
#### Passar ao pedido o certificado do cliente e a chave para um recurso, omitindo a validação do certificado:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}
```
{% endraw %}