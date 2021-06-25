---
layout: default
title: "bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bundle">
  <a href="/it/common/bundle.html">bundle</a> <a href="#bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di dipendenze per il linguaggio di programmazione Ruby.
> Maggiori informazioni: <https://bundler.io/man/bundle.1.html>.

#### Installa tutte le gem definite nel gemfile della directory corrente:
```shell
bundle install
```
#### Aggiorna tutte le gem secondo le regole definite nel gemfile e genera un `gemfile.lock`:
```shell
bundle update
```
#### Aggiorna una specifica gem definita nel gemfile:
```shell
bundle update --source {{nome_gem}}
```
#### Crea un scheletro per una nuova gem:
```shell
bundle gem {{nome_gem}}
```
{% endraw %}