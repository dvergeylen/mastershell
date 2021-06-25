---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/pt_br/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell, um interpretador de linha de comando compatível com `sh`.
> Veja também `histexpand` para a expansão do histórico.
> Mais informações: <https://gnu.org/software/bash/>.

#### Iniciar uma seção interativa do shell:
```shell
bash
```
#### Executar um comando e sair:
```shell
bash -c "{{comando}}"
```
#### Executar um script:
```shell
bash {{caminho/para/script.sh}}
```
#### Executar um script, exibindo cada comando antes de executá-lo:
```shell
bash -x {{caminho/para/script.sh}}
```
#### Executar os comandos de um script, parando de executar no primeiro erro:
```shell
bash -e {{caminho/para/script.sh}}
```
#### Ler e executar comandos do stdin (entrada padrão):
```shell
bash -s
```
#### Exibir a versão do Bash (`$BASH_VERSION` abrange apenas a versão sem informações da licença):
```shell
bash --version
```
{% endraw %}