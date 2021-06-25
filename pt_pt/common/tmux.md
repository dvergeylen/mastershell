---
layout: default
title: "tmux"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}