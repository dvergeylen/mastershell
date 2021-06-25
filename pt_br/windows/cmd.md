---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/pt_br/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> O interpretador de comandos do Windows.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/cmd>.

#### Iniciar nova instância do interpretador de comandos:
```shell
cmd
```
#### Executar o comando especificado e sair do interpretador:
```shell
cmd /c "{{comando}}"
```
#### Executar o comando especificado e entrar no shell interativo:
```shell
cmd /k "{{comando}}"
```
#### Desabilitar o uso do comando `echo` na saída dos comandos:
```shell
cmd /q
```
#### Habilitar ou desabilitar extensão de comandos:
```shell
cmd /e:{{on|off}}
```
#### Habilitar ou desabilitar a ferramenta que completa automaticamente o nome de arquivos ou diretórios:
```shell
cmd /f:{{on|off}}
```
#### Habilitar ou desabilitar a expansão de variáveis de ambiente:
```shell
cmd /v:{{on|off}}
```
#### Forçar que a saída de comandos use o padrão Unicode:
```shell
cmd /u
```
{% endraw %}