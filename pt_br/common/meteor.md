---
layout: default
title: "meteor"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="meteor">
  <a href="/pt_br/common/meteor.html">meteor</a> <a href="#meteor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plataforma Full-Stack de JavaScript para desenvolver aplicações web.
> Mais informações: <https://meteor.com>.

#### Executar um projeto meteor a partir do seu diretório base em modo de desenvolvimento:
```shell
meteor
```
#### Criar um novo projeto em um diretório específico:
```shell
meteor create {{caminho/para/diretório}}
```
#### Listar todos os pacotes usados pelo projeto:
```shell
meteor list
```
#### Adicionar um pacote ao projeto:
```shell
meteor add {{nome_pacote}}
```
#### Remover um pacote do projeto:
```shell
meteor remove {{nome_pacote}}
```
#### Criar uma build de produção do projeto, no formato tarball, em um diretório específico:
```shell
meteor build {{caminho/para/diretório}}
```
{% endraw %}