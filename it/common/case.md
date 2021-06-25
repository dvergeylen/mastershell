---
layout: default
title: "case"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="case">
  <a href="/it/common/case.html">case</a> <a href="#case"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui branch diversi in base al valore di un'espressione.
> Maggiori informazioni: <https://manned.org/case>.

#### Esegui il match di una variabile su diverse stringhe per decidere che comando eseguire:
```shell
case {{$metrica}} in {{parole}}) {{wc -w README}}; ;; {{linee}}) {{wc -l README}}; ;; esac
```
#### Combina pattern con |, utilizzando * come pattern di fallback:
```shell
case {{$metrica}} in {{[pP]|parole}}) {{wc -w README}}; ;; {{[lL]|linee}}) {{wc -l README}}; ;; *) {{echo "cosa?"}}; ;; esac
```
{% endraw %}