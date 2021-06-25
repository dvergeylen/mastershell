---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#alias">alias</a>
* <a href="#batch">batch</a>
* <a href="#cd">cd</a>
* <a href="#chmod">chmod</a>
* <a href="#history">history</a>
* <a href="#tmux">tmux</a>
* <a href="#touch">touch</a>
* <a href="#xkill">xkill</a>

{% raw %}
<h2 id="alias">
  <a href="/pt_pt/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria um alias -- palavras que são substituídas por um comando.
> Alias expiram com a sessão da shell atual, a menos que sejam definidos no ficheiro de configuração da shell, por exemplo `~/.bashrc`.
> Mais informações: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listar todos os alias:
```shell
alias
```
#### Criar um alias genérico:
```shell
alias {{palavra}}="{{comando}}"
```
#### Visualizar o comando associado a um dado alias:
```shell
alias {{palavra}}
```
#### Remover um alias de um comando:
```shell
unalias {{palavra}}
```
#### Tornar `rm` num comando interativo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Criar `la` como um atalho para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="batch">
  <a href="/pt_pt/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executar comandos num momento mais tarde quando a carga do sistema permitir.
> O serviço atd (ou atrun) deve correr para atuais execuções.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Executar comandos da entrada padrão (premir `Ctrl + D` quando terminado):
```shell
batch
```
#### Executar um comando da entrada padrão:
```shell
echo "{{./criar_copia_bd.sh}}" | batch
```
#### Executar comandos de um dado ficheiro:
```shell
batch -f {{caminho/para/ficheiro}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/pt_pt/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mudar o diretório atual.
> Mais informações: <https://man.archlinux.org/man/cd.n>.

#### Ir para um dado diretório:
```shell
cd {{caminho/para/diretorio}}
```
#### Ir para o diretório base do utilizador atual:
```shell
cd
```
#### Ir para o diretório pai do diretório atual:
```shell
cd ..
```
#### Ir para o diretório anteriormente escolhido:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="chmod">
  <a href="/pt_pt/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alterar as permissões de acesso a um ficheiro ou diretório.
> Mais informações: <https://www.gnu.org/software/coreutils/chmod>.

#### Dar a um [u]tilizador que possui um ficheiro o direito a e[x]ecutá-lo:
```shell
chmod u+x {{ficheiro}}
```
#### Dar a um [u]tilizador direitos para le[r] e escrever ([w]) num ficheiro/diretório:
```shell
chmod u+rw {{ficheiro_ou_diretorio}}
```
#### Remover direitos de execução de um [g]rupo:
```shell
chmod g-x {{ficheiro}}
```
#### Dar a todos ([a]) os utilizadores o direito de le[r] e e[x]ecutar:
```shell
chmod a+rx {{ficheiro}}
```
#### Dar a [o]utros (que não estão no grupo do dono do ficheiro) os mesmos direitos do [g]rupo:
```shell
chmod o=g {{ficheiro}}
```
#### Remover todos os direitos dos [o]utros:
```shell
chmod o= {{ficheiro}}
```
#### Mudar as permissões, recursivamente, dando ao [g]rupo e [o]utros a possibilidade de escrever ([w]):
```shell
chmod -R g+w,o+w {{diretorio}}
```
{% endraw %}{% raw %}
<h2 id="history">
  <a href="/pt_pt/common/history.html">history</a> <a href="#history"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Histórico da linha de comandos.

#### Mostrar o histórico da linha de comandos por ordem cronológica:
```shell
history
```
#### Apagar o histórico da linha de comandos:
```shell
history -c
```
#### Mostrar o enésimo comando no histórico da linha de comandos:
```shell
history !{{n}}
```
#### Mostrar as entradas do histórico da linha de comandos que correspondem a uma expressão regular:
```shell
history | grep {{expressao_regular}}
```
{% endraw %}{% raw %}
<h2 id="tmux">
  <a href="/pt_pt/common/tmux.html">tmux</a> <a href="#tmux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplexador do terminal. Permite várias sessões com janelas, painéis e muito mais.
> Mais informações: <https://github.com/tmux/tmux>.

#### Iniciar uma nova sessão:
```shell
tmux
```
#### Iniciar uma sessão com nome:
```shell
tmux new-session -s {{nome}}
```
#### Listar sessões existentes:
```shell
tmux ls
```
#### Entrar na última sessão utilizada:
```shell
tmux attach-session
```
#### Entrar numa sessão com nome:
```shell
tmux attach-session -t {{nome}}
```
#### Sair da sessão atual (com o prefixo Ctrl-B):
```shell
Ctrl-B d
```
#### Eliminar uma sessão com nome:
```shell
tmux kill-session -t {{nome}}
```
#### Eliminar a sessão atual (com o prefixo Ctrl-B):
```shell
Ctrl-B :kill-session<Enter>
```
{% endraw %}{% raw %}
<h2 id="touch">
  <a href="/pt_pt/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar as timestamps de um ficheiro para a hora atual.
> Se o ficheiro não existir, cria um ficheiro vazio, a menos que seja passado o parâmetro -c ou -h.
> Mais informações: <https://www.gnu.org/software/coreutils/touch>.

#### Criar um novo ficheiro vazio, ou atualizar as timestamps para a hora atual:
```shell
touch {{ficheiro}}
```
#### Definir as timestamps de um ficheiro para a hora especificada:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{ficheiro}}
```
#### Usar as timestamps do ficheiro1 para definir as timestamps do ficheiro2:
```shell
touch -r {{ficheiro1}} {{ficheiro2}}
```
#### Alterar as timestamps de um ficheiro. Não cria novo ficheiro se não existir:
```shell
touch -c {{ficheiro}}
```
{% endraw %}{% raw %}
<h2 id="xkill">
  <a href="/pt_pt/common/xkill.html">xkill</a> <a href="#xkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Termina o cliente associado a um elemento gráfico.
> Utilizado para forçar a terminação de processos que não respondem ou não apresentam botão "fechar".

#### Ativar um cursor para fechar uma janela com o clique do botão esquerdo do rato (pressionar qualquer outro botão para cancelar):
```shell
xkill
```
{% endraw %}