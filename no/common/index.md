---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#arch">arch</a>
* <a href="#chsh">chsh</a>
* <a href="#false">false</a>
* <a href="#logname">logname</a>
* <a href="#time">time</a>
* <a href="#tty">tty</a>
* <a href="#unalias">unalias</a>
* <a href="#unclutter">unclutter</a>
* <a href="#view">view</a>
* <a href="#zless">zless</a>

{% raw %}
<h2 id="arch">
  <a href="/no/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vis navnet på systemarkitekturen.
> Se også `uname`.
> Mer informasjon: <https://www.gnu.org/software/coreutils/arch>.

#### Vis systemets arkitektur:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="chsh">
  <a href="/no/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Forandre brukerens påloggings shell.
> Mer informasjon: <https://manned.org/chsh>.

#### Forandre shell:
```shell
chsh -s {{sti/til/shell_binær}} {{brukernavn}}
```
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/no/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Returner en utgangskode på 1.
> Mer informasjon: <https://www.gnu.org/software/coreutils/false>.

#### Returner en utgangskode på 1:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="logname">
  <a href="/no/common/logname.html">logname</a> <a href="#logname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Viser brukerens login navn.
> Mer informasjon: <https://www.gnu.org/software/coreutils/logname>.

#### Vis brukerens nåværende innloggings navn:
```shell
logname
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/no/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> See hvor lang en kommand tar.

#### Tid "ls":
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="tty">
  <a href="/no/common/tty.html">tty</a> <a href="#tty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Returner terminal navn.
> Mer informasjon: <https://www.gnu.org/software/coreutils/tty>.

#### Print fil navnet fra denne terminalen:
```shell
tty
```
{% endraw %}{% raw %}
<h2 id="unalias">
  <a href="/no/common/unalias.html">unalias</a> <a href="#unalias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fjern aliaser.

#### Fjern et alias:
```shell
unalias {{alias_navn}}
```
#### Fjern alle aliaser:
```shell
unalias -a
```
{% endraw %}{% raw %}
<h2 id="unclutter">
  <a href="/no/common/unclutter.html">unclutter</a> <a href="#unclutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gjemmer musepekeren.

#### Gjem musepekeren etter 3 sekunder:
```shell
unclutter -idle {{3}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/no/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> En skrivebeskytter vesjon av `vim`.
> Dette tilsvarer `vim -R`.

#### Åpne en fil:
```shell
view {{fil}}
```
{% endraw %}{% raw %}
<h2 id="zless">
  <a href="/no/common/zless.html">zless</a> <a href="#zless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vis komprimerte filer.

#### Bla gjennom et komprimert arkiv med `less`:
```shell
zless {{fil.txt.gz}}
```
{% endraw %}