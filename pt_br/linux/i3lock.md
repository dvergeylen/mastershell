---
layout: default
title: "i3lock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="i3lock">
  <a href="/pt_br/linux/i3lock.html">i3lock</a> <a href="#i3lock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bloqueador de tela simples para o i3wm.
> Mais informações: <https://i3wm.org/i3lock>.

#### Bloqueia a tela com uma cor de fundo (formato rrggbb):
```shell
i3lock -c {{0000ff}}
```
#### Bloqueia a tela com uma imagem PNG:
```shell
i3lock -i {{local/da/imagem.png}}
```
#### Desabilita o indicador de desbloqueio (remove a resposta ao apertar teclas):
```shell
i3lock -u
```
#### Exibe o ponteiro do mouse ao invés de ocultá-lo ('default' para o ponteiro padrão, 'win' para um ponteiro MS Windows):
```shell
i3lock -p {{default|win}}
```
#### Bloqueia a tela com uma imagem PNG exibida em múltiplos monitores, com o ponteiro do mouse habilitado:
```shell
i3lock -i {{local/da/imagem.png}} -p {{default|win}} -t
```
{% endraw %}