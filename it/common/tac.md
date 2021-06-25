---
layout: default
title: "tac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tac">
  <a href="/it/common/tac.html">tac</a> <a href="#tac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa e concatena file al contrario.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/tac>.

#### Stampa il contenuto di *file1* al contrario su standard output:
```shell
tac {{file1}}
```
#### Concatena multipli file al contrario in un nuovo file:
```shell
tac {{file1}} {{file2}} > {{nuovo_file}}
```
{% endraw %}