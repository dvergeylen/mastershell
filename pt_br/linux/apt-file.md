---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/pt_br/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Buscador de arquivos nos pacotes apt, incluindo os não instalados.
> Mais informações: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Atualizar as informações dos pacotes a partir de todos os repositórios remotos:
```shell
sudo apt update
```
#### Buscar por pacotes que contêm o arquivo ou caminho especificado:
```shell
apt-file search {{nome_do_pacote_ou_caminho}}
```
#### Listar o conteúdo de um pacote específico:
```shell
apt-file list {{nome_do_pacote}}
```
{% endraw %}