---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/pt_br/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário que altera as configurações dos pacotes instalados.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marcar um pacote como instalado automaticamente:
```shell
sudo apt-mark auto {{nome_do_pacote}}
```
#### Bloquear um pacote na sua versão atual, impedindo que ele seja atualizado:
```shell
sudo apt-mark hold {{nome_do_pacote}}
```
#### Desbloquear um pacote, permitindo que ele seja atualizado:
```shell
sudo apt-mark unhold {{nome_do_pacote}}
```
#### Listar os pacotes instalados manualmente:
```shell
apt-mark showmanual
```
#### Listar os pacotes bloqueados:
```shell
apt-mark showhold
```
{% endraw %}