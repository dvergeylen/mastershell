---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cd">cd</a>
* <a href="#dir">dir</a>
* <a href="#find">find</a>
* <a href="#rmdir">rmdir</a>
* <a href="#shutdown">shutdown</a>

{% raw %}
<h2 id="cd">
  <a href="/nl/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de naam van de huidige werkmap weer of wijzigt deze.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Ga naar een directory in dezelfde drive:
```shell
cd {{pad/naar/directory}}
```
#### Geef de naam van de huidige directory weer:
```shell
cd
```
#### Ga naar de ouder van de huidige directory:
```shell
cd ..
```
#### Ga naar een directory in een andere drive:
```shell
cd {{pad/naar/directory}} /d
```
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/nl/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de inhoud weer van een directory.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Geef de inhoud weer van de huidige map:
```shell
dir
```
#### Geef de inhoud weer van een gegeven directory:
```shell
dir {{pad/naar/directory}}
```
#### Geef de inhoud weer van de huidige directory, inclusief verborgen bestanden:
```shell
dir /A
```
#### Geef de inhoud weer van een gegeven directory, inclusief verborgen bestanden:
```shell
dir {{pad/naar/directory}} /A
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/nl/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vind een gespecificieerde string in een bestand.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Vind de lijnen dat een specifieke string bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}}
```
#### Laat lijnen zie die de string niet bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /v
```
#### Toon het aantal lijnen dat de string bevat:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /c
```
#### Laat het aantal lijnen zien samen met de lijnen:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /n
```
{% endraw %}{% raw %}
<h2 id="rmdir">
  <a href="/nl/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwijdert een directory en zijn inhoud.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/rmdir>.

#### Verwijder een lege directory:
```shell
rmdir {{pad/naar/directory}}
```
#### verwijder een directory en zen inhoud recursief:
```shell
rmdir {{pad/naar/directory}} /s
```
#### verwijder een directory en zen inhoud recursief zonder te vragen:
```shell
rmdir {{pad/naar/directory}} /s /q
```
{% endraw %}{% raw %}
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