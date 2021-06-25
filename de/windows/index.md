---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cd">cd</a>
* <a href="#choco">choco</a>
* <a href="#choco-feature">choco feature</a>
* <a href="#choco-info">choco info</a>
* <a href="#choco-install">choco install</a>
* <a href="#choco-list">choco list</a>
* <a href="#choco-new">choco new</a>
* <a href="#choco-outdated">choco outdated</a>
* <a href="#choco-pack">choco pack</a>
* <a href="#choco-pin">choco pin</a>
* <a href="#choco-search">choco search</a>
* <a href="#choco-source">choco source</a>
* <a href="#choco-uninstall">choco uninstall</a>
* <a href="#choco-upgrade">choco upgrade</a>
* <a href="#choco-apikey">choco-apikey</a>
* <a href="#scoop">scoop</a>
* <a href="#scoop-bucket">scoop bucket</a>

{% raw %}
<h2 id="cd">
  <a href="/de/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige den Namen des aktuellen Arbeitsverzeichnisses an oder ändere dieses.
> Weitere Informationen: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Wechsle zu einem Verzeichnis im selben Laufwerk:
```shell
cd {{pfad/zu/verzeichnis}}
```
#### Zeige den Namen des aktuellen Verzeichnisses an:
```shell
cd
```
#### Wechsle zum übergeordneten Verzeichnis des aktuellen Verzeichnisses:
```shell
cd ..
```
#### Wechsle in ein Verzeichnis auf einem anderen Laufwerk:
```shell
cd {{pfad/zu/verzeichnis}} /d
```
{% endraw %}{% raw %}
<h2 id="choco-apikey">
  <a href="/de/windows/choco-apikey.html">choco-apikey</a> <a href="#choco-apikey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte die API-Schlüssel für die Quellen von Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-apikey>.

#### Gib eine Liste von Quellen und ihren API-Schlüsseln aus:
```shell
choco apikey
```
#### Zeige eine bestimmte Quelle und ihren API-Schlüssel an:
```shell
choco apikey --source "{{quell_url}}"
```
#### Setze den API-Schlüssel für eine Quelle:
```shell
choco apikey --source "{{quell_url}}" --key "{{api_schluessel}}"
```
#### Entferne den API-Schlüssel einer Quelle:
```shell
choco apikey --source "{{quell_url}}" --remove
```
{% endraw %}{% raw %}
<h2 id="choco-feature">
  <a href="/de/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interagiere mit Funktionen, die das Verhalten von Chocolatey verändern.
> Weitere Informationen: <https://chocolatey.org/docs/commands-feature>.

#### Gib eine Liste von verfügbaren Funktionen aus:
```shell
choco feature list
```
#### Aktiviere eine Funktion:
```shell
choco feature enable --name {{name}}
```
#### Deaktiviere eine Funktion:
```shell
choco feature disable --name {{name}}
```
{% endraw %}{% raw %}
<h2 id="choco-info">
  <a href="/de/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige ausführliche Informationen über ein Chocolatey-Paket an.
> Weitere Informationen: <https://chocolatey.org/docs/commands-info>.

#### Zeige Informationen über ein bestimmtes Paket an:
```shell
choco info {{paket}}
```
#### Zeige Informationen über ein bestimmtes lokales Paket an:
```shell
choco info {{paket}} --local-only
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco info {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco info {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco-install">
  <a href="/de/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere ein oder mehrere Pakete mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-install>.

#### Installiere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco install {{paket1}} {{paket2}}
```
#### Installiere Pakete aus einer Konfigurationsdatei:
```shell
choco install {{pfad/zu/pakete.config}}
```
#### Installiere Pakete aus einer `nuspec`- oder `nupkg`-Datei:
```shell
choco install {{pfad/zu/datei}}
```
#### Installiere eine bestimmte Version eines Pakets:
```shell
choco install {{paket}} --version {{version}}
```
#### Erlaube die gleichzeitige Installation mehrerer Versionen eines Pakets:
```shell
choco install {{paket}} --allow-multiple
```
#### Stimme allen Fragen automatisch zu:
```shell
choco install {{paket}} --yes
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco install {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco install {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco-list">
  <a href="/de/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige mit Chocolatey eine Liste von Paketen an.
> Weitere Informationen: <https://chocolatey.org/docs/commands-list>.

#### Zeige alle verfügbaren Pakete an:
```shell
choco list
```
#### Zeige alle lokal installierten Pakete an:
```shell
choco list --local-only
```
#### Zeige eine Liste einschließlich der lokalen Windows-Programme an:
```shell
choco list --include-programs
```
#### Zeige nur zugelassene Pakete an:
```shell
choco list --approved-only
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco list --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco list --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco-new">
  <a href="/de/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle neue Paket-Beschreibungs-Dateien mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-new>.

#### Erstelle ein neues Grundgerüst für ein Paket:
```shell
choco new {{paket_name}}
```
#### Erstelle ein neues Paket mit einer bestimmten Version:
```shell
choco new {{paket_name}} --version {{version}}
```
#### Erstelle ein neues Paket mit einem bestimmten Betreuer*innen-Namen:
```shell
choco new {{paket_name}} --maintainer {{betreuer*innen_name}}
```
#### Erstelle ein neues Paket in einem bestimmten Ausgabe-Verzeichnis:
```shell
choco new {{paket_name}} --output-directory {{pfad/zu/verzeichnis}}
```
#### Erstelle ein neues Paket mit verschiedenen URLs für die 32-Bit und 64-Bit Installationsroutinen:
```shell
choco new {{paket_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}{% raw %}
<h2 id="choco-outdated">
  <a href="/de/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Überprüfe mit Chocolatey, ob Pakete veraltet sind.
> Weitere Informationen: <https://chocolatey.org/docs/commands-outdated>.

#### Zeige eine Liste von veralteten Paketen im Tabellen-Format:
```shell
choco outdated
```
#### Ignoriere angeheftete Pakete in der Ausgabe:
```shell
choco outdated --ignore-pinned
```
#### Gib eine eigene Quelle an, mit der die Aktualität der Pakete überprüft wird:
```shell
choco outdated --source {{source_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco outdated --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco-pack">
  <a href="/de/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verpacke eine NuGet-Spezifikation in eine nupkg-Datei.
> Weitere Informationen: <https://chocolatey.org/docs/commands-pack>.

#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei:
```shell
choco pack {{pfad/zu/spezifikation}}
```
#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei und bestimme die Version der ausgegebenen Datei:
```shell
choco pack {{pfad/zu/spezifikation}} --version {{version}}
```
#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei, welche in einem bestimmten Verzeichnis gespeichert wird:
```shell
choco pack {{pfad/zu/spezifikation}} --output-directory {{pfad/zu/ausgabe_verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="choco-pin">
  <a href="/de/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hefte ein Chocolatey-Paket bei einer bestimmten Version an.
> Angeheftete Pakete werden nicht weiter aktualisiert.
> Weitere Informationen: <https://chocolatey.org/docs/commands-pin>.

#### Zeige eine Liste der angehefteten Pakete und ihrer Versionen an:
```shell
choco pin list
```
#### Hefte ein Paket in der installierten Version an:
```shell
choco pin add --name {{paket}}
```
#### Hefte ein Paket in einer bestimmten Version an:
```shell
choco pin add --name {{paket}} --version {{version}}
```
#### Entferne die Anheftung für ein bestimmtes Paket:
```shell
choco pin remove --name {{paket}}
```
{% endraw %}{% raw %}
<h2 id="choco-search">
  <a href="/de/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Suche mit Chocolatey nach einem lokal oder im Internet verfügbaren Paket.
> Weitere Informationen: <https://chocolatey.org/docs/commands-search>.

#### Suche nach einem Paket:
```shell
choco search {{suchabfrage}}
```
#### Suche nur lokal nach einem Paket:
```shell
choco search {{suchabfrage}} --local-only
```
#### Suche nur nach genauen Übereinstimmungen:
```shell
choco search {{suchabfrage}} --exact
```
#### Stimme allen Fragen automatisch zu:
```shell
choco search {{suchabfrage}} --yes
```
#### Gib eine eigene Quelle an, welche nach Paketen durchsucht wird:
```shell
choco search {{suchabfrage}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco search {{suchabfrage}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco-source">
  <a href="/de/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte die Paketquellen mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-source>.

#### Gib alle momentan verfügbaren Quellen aus:
```shell
choco source list
```
#### Füge eine neue Paketquelle hinzu:
```shell
choco source add --name {{name}} --source {{url}}
```
#### Füge eine neue Paketquelle mit Zugangsdaten hinzu:
```shell
choco source add --name {{name}} --source {{url}} --user {{benutzername}} --password {{passwort}}
```
#### Füge eine neue Paketquelle mit Client-Zertifikat hinzu:
```shell
choco source add --name {{name}} --source {{url}} --cert {{pfad/zu/zertifikat}}
```
#### Aktiviere eine Paketquelle:
```shell
choco source enable --name {{name}}
```
#### Deaktiviere eine Paketquelle:
```shell
choco source disable --name {{name}}
```
#### Entferne eine Paketquelle:
```shell
choco source remove --name {{name}}
```
{% endraw %}{% raw %}
<h2 id="choco-uninstall">
  <a href="/de/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deinstalliere mit Chocolatey ein oder mehrere Pakete.
> Weitere Informationen: <https://chocolatey.org/docs/commands-uninstall>.

#### Deinstalliere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco uninstall {{paket(e)}}
```
#### Deinstalliere eine bestimmte Version eines Paketes:
```shell
choco uninstall {{paket}} --version {{version}}
```
#### Stimme allen Fragen automatisch zu:
```shell
choco uninstall {{paket}} --yes
```
#### Deinstalliere auch alle Abhängigkeiten:
```shell
choco uninstall {{paket}} --remove-dependencies
```
#### Deinstalliere alle Pakete:
```shell
choco uninstall all
```
{% endraw %}{% raw %}
<h2 id="choco-upgrade">
  <a href="/de/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aktualisiere mit Chocolatey ein oder mehrere Pakete.
> Weitere Informationen: <https://chocolatey.org/docs/commands-upgrade>.

#### Aktualisiere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco upgrade {{paket(e)}}
```
#### Aktualisiere auf eine bestimmte Version des Pakets:
```shell
choco upgrade {{paket}} --version {{version}}
```
#### Aktualisiere alle Pakete:
```shell
choco upgrade all
```
#### Aktualisiere alle außer den angegebenen, durch Kommas getrennten Paketen:
```shell
choco upgrade all --except "{{paket(e)}}"
```
#### Stimme allen Fragen automatisch zu:
```shell
choco upgrade {{paket}} --yes
```
#### Gib eine eigene Quelle an, von der Pakete aktualisiert werden:
```shell
choco upgrade {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco upgrade {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="choco">
  <a href="/de/windows/choco.html">choco</a> <a href="#choco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Kommandozeilenwerkzeug für die Chocolatey Paketverwaltung.
> Schau dir `choco install`, `choco upgrade` und andere Seiten für weitergehende Informationen an.
> Weitere Informationen: <https://chocolatey.org>.

#### Führe einen Chocolatey-Befehl aus:
```shell
choco {{befehl}}
```
#### Zeige die allgemeine Hilfe an:
```shell
choco -?
```
#### Zeige die Hilfe für einen bestimmten Befehl an:
```shell
choco {{befehl}} -?
```
#### Überprüfe die Version von Chocolatey:
```shell
choco --version
```
{% endraw %}{% raw %}
<h2 id="scoop-bucket">
  <a href="/de/windows/scoop-bucket.html">scoop bucket</a> <a href="#scoop-bucket"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte "Eimer": Git-Repositories, welche Dateien enthalten, die beschreiben, wie Scoop Programme installiert werden.
> Kennt Scoop nicht die URL eines Eimers, so muss diese angegeben werden.
> Weitere Informationen: <https://github.com/lukesampson/scoop/wiki/Buckets>.

#### Liste alle Eimer auf, die gerade aktiv sind:
```shell
scoop bucket list
```
#### Liste alle bekannten Eimer auf:
```shell
scoop bucket known
```
#### Aktiviere einen bekannten Eimer:
```shell
scoop bucket add {{name}}
```
#### Aktiviere einen unbekannten Eimer durch die Angabe eines Namens und einer Git-Repository-URL:
```shell
scoop bucket add {{name}} {{https://beispiel.de/repository.git}}
```
#### Deaktiviere einen Eimer:
```shell
scoop bucket rm {{name}}
```
{% endraw %}{% raw %}
<h2 id="scoop">
  <a href="/de/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Kommandozeilenwerkzeug, um Windows-Programme (hier bezeichnet als Pakete) zu installieren.
> Weitere Informationen: <https://scoop.sh>.

#### Installiere ein Paket:
```shell
scoop install {{paket}}
```
#### Entferne ein Paket:
```shell
scoop uninstall {{paket}}
```
#### Aktualisiere alle installierten Pakete:
```shell
scoop update *
```
#### Zeige alle installierten Pakete an:
```shell
scoop list
```
#### Zeige Informationen über ein bestimmtes Paket an:
```shell
scoop info {{paket}}
```
#### Suche nach einem Paket:
```shell
scoop search {{paket}}
```
#### Entferne die alten Versionen aller Pakete und lösche den Download-Zwischenspeicher:
```shell
scoop cleanup -k *
```
{% endraw %}