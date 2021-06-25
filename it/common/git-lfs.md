---
layout: default
title: "git lfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-lfs">
  <a href="/it/common/git-lfs.html">git lfs</a> <a href="#git-lfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lavora con file di grandi dimensioni in repository Git.
> Maggiori informazioni: <https://git-lfs.github.com>.

#### Inizializza Git LFS:
```shell
git lfs install
```
#### Tieni traccia dei file che soddisfano un criterio glob:
```shell
git lfs track '{{*.bin}}'
```
#### Cambia l'URL endpoint di Git LFS (utile quando server LFS e server Git sono separati):
```shell
git config -f .lfsconfig lfs.url {{lfs_url_endpoint}}
```
#### Elenca i criteri tracciati:
```shell
git lfs track
```
#### Elenca i file tracciati che sono già stati salvati in un commit:
```shell
git lfs ls-files
```
#### Invia tutti gli oggetti Git LFS al server remoto (utile in caso di errori):
```shell
git lfs push --all {{nome_repository_remoto}} {{nome_ramo}}
```
#### Scarica tutti gli oggetti Git LFS:
```shell
git lfs fetch
```
#### Ripristina gli oggetti Git LFS:
```shell
git lfs checkout
```
{% endraw %}