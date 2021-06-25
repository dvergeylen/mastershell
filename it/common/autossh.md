---
layout: default
title: "autossh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autossh">
  <a href="/it/common/autossh.html">autossh</a> <a href="#autossh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegue, monitora e riavvia connessioni SSH.
> Si riconnette automaticamente per tenere attivi tunnel di port forwarding. Accetta tutte le flag di ssh.
> Maggiori informazioni: <https://harding.motd.ca/autossh>.

#### Apri una sessione SSH, riavviandola quando una porta monitorata smette di rispondere:
```shell
autossh -M {{porta_monitorata}} {{comando_ssh}}
```
#### Apri una sessione ssh che forwarda una porta locale verso una remota, riavviandola se necessario:
```shell
autossh -M {{porta_monitorata}} -L {{porta_locale}}:localhost:{{porta_remota}} {{utente}}@{{host}}
```
#### Forka prima di eseguire il comando ssh (si avvia in background) e non aprire una shell remota:
```shell
autossh -f -M {{porta_monitorata}} -N {{comando_ssh}}
```
#### Esegui autossh in background, senza una porta da monitorare, utilizzando i keep-alive di SSH ogni 10 secondi per rilevare una disconnessione:
```shell
autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" {{comando_ssh}}
```
#### Esegui autossh in background, senza una porta da monitorare, senza una shell remota, uscendo se il port forwarding fallisce:
```shell
autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" -o ExitOnForwardFailure=yes -L {{porta_locale}}:localhost:{{porta_remota}} {{utente}}@{{host}}
```
#### Esegui autossh in background con output di debug su un file e output verboso di ssh su un altro file:
```shell
AUTOSSH_DEBUG=1 AUTOSSH_LOGFILE={{file_log}} autossh -f -M {{porta_monitorata}} -v -E {{file_log_ssh}} {{comando_ssh}}
```
{% endraw %}