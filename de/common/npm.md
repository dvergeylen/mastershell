---
layout: default
title: "npm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="npm">
  <a href="/de/common/npm.html">npm</a> <a href="#npm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Kommandozeilenwerkzeug für die Verwaltung von JavaScript und Node.js Paketen (Packages).
> Weitere Informationen: <https://www.npmjs.com>.

#### Erstelle eine `package.json` Datei interaktiv:
```shell
npm init
```
#### Installiere alle in der `package.json` Datei gelisteten Abhängigkeiten:
```shell
npm install
```
#### Installiere eine spezifische Version eines Packages und füge es automatisch der `package.json` Datei hinzu:
```shell
npm install {{package_name}}@{{version}}
```
#### Installiere ein Package und füge es als Entwicklungs-Abhängigkeit der `package.json` Datei hinzu:
```shell
npm install {{package_name}} --save-dev
```
#### Installiere ein Package global:
```shell
npm install --global {{package_name}}
```
#### Deinstalliere ein Package und entferne es automatisch aus der `package.json` Datei:
```shell
npm uninstall {{package_name}}
```
#### Gib eine Liste aller lokal installierten Packages aus:
```shell
npm list
```
#### Gib eine Liste aller global installierten Packages aus:
```shell
npm list --global --depth={{0}}
```
{% endraw %}