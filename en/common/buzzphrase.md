---
layout: default
title: "buzzphrase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="buzzphrase">
  <a href="/en/common/buzzphrase.html">buzzphrase</a> <a href="#buzzphrase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Node.js command-line tool to output a random buzzphrase.
> More information: <https://github.com/atomantic/buzzphrase>.

#### Generate a string of three random phrases containing an adjective, a past tense verb and a plural noun:
```shell
buzzphrase
```
#### Output a phrase formatted as [i]mperative verb + past tense [v]erb + [a]djective + plural [N]oun:
```shell
buzzphrase {{'{i} {v} {a} {N}'}}
```
#### Output 4 phrases formatted as present participle [V]erb + [a]djective + singular [n]oun + [f]inal:
```shell
buzzphrase {{4 '{V} {a} {n} {f}'}}
```
{% endraw %}