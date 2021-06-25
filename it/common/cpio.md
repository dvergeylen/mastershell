---
layout: default
title: "cpio"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpio">
  <a href="/it/common/cpio.html">cpio</a> <a href="#cpio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia file da/a archivi.
> Supporta i seguenti formati di archivio: cpio binario, vecchio ASCII, nuovo ASCII, crc, HPUX binario, HPUX vecchio ASCII, vecchio tar, e tar POSIX.1.
> Maggiori informazioni: <https://www.gnu.org/software/cpio>.

#### Accetta una lista di nomi di file da standard input ed aggiungili ad un archivio in formato binario cpio:
```shell
echo "{{file1}} {{file2}} {{file3}}" | cpio -o > {{archivio.cpio}}
```
#### Copia tutti i file e le directory in una directory ed aggiungili ad un archivio, in modalità verbosa:
```shell
find {{path/to/directory}} | cpio -ov > {{archivio.cpio}}
```
#### Estrai file da un archivio, generando le directory necessarie, in modalità verbosa:
```shell
cpio -idv < {{archivio.cpio}}
```
{% endraw %}