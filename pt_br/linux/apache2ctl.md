---
layout: default
title: "apache2ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apache2ctl">
  <a href="/pt_br/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de controle do servidor web HTTP Apache.
> Este comando está disponível nas distribuições baseadas em Debian, para as baseadas em RHEL veja `httpd`.
> Mais informações: <https://manpages.debian.org/latest/apache2/apache2ctl.8.html>.

#### Iniciar o Apache. Caso ele já esteja em execução, uma mensagem será apresentada:
```shell
sudo apache2ctl start
```
#### Encerrar o Apache:
```shell
sudo apache2ctl stop
```
#### Reiniciar o Apache:
```shell
sudo apache2ctl restart
```
#### Verificar se o arquivo de configuração está correto sintaticamente:
```shell
sudo apache2ctl -t
```
#### Listar os módulos carregados:
```shell
sudo apache2ctl -M
```
{% endraw %}