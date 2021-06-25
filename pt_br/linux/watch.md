---
layout: default
title: "watch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="watch">
  <a href="/pt_br/linux/watch.html">watch</a> <a href="#watch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa um comando repetidas vezes, e monitora a saída em tela cheia.

#### Monitora arquivos no diretório atual:
```shell
watch {{ls}}
```
#### Monitora espaço em disco e destaca as alterações:
```shell
watch -d {{df}}
```
#### Monitora processos "node", atualizando a cada 3 segundos:
```shell
watch -n {{3}} "{{ps aux | grep node}}"
```
{% endraw %}