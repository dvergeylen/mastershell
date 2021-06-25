---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/pt_br/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> Mais informações: <https://github.com/microsoft/vscode>.

#### Abrir o VS Code:
```shell
code
```
#### Abrir o diretório atual no VS Code:
```shell
code .
```
#### Abrir um arquivo ou diretório no VS Code:
```shell
code {{caminho/para/arquivo-ou-diretório}}
```
#### Abrir um arquivo ou diretório numa janela já aberta do VS Code:
```shell
code --reuse-window {{caminho/para/arquivo-ou-diretório}}
```
#### Comparar o conteúdo de dois arquivos no VS Code:
```shell
code -d {{arquivo1}} {{arquivo2}}
```
#### Iniciar o VS Code com permissão de super usuário (sudo):
```shell
sudo code {{path/to/file_or_directory}} --user-data-dir
```
{% endraw %}