---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/pt_br/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de conversão de imagens da ImageMagick.
> Mais informações: <https://imagemagick.org/script/convert.php>.

#### Converter uma imagem do formato JPG para o formato PNG:
```shell
convert {{imagem.jpg}} {{imagem.png}}
```
#### Escalar uma imagem para 50% do seu tamanho original:
```shell
convert {{imagem.png}} -resize 50% {{nova_imagem.png}}
```
#### Escalar uma imagem, mantendo as suas proporções originais, para uma dimensão máxima de 640x480:
```shell
convert {{imagem.png}} -resize 640x480 {{nova_imagem.png}}
```
#### Juntar várias imagens horizontalmente:
```shell
convert {{imagem1.png}} {{imagem2.png}} {{imagem3.png}} +append {{nova_imagem.png}}
```
#### Criar um GIF a partir de uma série de imagens, com um intervalo de 100ms entre elas:
```shell
convert {{imagem1.png}} {{imagem2.png}} {{imagem3.png}} -delay {{100}} {{nova_imagem.gif}}
```
#### Criar uma nova imagem de tamanho 800x600 com apenas um fundo sólido vermelho:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{imagem.png}}
```
{% endraw %}