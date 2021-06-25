---
layout: default
title: "csslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csslint">
  <a href="/pl/common/csslint.html">csslint</a> <a href="#csslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linter dla kodu CSS.
> Więcej informacji: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

#### Lintowanie pojedynczego pliku CSS:
```shell
csslint {{plik.css}}
```
#### Lintowanie wiele plików CSS:
```shell
csslint {{plik1.css}} {{plik2.css}} {{plik3.css}}
```
#### Wymień wszystkie możliwe reguły stylu:
```shell
csslint --list-rules
```
#### Określ pewne reguły jako błędy (które powodują niezerowy kod wyjścia):
```shell
csslint --errors={{bledy,universal-selector,imports}} {{plik.css}}
```
#### Określ pewne reguły jako ostrzeżenia:
```shell
csslint --warnings={{box-sizing,selector-max,floats}} {{plik.css}}
```
#### Określ pewne reguły, które będą całkowicie ignorowane:
```shell
csslint --ignore={{ids,rules-count,shorthand}} {{plik.css}}
```
{% endraw %}