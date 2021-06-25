---
layout: default
title: "command"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="command">
  <a href="/it/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command forza la shell ad eseguire programmi ignorando qualsiasi funzione, builtin e alias con lo stesso nome.
> Maggiori informazioni: <https://manned.org/command>.

#### Esegui il comando `ls` letteralmente, anche se esiste un alias `ls`:
```shell
command {{ls}}
```
{% endraw %}