---
layout: default
title: "duplicity"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="duplicity">
  <a href="/it/common/duplicity.html">duplicity</a> <a href="#duplicity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea archivi incrementali, compressi, cifrati con controllo di versione.
> Può caricare i backup su una varietà di servizi backend.
> Maggiori informazioni: <http://duplicity.nongnu.org>.

#### Esegui il backup di una directory via FTPS su una macchina remota, cifrandolo con una password:
```shell
FTP_PASSWORD={{password_login_ftp}} PASSPHRASE={{password_cifratura}} duplicity {{percorso/a/cartella_sorgente}} {{ftps://utente@hostname/percorso/a/cartella_target/}}
```
#### Esegui il backup di una directory in un server Amazon S3, facendo un backup completo ogni mese:
```shell
duplicity --full-if-older-than {{1M}} --use-new-style s3://{{nome_bucket[/prefisso]}}
```
#### Elimina le versioni più vecchie di un anno da un backup salvato in un server WebDAV:
```shell
FTP_PASSWORD={{password_login_webdav}} duplicity remove-older-than {{1Y}} --force {{webdav[s]://utente@hostname[:porta]/directory}}
```
#### Elenca i backup disponibili:
```shell
duplicity collection-status "file://{{percorso/assoluto/a/directory/di/backup}}"
```
#### Elenca i file in un backup salvato su una macchina remota, via SSH:
```shell
duplicity list-current-files --time {{YYYY-MM-DD}} scp://{{utente@hostname}}/percorso/a/directory/backup
```
#### Ripristina una sotto-directory da un backup locale cifrato con GnuPG in una posizione precisa:
```shell
PASSPHRASE={{password_chiave_gpg}} duplicity restore --encrypt-key {{id_chiave_gpg}} --file-to-restore {{percorso/relativo/sotto_directory}} file://{{percorso/assoluto/a/directory/di/backup}} {{percorso/a/directory/dove/ripristinare}}
```
{% endraw %}