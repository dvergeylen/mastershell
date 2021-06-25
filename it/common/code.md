---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/it/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> Maggiori informazioni: <https://github.com/microsoft/vscode>.

#### Apri VS Code:
```shell
code
```
#### Apri la directory corrente in VS Code:
```shell
code .
```
#### Apri un file o una directory in VS Code:
```shell
code {{percorso/a/file_o_directory}}
```
#### Apri un file o una directory nella finestra attualmente aperta di VS Code:
```shell
code --reuse-window {{percorso/a/file_o_directory}}
```
#### Confronta due file in VS Code:
```shell
code -d {{file1}} {{file2}}
```
{% endraw %}