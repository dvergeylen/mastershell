---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#choco">choco</a>
* <a href="#choco-info">choco info</a>
* <a href="#choco-install">choco install</a>
* <a href="#choco-list">choco list</a>
* <a href="#choco-source">choco source</a>
* <a href="#choco-uninstall">choco uninstall</a>
* <a href="#choco-upgrade">choco upgrade</a>
* <a href="#cls">cls</a>
* <a href="#cmd">cmd</a>
* <a href="#dir">dir</a>
* <a href="#mkdir">mkdir</a>
* <a href="#print">print</a>
* <a href="#title">title</a>
* <a href="#tree">tree</a>
* <a href="#type">type</a>
* <a href="#ver">ver</a>
* <a href="#whoami">whoami</a>

{% raw %}
<h2 id="choco-info">
  <a href="/pt_br/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibir informações detalhadas de um pacote com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-info>.

#### Exibir informações sobre um pacote específico:
```shell
choco info {{pacote}}
```
#### Exibir informação para um pacote local:
```shell
choco info {{pacote}} --local-only
```
#### Especificar uma fonte personalizada para receber as informações de um pacote:
```shell
choco info {{pacote}} --source {{url_da_fonte|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco info {{pacote}} --user {{apelido}} --password {{senha}}
```
{% endraw %}{% raw %}
<h2 id="choco-install">
  <a href="/pt_br/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Instalar um pacote ou mais com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-install>.

#### Instalar um ou mais pacotes separado por espaço:
```shell
choco install {{pacote(s)}}
```
#### Instalar pacotes a partir de um aquivo de configuração personalizado:
```shell
choco install {{caminho/para/pacotes.config}}
```
#### Instalar um arquivo específico `nuspec` ou `nupkg`:
```shell
choco install {{caminho/para/arquivo}}
```
#### Instalar uma versão específica de um pacote:
```shell
choco install {{pacote}} --version {{versão}}
```
#### Permitir a instalação de múltiplas versões de um pacote:
```shell
choco install {{pacote}} --allow-multiple
```
#### Confirmar todos prompts automaticamente:
```shell
choco install {{pacote}} --yes
```
#### Especificar uma fonte personalizada para receber pacotes:
```shell
choco install {{pacote}} --source {{url_do_pacote|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco install {{pacote}} --user {{usuario}} --password {{senha}}
```
{% endraw %}{% raw %}
<h2 id="choco-list">
  <a href="/pt_br/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibir uma lista de pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-list>.

#### Exibir todos pacotes disponíveis:
```shell
choco list
```
#### Exibir todos pacotes instalados localmente:
```shell
choco list --local-only
```
#### Exibir uma lista incluindo programas locais:
```shell
choco list --include-programs
```
#### Exibir apenas pacotes aprovados:
```shell
choco list --approved-only
```
#### Especificar uma fonte personalizada para exibir os pacotes:
```shell
choco list --source {{url_da_fonte|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco list --user {{usuário}} --password {{senha}}
```
{% endraw %}{% raw %}
<h2 id="choco-source">
  <a href="/pt_br/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciar fontes para pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-source>.

#### Listar fontes atualmente disponíveis:
```shell
choco source list
```
#### Adicionar uma nova fonte de pacotes:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}}
```
#### Adicionar uma nova fonte de pacotes com credenciais:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}} --user {{nome}} --password {{senha}}
```
#### Adicionar uma nova fonte de pacotes com certificado do cliente:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}} --cert {{caminho/para/certificado}}
```
#### Habilitar uma fonte de pacotes:
```shell
choco source enable --name {{nome}}
```
#### Desabilitar uma fonte de pacotes:
```shell
choco source disable --name {{nome}}
```
#### Remover uma fonte de pacotes:
```shell
choco source remove --name {{nome}}
```
{% endraw %}{% raw %}
<h2 id="choco-uninstall">
  <a href="/pt_br/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desinstalar um pacote ou mais com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-uninstall>.

#### Desinstalar um pacote ou mais separado por espaços:
```shell
choco uninstall {{pacote(s)}}
```
#### Desinstalar uma versão específica de um pacote:
```shell
choco uninstall {{pacote}} --version {{versão}}
```
#### Confirmar todos prompts automaticamente:
```shell
choco uninstall {{pacote}} --yes
```
#### Remover todas dependências ao desinstalar:
```shell
choco uninstall {{pacote}} --remove-dependencies
```
#### Desinstalar todos os pacotes:
```shell
choco uninstall all
```
{% endraw %}{% raw %}
<h2 id="choco-upgrade">
  <a href="/pt_br/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar um ou mais pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-upgrade>.

#### Atualizar um ou mais pacotes separados por espaço:
```shell
choco upgrade {{pacote(s)}}
```
#### Atualizar para uma versão específica de um pacote:
```shell
choco upgrade {{pacote}} --version {{versão}}
```
#### Atualizar todos pacotes:
```shell
choco upgrade all
```
#### Atualizar todos os pacotes, exceto os especificados separados por virgula:
```shell
choco upgrade all --except "{{pacote(s)}}"
```
#### Confirmar todos prompts automaticamente:
```shell
choco upgrade {{pacote}} --yes
```
#### Especifique uma fonte personalizada para receber pacotes:
```shell
choco upgrade {{pacote}} --source {{url_do_pacote|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco upgrade {{pacote}} --user {{usuário}} --password {{senha}}
```
{% endraw %}{% raw %}
<h2 id="choco">
  <a href="/pt_br/windows/choco.html">choco</a> <a href="#choco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uma interface de linha de comando para o gerenciador de pacotes Chocolatey.
> Veja `choco install`, `choco upgrade` e outras páginas para mais informações.
> Mais informações: <https://chocolatey.org>.

#### Executar o comando Chocolatey:
```shell
choco {{comando}}
```
#### Exibir ajuda generalizada:
```shell
choco -?
```
#### Exibir ajuda em um comando específico:
```shell
choco {{comando}} -?
```
#### Exibir a versão do Chocolatey:
```shell
choco --version
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/pt_br/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Limpar a tela de saída.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/cls>.

#### Limpar a tela:
```shell
cls
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/pt_br/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Listar os conteúdos de um diretório.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/dir>.

#### Mostrar o conteúdo do diretório atual:
```shell
dir
```
#### Mostrar o conteúdo do diretório no caminho provido pelo usuário:
```shell
dir {{caminho/para/diretório}}
```
#### Mostrar o conteúdo do diretório atual, incluindo arquivos e pastas escondidas:
```shell
dir /A
```
#### Mostrar o conteúdo do diretório provido pelo usuário, incluindo arquivos e pastas escondidas:
```shell
dir {{caminho/para/diretório}} /A
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/pt_br/windows/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Criar um diretório.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/mkdir>.

#### Criar um diretório:
```shell
mkdir {{nome_do_diretorio}}
```
#### Criar recursivamente uma árvore de diretórios aninhados:
```shell
mkdir {{caminho/para/subdiretorio}}
```
{% endraw %}{% raw %}
<h2 id="print">
  <a href="/pt_br/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprimir um arquivo de texto em uma impressora.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/print>.

#### Imprimir um arquivo de texto na impressora padrão:
```shell
print {{caminho/para/arquivo}}
```
#### Imprimir arquivo de texto em uma impressora específica:
```shell
print /d:{{impressora}} {{caminho/para/arquivo}}
```
{% endraw %}{% raw %}
<h2 id="title">
  <a href="/pt_br/windows/title.html">title</a> <a href="#title"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe o título do prompt de comando.
> Mais informações: <https://docs.microsoft.com/windows-server/administration/windows-commands/title>.

#### Define o título do prompt de comando:
```shell
title {{novo_título}}
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/pt_br/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe uma árvore gráfica da estrutura do diretório no caminho.
> Mais informações: <https://docs.microsoft.com/windows-server/administration/windows-commands/tree>.

#### Exibe a árvore para o diretório atual:
```shell
tree
```
#### Exibe a árvore para o diretório específico:
```shell
tree {{caminho/para/diretório}}
```
#### Exibe a árvore para o diretório específico incluíndo arquivos:
```shell
tree {{caminho/para/diretório}} /f
```
#### Exibe a árvore usando caractéres ASCII:
```shell
tree {{caminho/para/diretório}} /a
```
{% endraw %}{% raw %}
<h2 id="type">
  <a href="/pt_br/windows/type.html">type</a> <a href="#type"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostrar o conteúdo de um arquivo.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/type>.

#### Mostrar o conteúdo de um arquivo específico:
```shell
type {{caminho/para/arquivo}}
```
{% endraw %}{% raw %}
<h2 id="ver">
  <a href="/pt_br/windows/ver.html">ver</a> <a href="#ver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe a atual versão do Windows ou MS-DOS.
> Mais informações: <https://docs.microsoft.com/windows-server/administration/windows-commands/ver>.

#### Mostra a atual versão:
```shell
ver
```
{% endraw %}{% raw %}
<h2 id="whoami">
  <a href="/pt_br/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra detalhes sobre o usuário atual.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/whoami>.

#### Mostra o username do usuário atual:
```shell
whoami
```
#### Mostra os grupos dos quais o usuário atual faz parte:
```shell
whoami /groups
```
#### Mostra os privilégios do usuário atual:
```shell
whoami /priv
```
#### Mostra o nome principal (UPN) do usuário atual:
```shell
whoami /upn
```
#### Mostra o id de logon do usuário atual:
```shell
whoami /logonid
```
{% endraw %}