---
layout: default
title: "alex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alex">
  <a href="/it/common/alex.html">alex</a> <a href="#alex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno strumento per individuare frasi scritte in modo insensibile o sconsiderato.
> Aiuta a trovare termini che favoriscono un certo genere, legati alla razza, religiosamente inappropriati, o simili termini non equi in un testo.
> Maggiori informazioni: <https://github.com/get-alex/alex>.

#### Analizza testo da standard input:
```shell
echo {{Frase da analizzare}} | alex --stdin
```
#### Analizza tutti i file nella directory corrente:
```shell
alex
```
#### Analizza uno specifico file:
```shell
alex {{file.md}}
```
#### Analizza tutti i file Markdown eccetto `esempio.md`:
```shell
alex *.md !{{esempio.md}}
```
{% endraw %}