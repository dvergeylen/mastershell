---
layout: default
title: "xcv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcv">
  <a href="/pt_br/common/xcv.html">xcv</a> <a href="#xcv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Corta, copia e cola na linha de comando.
> Mais informações: <https://github.com/busterc/xcv>.

#### Cortar um arquivo:
```shell
xcv x {{arquivo_a_ser_cortado}}
```
#### Copiar um arquivo:
```shell
xcv c {{arquivo_a_ser_copiado}}
```
#### Colar um arquivo:
```shell
xcv v {{arquivo_a_ser_colado}}
```
#### Listar todos os arquivos disponíveis para serem colados:
```shell
xcv l
```
{% endraw %}