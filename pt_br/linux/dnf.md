---
layout: default
title: "dnf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dnf">
  <a href="/pt_br/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em RHEL (substituto do yum).

#### Instalar um novo pacote:
```shell
sudo dnf install {{nome_do_pacote}}
```
#### Instalar um novo pacote e responder sim para todas as questões:
```shell
sudo dnf -y install {{nome_do_pacote}}
```
#### Remover um pacote:
```shell
sudo dnf remove {{nome_do_pacote}}
```
#### Atualizar todos os pacotes instalados para as versões mais recentes:
```shell
sudo dnf upgrade
```
{% endraw %}