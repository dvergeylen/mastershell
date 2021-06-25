---
layout: default
title: "trans"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trans">
  <a href="/en/common/trans.html">trans</a> <a href="#trans"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Translate Shell is a command-line translator.
> More information: <https://github.com/soimort/translate-shell>.

#### Translate a word (language is detected automatically):
```shell
trans "{{word_or_sentence_to_translate}}"
```
#### Get a brief translation:
```shell
trans --brief "{{word_or_sentence_to_translate}}"
```
#### Translate a word into french:
```shell
trans :{{fr}} {{word}}
```
#### Translate a word from German to English:
```shell
trans {{de}}:{{en}} {{Schmetterling}}
```
#### Behave like a dictionary to get the meaning of a word:
```shell
trans -d {{word}}
```
{% endraw %}