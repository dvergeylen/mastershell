---
layout: default
title: "cmp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmp">
  <a href="/it/common/cmp.html">cmp</a> <a href="#cmp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compara due file.
> Maggiori informazioni: <https://www.gnu.org/software/diffutils/manual/html_node/Invoking-cmp.html>.

#### Trova l'indice del primo byte e della prima riga differente tra due file:
```shell
cmp {{file1}} {{file2}}
```
#### Trova ogni coppia di byte differenti ed il relativo indice:
```shell
cmp -l {{file1}} {{file2}}
```
{% endraw %}