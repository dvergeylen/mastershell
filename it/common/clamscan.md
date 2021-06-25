---
layout: default
title: "clamscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clamscan">
  <a href="/it/common/clamscan.html">clamscan</a> <a href="#clamscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scanner antivirus da linea di comando.
> Maggiori informazioni: <https://www.clamav.net>.

#### Analizza un file cercando vulnerabilità:
```shell
clamscan {{percorso/al/file}}
```
#### Analizza ricorsivamente tutti i file in una specifica directory:
```shell
clamscan -r {{percorso/alla/directory}}
```
#### Analizza dati da standard input:
```shell
{{comando}} | clamscan -
```
#### Specifica un file o directory di file da usare come database virus:
```shell
clamscan --database {{percorso/a/file_o_directory}}
```
#### Analizza la directory corrente e mostra in output solo i file infetti:
```shell
clamscan --infected
```
#### Scrivi il risultato di uno scan in un file di log:
```shell
clamscan --log {{percorso/a/file_log}}
```
#### Sposta i file infetti in una specifica directory:
```shell
clamscan --move {{percorso/a/directory_quarantena}}
```
#### Elimina i file infetti:
```shell
clamscan --remove yes
```
{% endraw %}