---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#arch">arch</a>
* <a href="#chsh">chsh</a>
* <a href="#exit">exit</a>
* <a href="#false">false</a>
* <a href="#go-bug">go bug</a>
* <a href="#go-fix">go fix</a>
* <a href="#hostid">hostid</a>
* <a href="#is-up">is-up</a>
* <a href="#kotlin">kotlin</a>
* <a href="#logname">logname</a>
* <a href="#nohup">nohup</a>
* <a href="#npm-why">npm-why</a>
* <a href="#rev">rev</a>
* <a href="#sleep">sleep</a>
* <a href="#source">source</a>
* <a href="#time">time</a>
* <a href="#true">true</a>
* <a href="#tty">tty</a>
* <a href="#unalias">unalias</a>
* <a href="#unclutter">unclutter</a>
* <a href="#users">users</a>
* <a href="#view">view</a>
* <a href="#vimtutor">vimtutor</a>
* <a href="#visudo">visudo</a>
* <a href="#yarn-why">yarn-why</a>
* <a href="#zbarimg">zbarimg</a>
* <a href="#zless">zless</a>

{% raw %}
<h2 id="arch">
  <a href="/sv/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visa namnet på systemarkitekturen:
> Se även `uname`.
> Mer information: <https://www.gnu.org/software/coreutils/arch>.

#### Visa systemarkitekturen:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="chsh">
  <a href="/sv/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ändra användarens inloggnings-shell.
> Mer information: <https://manned.org/chsh>.

#### Ändra shell:
```shell
chsh -s {{väg/till/shell_binär}} {{användarnamn}}
```
{% endraw %}{% raw %}
<h2 id="exit">
  <a href="/sv/common/exit.html">exit</a> <a href="#exit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Avsluta shell.
> Mer information: <https://manned.org/exit>.

#### Avsluta shell med utgångskoden från det senast utförda kommandot:
```shell
exit
```
#### Avsluta shell med den angivna utgångskoden:
```shell
exit {{utgångskoden}}
```
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/sv/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Returnerar en utgångskod på 1.
> Mer information: <https://www.gnu.org/software/coreutils/false>.

#### Returnera en utgångskod på 1:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="go-bug">
  <a href="/sv/common/go-bug.html">go bug</a> <a href="#go-bug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rapportera en bugg.
> Mer information: <https://golang.org/cmd/go/#hdr-Start_a_bug_report>.

#### Öppna en webbsida för att starta en felrapport:
```shell
go bug
```
{% endraw %}{% raw %}
<h2 id="go-fix">
  <a href="/sv/common/go-fix.html">go fix</a> <a href="#go-fix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uppdatera paketen för att använda nya API.
> Mer information: <https://golang.org/cmd/go/#hdr-Update_packages_to_use_new_APIs>.

#### Uppdatera paketen för att använda nya API:
```shell
go fix {{paketen}}
```
{% endraw %}{% raw %}
<h2 id="hostid">
  <a href="/sv/common/hostid.html">hostid</a> <a href="#hostid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Skriver ut den numeriska identifieraren för den aktuella värden (inte nödvändigtvis IP-adressen).
> Mer information: <https://www.gnu.org/software/coreutils/hostid>.

#### Visa den numeriska identifieraren för den aktuella värden i hexadecimal:
```shell
hostid
```
{% endraw %}{% raw %}
<h2 id="is-up">
  <a href="/sv/common/is-up.html">is-up</a> <a href="#is-up"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kontrollera om en webbplats är uppe eller nere.
> Mer information: <https://github.com/sindresorhus/is-up-cli>.

#### Kontrollera statusen för den angivna webbplatsen:
```shell
is-up {{exempel.com}}
```
{% endraw %}{% raw %}
<h2 id="kotlin">
  <a href="/sv/common/kotlin.html">kotlin</a> <a href="#kotlin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kotlin Programstartare.
> Mer information: <https://kotlinlang.org>.

#### Kör en jar fil:
```shell
kotlin {{filnamn.jar}}
```
#### Visa Kotlin och JVM version:
```shell
kotlin -version
```
{% endraw %}{% raw %}
<h2 id="logname">
  <a href="/sv/common/logname.html">logname</a> <a href="#logname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visar användarens inloggningsnamn.
> Mer information: <https://www.gnu.org/software/coreutils/logname>.

#### Visa den för tillfället inloggades användarnamn:
```shell
logname
```
{% endraw %}{% raw %}
<h2 id="nohup">
  <a href="/sv/common/nohup.html">nohup</a> <a href="#nohup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tillåter en process att leva när terminalen dödas.
> Mer information: <https://www.gnu.org/software/coreutils/nohup>.

#### Kör process som kan leva bortom terminalen:
```shell
nohup {{kommandoalternativ}}
```
{% endraw %}{% raw %}
<h2 id="npm-why">
  <a href="/sv/common/npm-why.html">npm-why</a> <a href="#npm-why"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Identifierar varför ett npm-paket är installerat.
> Mer information: <https://www.npmjs.com/package/npm-why>.

#### Visa varför ett npm-paket är installerat:
```shell
npm-why {{paket_namn}}
```
{% endraw %}{% raw %}
<h2 id="rev">
  <a href="/sv/common/rev.html">rev</a> <a href="#rev"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Omvänd en textrad.

#### Omvänd textraden "hello":
```shell
echo "hello" | rev
```
#### Omvänd hel fil och skriv till stdout:
```shell
rev {{fil}}
```
{% endraw %}{% raw %}
<h2 id="sleep">
  <a href="/sv/common/sleep.html">sleep</a> <a href="#sleep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fördröjning under bestämd tid.
> Mer information: <https://www.gnu.org/software/coreutils/sleep>.

#### Fördröj i sekunder:
```shell
sleep {{sekunder}}
```
#### Fördröj i minuter:
```shell
sleep {{minuter}}m
```
#### Fördröj i timmar:
```shell
sleep {{timmar}}h
```
{% endraw %}{% raw %}
<h2 id="source">
  <a href="/sv/common/source.html">source</a> <a href="#source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kör kommandon från en fil i det aktuella skalet.

#### Utvärdera innehållet i en viss fil:
```shell
source {{väg/till/fil}}
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/sv/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Se hur lång tid ett kommando tar.

#### Tidtagning "ls":
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="true">
  <a href="/sv/common/true.html">true</a> <a href="#true"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Returnerar en lyckad utgångsstatuskod på 0.
> Använd detta med || operatör för att göra att ett kommando alltid stänger med 0.
> Mer information: <https://www.gnu.org/software/coreutils/true>.

#### Returnera en lyckad utgångskod:
```shell
true
```
{% endraw %}{% raw %}
<h2 id="tty">
  <a href="/sv/common/tty.html">tty</a> <a href="#tty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Returnerar terminalnamn.
> Mer information: <https://www.gnu.org/software/coreutils/tty>.

#### Skriv ut filnamnet på denna terminal:
```shell
tty
```
{% endraw %}{% raw %}
<h2 id="unalias">
  <a href="/sv/common/unalias.html">unalias</a> <a href="#unalias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ta bort alias.

#### Ta bort en alias:
```shell
unalias {{alias_namn}}
```
#### Ta bort alla alias:
```shell
unalias -a
```
{% endraw %}{% raw %}
<h2 id="unclutter">
  <a href="/sv/common/unclutter.html">unclutter</a> <a href="#unclutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Döljer muspekaren.

#### Dölj muspekarn efter 3 sekunder:
```shell
unclutter -idle {{3}}
```
{% endraw %}{% raw %}
<h2 id="users">
  <a href="/sv/common/users.html">users</a> <a href="#users"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visa en lista över inloggade användare.
> Mer information: <https://www.gnu.org/software/coreutils/users>.

#### Visa en lista över inloggade användare:
```shell
users
```
#### Visa en lista över inloggade användare enligt en specifik fil:
```shell
users {{/var/log/wmtp}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/sv/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> En skrivskyddad version av `vim`.
> Detta är lika med `vim -R`.

#### Öppna en fil:
```shell
view {{fil}}
```
{% endraw %}{% raw %}
<h2 id="vimtutor">
  <a href="/sv/common/vimtutor.html">vimtutor</a> <a href="#vimtutor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vim-handledare, lär ut de grundläggande vim-kommandona.

#### Starta vim-handledaren med det angivna språket (en, fr, de, ...):
```shell
vimtutor {{språk}}
```
#### Gå ur handledaren:
```shell
<Esc> :q <Enter>
```
{% endraw %}{% raw %}
<h2 id="visudo">
  <a href="/sv/common/visudo.html">visudo</a> <a href="#visudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Redigera sudoers-filen på säkert sätt.

#### Redigera sudoers-filen:
```shell
sudo visudo
```
#### Sök fel i sudoers-filen:
```shell
sudo visudo -c
```
{% endraw %}{% raw %}
<h2 id="yarn-why">
  <a href="/sv/common/yarn-why.html">yarn-why</a> <a href="#yarn-why"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Identifierar varför ett Yarn paket har installerats.
> Mer information: <https://www.npmjs.com/package/yarn-why>.

#### Visa varför ett Yarn paket är installerat:
```shell
yarn-why {{paket_namn}}
```
{% endraw %}{% raw %}
<h2 id="zbarimg">
  <a href="/sv/common/zbarimg.html">zbarimg</a> <a href="#zbarimg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Skanna och avkoda streckkoder från bildfil(er).
> Mer information: <http://zbar.sourceforge.net>.

#### Processa en bildfil:
```shell
zbarimg {{bild_fil}}
```
{% endraw %}{% raw %}
<h2 id="zless">
  <a href="/sv/common/zless.html">zless</a> <a href="#zless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visa komprimerade filer.

#### Bläddra igenom ett komprimerat arkiv med `less`:
```shell
zless {{fil.txt.gz}}
```
{% endraw %}