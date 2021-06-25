---
layout: default
title: "diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff">
  <a href="/it/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Confronta file e directory.

#### Confronta due file (elenca cambiamenti necessari per trasformare `vecchio_file` in `nuovo_file`):
```shell
diff {{vecchio_file}} {{nuovo_file}}
```
#### Confronta due file ignorando gli spazi:
```shell
diff -w {{vecchio_file}} {{nuovo_file}}
```
#### Confronta due file mostrando le differenze fianco a fianco:
```shell
diff -y {{vecchio_file}} {{nuovo_file}}
```
#### Confronta due file, mostrando le differenze in formato unificato (come `git diff`):
```shell
diff -u {{vecchio_file}} {{nuovo_file}}
```
#### Confronta due directory ricorsivamente (mostra i nomi dei file/directory diversi e le differenze trai file):
```shell
diff -r {{old_directory}} {{new_directory}}
```
#### Confronta due directory mostrando solamente il nome dei file diversi:
```shell
diff -rq {{old_directory}} {{new_directory}}
```
{% endraw %}