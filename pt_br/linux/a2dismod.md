---
layout: default
title: "a2dismod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dismod">
  <a href="/pt_br/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desativa um módulo do Apache em sistemas operacionais baseados no Debian.
> Mais informações: <https://manpages.debian.org/buster/apache2/a2dismod.8.en.html>.

#### Desativar um módulo:
```shell
sudo a2dismod {{módulo}}
```
#### Não mostrar mensagens informativas:
```shell
sudo a2dismod --quiet {{módulo}}
```
{% endraw %}