---
layout: default
title: "minisign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minisign">
  <a href="/de/common/minisign.html">minisign</a> <a href="#minisign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein denkbar einfaches Werkzeug um Dateien zu signieren und Signaturen zu verifizieren.
> Weitere Informationen: <https://jedisct1.github.io/minisign/>.

#### Generiere ein neues Schlüsselpaar im Standardpfad:
```shell
minisign -G
```
#### Signiere eine Datei:
```shell
minisign -Sm {{pfad/zu/datei}}
```
#### Signiere eine Datei und füge dabei einen vertrauenswürdigen (signierten) und einen nicht vertrauenswürdigen (unsignierten) Kommentar in der Signatur an:
```shell
minisign -Sm {{pfad/zu/datei}} -c "{{Nicht vertrauenswürdiger Kommentar}}" -t "{{Vertrauenswürdiger Kommentar}}"
```
#### Verifiziere eine Datei und die vertrauenswürdigen Kommentare in ihrer Signatur gegen die angegebene Datei mit dem öffentlichen Schlüssel:
```shell
minisign -Vm {{pfad/zu/datei}} -p {{pfad/zu/öffentlicher_schlüssel.pub}}
```
#### Verifiziere eine Datei und die vertrauenswürdigen Kommentare in ihrer Signatur gegen den angegebenen, in Base64 codierten öffentlichen Schlüssel:
```shell
minisign -Vm {{pfad/zu/datei}} -P "{{öffentlicher_schlüssel_base64}}"
```
{% endraw %}