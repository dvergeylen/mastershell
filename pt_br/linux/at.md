---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/pt_br/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa comandos em um determinado momento.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Iniciar o prompt `at` para que um novo conjunto de comandos seja agendado, pressione `Ctrl + D` para salvar e sair:
```shell
at {{hh:mm:ss}}
```
#### Executar os comandos e enviar o resultado por e-mail utilizando algum programa de envio de e-mail local, por exemplo o sendmail:
```shell
at {{hh:mm:ss}} -m
```
#### Executar um script em um determinado momento:
```shell
at {{hh:mm:ss}} -f {{caminho_para_o_script}}
```
{% endraw %}