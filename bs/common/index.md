---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#chsh">chsh</a>
* <a href="#false">false</a>
* <a href="#logname">logname</a>
* <a href="#mkfifo">mkfifo</a>
* <a href="#time">time</a>
* <a href="#tty">tty</a>
* <a href="#unalias">unalias</a>
* <a href="#unclutter">unclutter</a>
* <a href="#view">view</a>
* <a href="#zless">zless</a>

{% raw %}
<h2 id="chsh">
  <a href="/bs/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Promijeni korisnički login shell.
> Više informacija: <https://manned.org/chsh>.

#### Promijeni shell:
```shell
chsh -s {{putanja/do/shell_binarni}} {{korisničkoime}}
```
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/bs/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vrati izlazni kod od 1.
> Više informacija: <https://www.gnu.org/software/coreutils/false>.

#### Vrati izlazni kod od 1:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="logname">
  <a href="/bs/common/logname.html">logname</a> <a href="#logname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prikazuje ime prijevljenog korisnika.
> Više informacija: <https://www.gnu.org/software/coreutils/logname>.

#### Prikaži ime trenutno prijavljenog korisnika:
```shell
logname
```
{% endraw %}{% raw %}
<h2 id="mkfifo">
  <a href="/bs/common/mkfifo.html">mkfifo</a> <a href="#mkfifo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pravi FIFOs (imenovane cijevi).
> Više informacija: <https://www.gnu.org/software/coreutils/mkfifo>.

#### Napravi imenovanu cijev na zadatoj putanji:
```shell
mkfifo {{putanja/do/cijev}}
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/bs/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vidi koliko dugo traje komanda.

#### Vrijeme `ls`:
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="tty">
  <a href="/bs/common/tty.html">tty</a> <a href="#tty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vraća ime terminala.
> Više informacija: <https://www.gnu.org/software/coreutils/tty>.

#### Ispiši ime fajla ovog terminala:
```shell
tty
```
{% endraw %}{% raw %}
<h2 id="unalias">
  <a href="/bs/common/unalias.html">unalias</a> <a href="#unalias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ukloni alijase.

#### Ukloni alijas:
```shell
unalias {{ime_alijasa}}
```
#### Ukloni sve alijase:
```shell
unalias -a
```
{% endraw %}{% raw %}
<h2 id="unclutter">
  <a href="/bs/common/unclutter.html">unclutter</a> <a href="#unclutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Skriva kursor miša.

#### Sakrij kursor miša nakon 3 sekunde:
```shell
unclutter -idle {{3}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/bs/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read-only verzija `vim`.
> Ovo je ekvivalent za `vim -R`.

#### Otvori datoteku:
```shell
view {{datoteka}}
```
{% endraw %}{% raw %}
<h2 id="zless">
  <a href="/bs/common/zless.html">zless</a> <a href="#zless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pregledaj kompresovane datoteke.

#### Prelistaj kroz kompresovanu arhivu sa `less`:
```shell
zless {{fajl.txt.gz}}
```
{% endraw %}