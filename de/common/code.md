---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/de/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> Weitere Informationen: <https://github.com/microsoft/vscode>.

#### Öffne VS Code:
```shell
code
```
#### Öffne das aktuelle Verzeichnis in VS Code:
```shell
code .
```
#### Öffne eine bestimmte Datei oder Verzeichnis in VS Code:
```shell
code {{pfad/zu/datei_oder_verzeichnis}}
```
#### Öffne eine Datei oder ein Verzeichnis im aktuell geöffnetem VS Code Fenster:
```shell
code --reuse-window {{pfad/zu/datei_oder_verzeichnis}}
```
#### Öffne mehrere Dateien in VS Code:
```shell
code -d {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Öffne VS Code root:
```shell
sudo code {{pfad/zu/datei_oder_verzeichnis}} --user-data-dir
```
{% endraw %}