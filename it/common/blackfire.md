---
layout: default
title: "blackfire"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blackfire">
  <a href="/it/common/blackfire.html">blackfire</a> <a href="#blackfire"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di profilazione da linea di comando per PHP.
> Maggiori informazioni: <https://blackfire.io>.

#### Inizializza e configura il client Blackfire:
```shell
blackfire config
```
#### Lancia l'agent Blackfire:
```shell
blackfire agent
```
#### Lancia l'agent Blackfire su uno specifico socket:
```shell
blackfire agent --socket="{{tcp://127.0.0.1:8307}}"
```
#### Lancia il profiler su uno specifico programma:
```shell
blackfire run {{php percorso/al/file.php}}
```
#### Lancia il profiler e raccogli 10 campioni:
```shell
blackfire --samples={{10}} run {{php percorso/al/file.php}}
```
#### Lancia il profiler e mostra i risultati in output come JSON:
```shell
blackfire --json run {{php percorso/al/file.php}}
```
#### Carica un file del profiler sul servizio web di Blackfire:
```shell
blackfire upload {{percorso/al/file}}
```
#### Mostra lo stato dei profili sul servizio web di Blackfire:
```shell
blackfire status
```
{% endraw %}