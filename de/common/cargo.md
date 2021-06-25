---
layout: default
title: "cargo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo">
  <a href="/de/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust Paketmanager.
> Verwalte Rust-Projekte und deren Abhängigkeiten (crates).
> Weitere Informationen: <https://crates.io/>.

#### Suche nach Abhängigkeiten (crates):
```shell
cargo search {{suche}}
```
#### Installiere eine Abhängigkeit (crate):
```shell
cargo install {{abhängigkeit}}
```
#### Liste alle installierten Abhängigkeiten (crates) auf:
```shell
cargo install --list
```
#### Erzeuge ein neues Rust-Projekt als Anwendung oder Bibliothek im aktuellen Verzeichnis:
```shell
cargo init --{{bin|lib}}
```
#### Erzeuge ein neues Rust-Projekt als Anwendung oder Bibliothek im angegebenen Verzeichnis:
```shell
cargo new {{pfad/zu/verzeichnis}} --{{bin|lib}}
```
#### Erstelle (bzw. kompiliere) ein Rust-Projekt im aktuellen Verzeichnis:
```shell
cargo build
```
#### Erstelle (bzw. kompiliere) ein Rust-Projekt mit einer bestimmten Anzahl an Threads (standardmäßig die Anzahl der CPU-Kerne):
```shell
cargo build -j {{thread_anzahl}}
```
{% endraw %}