---
layout: default
title: "crontab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crontab">
  <a href="/it/common/crontab.html">crontab</a> <a href="#crontab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programma cron job per essere eseguiti a determinati intervalli di tempo per l'utente corrente.
> Formato definizione di un job: "(minuto) (ora) (giorno_del_mese) (mese) (giorno_della_settimana) comando_da_eseguire".
> Maggiori informazioni: <https://manned.org/crontab>.

#### Modifica il file crontab per l'utente corrente:
```shell
crontab -e
```
#### Elenca i cron job esistenti per l'utente corrente:
```shell
crontab -l
```
#### Rimuovi tutti i cron job per l'utente corrente:
```shell
crontab -r
```
#### Esempio di un job eseguito alle 10:00 ogni giorno (* vuol dire qualsiasi valore):
```shell
0 10 * * * {{comando_da_eseguire}}
```
#### Esempio di un job eseguito ogni minuto il 3 Aprile:
```shell
* * 3 Apr * {{comando_da_eseguire}}
```
#### Esempio di un job che esegue un determinato script alle 02:30 ogni venerdì:
```shell
30 2 * * Fri {{/percorso/assoluto/allo/script.sh}}
```
{% endraw %}