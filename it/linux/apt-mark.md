---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/it/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio per cambiare lo stato di un pacchetto installato.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Contrassegna un pacchetto come installato automaticamente:
```shell
sudo apt-mark auto {{nome_del_pacchetto}}
```
#### Mantiene un pacchetto alla sua versione attuale e ne previene l'aggiornamento:
```shell
sudo apt-mark hold {{nome_del_pacchetto}}
```
#### Consente ad un pacchetto di essere nuovamente aggiornato:
```shell
sudo apt-mark unhold {{nome_del_pacchetto}}
```
#### Mostra i pacchetti installati manualmente:
```shell
apt-mark showmanual
```
#### Visualizza i pacchetti mantenuti alla versione attuale che non sono stati aggiornati:
```shell
apt-mark showhold
```
{% endraw %}