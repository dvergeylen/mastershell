---
layout: default
title: "csslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csslint">
  <a href="/it/common/csslint.html">csslint</a> <a href="#csslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un linter per codice CSS.
> Maggiori informazioni: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

#### Esegui il linting di un singolo file CSS:
```shell
csslint {{file.css}}
```
#### Esegui il linting di file CSS multipli:
```shell
csslint {{file1.css}} {{file2.css}} {{file3.css}}
```
#### Elenca tutte le possibili regole di stile:
```shell
csslint --list-rules
```
#### Specifica certe regole come errori (che risulteranno in un codice d'uscita diverso da zero):
```shell
csslint --errors={{errors,universal-selector,imports}} {{file.css}}
```
#### Specifica certe regole come warning:
```shell
csslint --warnings={{box-sizing,selector-max,floats}} {{file.css}}
```
#### Specifica certe regole da essere completamente ignorate:
```shell
csslint --ignore={{ids,rules-count,shorthand}} {{file.css}}
```
{% endraw %}