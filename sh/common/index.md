---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#head">head</a>
* <a href="#sh">sh</a>
* <a href="#sha1sum">sha1sum</a>
* <a href="#sha224sum">sha224sum</a>
* <a href="#sha256sum">sha256sum</a>
* <a href="#sha384sum">sha384sum</a>
* <a href="#sha512sum">sha512sum</a>
* <a href="#tail">tail</a>
* <a href="#tldr">tldr</a>
* <a href="#tldr-lint">tldr-lint</a>

{% raw %}
<h2 id="head">
  <a href="/sh/common/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prikazuje prvi deo datoteka.
> Više informacija: <https://www.gnu.org/software/coreutils/head>.

#### Prikaži prvih nekoliko linija datoteke:
```shell
head -n {{broj_linija}} {{naziv_datoteke}}
```
#### Prikaži prvih nekoliko bajtova datoteke:
```shell
head -c {{veličina_u_bajtovima}} {{naziv_datoteke}}
```
#### Prikaži sve osim nekoliko poslednjih linija datoteke:
```shell
head -n -{{broj_linija}} {{naziv_datoteke}}
```
#### Prikaži sve osim nekoliko poslednjih bajtova datoteke:
```shell
head -c -{{veličina_u_bajtovima}} {{naziv_datoteke}}
```
{% endraw %}{% raw %}
<h2 id="sh">
  <a href="/sh/common/sh.html">sh</a> <a href="#sh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne ljuska.
> Standardni interpreter komandnog jezika.
> Više informacija: <https://manned.org/sh>.

#### Pokreni interaktivnu ljusku:
```shell
sh
```
#### Izvrši komandu:
```shell
sh -c {{komanda}}
```
#### Pokreni komande iz datoteke:
```shell
sh {{datoteka.sh}}
```
#### Pokreni komande iz stdin-a:
```shell
sh -s
```
{% endraw %}{% raw %}
<h2 id="sha1sum">
  <a href="/sh/common/sha1sum.html">sha1sum</a> <a href="#sha1sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA1 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/sha1sum>.

#### Izračunaj SHA1 kontrolni broj za datoteku:
```shell
sha1sum {{datoteka1}}
```
#### Izračunaj SHA1 kontrolne brojeve za više datoteka:
```shell
sha1sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA1 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha1sum -c {{datoteka.sha1}}
```
{% endraw %}{% raw %}
<h2 id="sha224sum">
  <a href="/sh/common/sha224sum.html">sha224sum</a> <a href="#sha224sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA224 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA224 kontrolni broj za datoteku:
```shell
sha224sum {{datoteka1}}
```
#### Izračunaj SHA224 kontrolne brojeve za više datoteka:
```shell
sha224sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA224 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha224sum -c {{datoteka.sha224}}
```
{% endraw %}{% raw %}
<h2 id="sha256sum">
  <a href="/sh/common/sha256sum.html">sha256sum</a> <a href="#sha256sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA256 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA256 kontrolni broj za datoteku:
```shell
sha256sum {{datoteka1}}
```
#### Izračunaj SHA256 kontrolne brojeve za više datoteka:
```shell
sha256sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA256 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha256sum -c {{datoteka.sha256}}
```
{% endraw %}{% raw %}
<h2 id="sha384sum">
  <a href="/sh/common/sha384sum.html">sha384sum</a> <a href="#sha384sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA384 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA384 kontrolni broj za datoteku:
```shell
sha384sum {{datoteka1}}
```
#### Izračunaj SHA384 kontrolne brojeve za više datoteka:
```shell
sha384sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA384 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha384sum -c {{datoteka.sha384}}
```
{% endraw %}{% raw %}
<h2 id="sha512sum">
  <a href="/sh/common/sha512sum.html">sha512sum</a> <a href="#sha512sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA512 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA512 kontrolni broj za datoteku:
```shell
sha512sum {{datoteka1}}
```
#### Izračunaj SHA512 kontrolne brojeve za više datoteka:
```shell
sha512sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA512 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha512sum -c {{datoteka.sha512}}
```
{% endraw %}{% raw %}
<h2 id="tail">
  <a href="/sh/common/tail.html">tail</a> <a href="#tail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prikazuje krajnji deo datoteke.
> Više informacija: <https://www.gnu.org/software/coreutils/tail>.

#### Prikaži poslednjih 'broj' linija u datoteci:
```shell
tail -n {{broj}} {{datoteka}}
```
#### Prikaži celu datoteku od linije 'broj':
```shell
tail -n +{{broj}} {{datoteka}}
```
#### Prikaži poslednjih 'broj' bajtova u datoteci:
```shell
tail -c {{broj}} {{datoteka}}
```
#### Čitaj datoteku sve do `Ctrl + C`:
```shell
tail -f {{datoteka}}
```
#### Čitaj datoteku sve do `Ctrl + C`, čak i kad je datoteka rotirana:
```shell
tail -F {{datoteka}}
```
{% endraw %}{% raw %}
<h2 id="tldr-lint">
  <a href="/sh/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lintuje i formatira tldr stranice.
> Više informacija: <https://github.com/tldr-pages/tldr-lint>.

#### Lintuj sve stranice:
```shell
tldr-lint {{direktorijum_stranica}}
```
#### Formatiraj određenu stranicu u stdout:
```shell
tldr-lint --format {{stranica.md}}
```
#### Formatiraj sve stranice na njihovom mestu:
```shell
tldr-lint --format --in-place {{direktorijum_stranica}}
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/sh/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pojednostavljene man stranice.
> Više informacija: <https://tldr.sh>.

#### Prikaži tipičnu upotrebu komande (pomoć: ovako ste stigli ovde!):
```shell
tldr {{komanda}}
```
#### Prikaži tar tldr stranicu za Linux:
```shell
tldr -p {{linux}} {{tar}}
```
#### Prikaži pomoć za Git potkomandu:
```shell
tldr {{git-checkout}}
```
{% endraw %}