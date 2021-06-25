---
layout: default
title: "chcon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chcon">
  <a href="/it/common/chcon.html">chcon</a> <a href="#chcon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia contesto di sicurezza SELinux di file o directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/chcon>.

#### Mostra il contesto di sicurezza di un file:
```shell
ls -lZ {{percorso/al/file}}
```
#### Cambia il contesto di sicurezza di un file usandone un'altro come riferimento:
```shell
chcon --reference={{file_di_riferimento}} {{file}}
```
#### Cambia l'intero contesto di sicurezza SELinux di un file:
```shell
chcon {{utente}}:{{ruolo}}:{{tipo}}:{{range/livello}} {{file}}
```
#### Cambia solo l'utente di un contesto di sicurezza SELinux:
```shell
chcon -u {{utente}} {{file}}
```
#### Cambia solo il ruolo di un contesto di sicurezza SELinux:
```shell
chcon -r {{ruolo}} {{file}}
```
#### Cambia solo il tipo di un contesto di sicurezza SELinux:
```shell
chcon -t {{tipo}} {{file}}
```
#### Cambia solo il range/livello di un contesto di sicurezza SELinux:
```shell
chcon -l {{range/livello}} {{file}}
```
{% endraw %}