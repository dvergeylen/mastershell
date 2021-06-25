---
layout: default
title: "alacritty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alacritty">
  <a href="/de/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattformübergreifender, GPU-beschleunigter Terminalemulator.
> Weitere Informationen: <https://github.com/alacritty/alacritty>.

#### Öffne ein neues Alacritty-Fenster:
```shell
alacritty
```
#### Starte Alacritty in einem bestimmten Arbeitsverzeichnis:
```shell
alacritty --working-directory {{pfad/zu/verzeichnis}}
```
#### Führe einen Befehl in einem neuen Alacritty-Fenster aus:
```shell
alacritty -e {{befehl}}
```
#### Gib eine alternative Konfigurations-Datei an (ist standardmäßig `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{pfad/zu/konfiguration.yml}}
```
#### Starte mit aktiviertem Live-Konfigurations-Neuladen (kann auch standardmäßig in `alacritty.yml` eingestellt werden):
```shell
alacritty --live-config-reload --config-file {{pfad/zu/konfiguration.yml}}
```
{% endraw %}