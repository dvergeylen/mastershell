---
layout: default
title: "nativefier"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nativefier">
  <a href="/pt_br/common/nativefier.html">nativefier</a> <a href="#nativefier"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para criação de aplicativos para desktop à partir de web sites.
> Mais informações: <https://github.com/jiahaog/nativefier>.

#### Gerar aplicativo desktop para site:
```shell
nativefier {{url}}
```
#### Gerar aplicativo desktop com nome customizado:
```shell
nativefier --name {{nome}} {{url}}
```
#### Gerar aplicativo desktop usando um ícone PNG customizado:
```shell
nativefier --icon {{caminho/para/icone.png}} {{url}}
```
{% endraw %}