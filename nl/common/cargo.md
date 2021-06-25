---
layout: default
title: "cargo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo">
  <a href="/nl/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust pakketbeheerder.
> Beheer Rust projecten en hun afhankelijkheden (crates).
> Meer informatie: <https://crates.io/>.

#### Zoek naar crates:
```shell
cargo search {{zoekopdracht}}
```
#### Installeer een crate:
```shell
cargo install {{crate-naam}}
```
#### Geef een lijst van geïnstalleerde crates:
```shell
cargo install --list
```
#### Maak een nieuwe Rust-binary (bin) of -bibliotheek (lib) in de huidige map:
```shell
cargo init --{{bin|lib}}
```
#### Maak een nieuwe Rust-binary (bin) of -bibliotheek (lib) in de gegeven map:
```shell
cargo new {{pad/naar/map}} --{{bin|lib}}
```
#### Bouw het Rust-project in de huidige map:
```shell
cargo build
```
#### Bouw met een gegeven aantal taken. (Standaard is het aantal CPU-kernen):
```shell
cargo build -j {{taken}}
```
{% endraw %}