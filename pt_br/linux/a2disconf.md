---
layout: default
title: "a2disconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2disconf">
  <a href="/pt_br/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desativar um arquivo de configuração em sistemas operacionais baseados no Debian.
> Mais informações: <https://manpages.debian.org/buster/apache2/a2disconf.8.en.html>.

#### Desativar um arquivo de configuração:
```shell
sudo a2disconf {{arquivo_de_configuracao}}
```
#### Não mostrar mensagens informativas:
```shell
sudo a2disconf --quiet {{arquivo_de_configuracao}}
```
{% endraw %}