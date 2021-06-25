---
layout: default
title: "cargo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo">
  <a href="/it/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti di Rust.
> Gestisce progetti Rust ed i moduli dai quali sono dipendenti (detti crate).
> Maggiori informazioni: <https://crates.io/>.

#### Cerca una crate:
```shell
cargo search {{termine_di_ricerca}}
```
#### Installa una crate:
```shell
cargo install {{nome_crate}}
```
#### Elenca crate installate:
```shell
cargo install --list
```
#### Crea un nuovo progetto Rust binario o di libreria nella directory corrente:
```shell
cargo init --{{bin|lib}}
```
#### Crea un nuovo progetto Rust binario o di libreria nella directory specificata:
```shell
cargo new {{path/a/directory}} --{{bin|lib}}
```
#### Builda il progetto Rust nella cartella corrente:
```shell
cargo build
```
#### Builda utilizzando più job (thread) paralleli:
```shell
cargo build -j {{numero_job}}
```
{% endraw %}