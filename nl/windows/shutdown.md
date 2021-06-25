---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/nl/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een tool om een machine af te sluiten, her op te starten of af te melden.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/shutdown>.

#### Sluit de huidige machine af:
```shell
shutdown /s
```
#### Sluit de huidige machine af en sluit alle applicaties:
```shell
shutdown /s /f
```
#### Herstart de huidige machine:
```shell
shutdown /r /t 0
```
#### Zet de huidige machine in slaapstand:
```shell
shutdown /h
```
#### Log uit van de huidige machine:
```shell
shutdown /l
```
#### Zet een timer in aantal seconden voor het afsluiten van de huidige machine:
```shell
shutdown /s /t {{seconden}}
```
#### Breek een afsluit sequentie af vooraleer de timer was afgelopen:
```shell
shutdown /a
```
#### Sluit een machine af op afstand:
```shell
shutdown /m {{\\hostnaam}}
```
{% endraw %}