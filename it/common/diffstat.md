---
layout: default
title: "diffstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diffstat">
  <a href="/it/common/diffstat.html">diffstat</a> <a href="#diffstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea un istogramma dall'output del comando `diff`.
> Maggiori informazioni: <https://manned.org/diffstat>.

#### Mostra i cambiamenti in un istogramma:
```shell
diff {{file1}} {{file2}} | diffstat
```
#### Mostra inserimenti, cancellazioni e modifiche come una tabella:
```shell
diff {{file1}} {{file2}} | diffstat -t
```
{% endraw %}