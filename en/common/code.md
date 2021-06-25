---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/en/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> More information: <https://github.com/microsoft/vscode>.

#### Open VS Code:
```shell
code
```
#### Open the current directory in VS Code:
```shell
code .
```
#### Open a file or directory in VS Code:
```shell
code {{path/to/file_or_directory}}
```
#### Open a file or directory in the currently open VS Code window:
```shell
code --reuse-window {{path/to/file_or_directory}}
```
#### Compare two files in VS Code:
```shell
code -d {{file1}} {{file2}}
```
#### Open VS Code with super user (sudo) permissions:
```shell
sudo code {{path/to/file_or_directory}} --user-data-dir
```
{% endraw %}