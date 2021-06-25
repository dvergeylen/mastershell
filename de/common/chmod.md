---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/de/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ändere die Zugriffsberechtigungen einer Datei oder eines Verzeichnisses.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chmod>.

#### Gib dem Besitzer einer Datei ([u]ser) das Recht, sie auszuführen (e[x]ecute):
```shell
chmod u+x {{pfad/zu/datei}}
```
#### Gib dem Besitzer ([u]ser) Rechte zum Lesen ([r]ead) und Schreiben ([w]rite) einer Datei / einem Verzeichnis:
```shell
chmod u+rw {{pfad/zu/datei_oder_verzeichnis}}
```
#### Entferne die Ausführrechte (e[x]ecute) der Besitzer[g]ruppe:
```shell
chmod g-x {{pfad/zu/datei}}
```
#### Gib [a]llen Benutzern Rechte zum Lesen ([r]ead) und Ausführen (e[x]ecute) einer Datei:
```shell
chmod a+rx {{pfad/zu/datei}}
```
#### Gib anderen ([o]thers) (nicht in der Besitzer[g]ruppe) die gleichen Rechte wie der Besitzer[g]ruppe:
```shell
chmod o=g {{pfad/zu/datei}}
```
#### Entferne alle Rechte der anderen ([o]thers):
```shell
chmod o= {{pfad/zu/datei}}
```
#### Ändere Rechte rekursiv, indem der Besitzer[g]ruppe und anderen ([o]thers) die Rechte zum Schreiben ([w]rite) geben werden:
```shell
chmod -R g+w,o+w {{pfad/zu/verzeichnis}}
```
{% endraw %}