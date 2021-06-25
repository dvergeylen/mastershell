---
layout: default
title: "espeak"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="espeak">
  <a href="/it/common/espeak.html">espeak</a> <a href="#espeak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Usa la sintesi vocale per parlare tramite il dispositivo audio di output predefinito.
> Maggiori informazioni: <http://espeak.sourceforge.net>.

#### Pronuncia una frase ad alta voce:
```shell
espeak "Mi piace andare in bici."
```
#### Pronuncia il contenuto di un file ad alta voce:
```shell
espeak -f {{nome_file}}
```
#### Salva l'output su un file audio WAV, invece che parlare direttamente:
```shell
espeak -w {{nome_file.wav}} "È GNU più Linux."
```
#### Usa una voce differente:
```shell
espeak -v {{voce}}
```
{% endraw %}