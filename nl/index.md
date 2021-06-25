---
layout: default
title: "NL"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#common">Common</a>
  * <a href="#7z">7z</a>
  * <a href="#adb">adb</a>
  * <a href="#arch">arch</a>
  * <a href="#autopep8">autopep8</a>
  * <a href="#base64">base64</a>
  * <a href="#bash">bash</a>
  * <a href="#cargo">cargo</a>
  * <a href="#cd">cd</a>
  * <a href="#chgrp">chgrp</a>
  * <a href="#chmod">chmod</a>
  * <a href="#chown">chown</a>
  * <a href="#chroot">chroot</a>
  * <a href="#chsh">chsh</a>
  * <a href="#false">false</a>
  * <a href="#git">git</a>
  * <a href="#inkscape">inkscape</a>
  * <a href="#logname">logname</a>
  * <a href="#magick">magick</a>
  * <a href="#source">source</a>
  * <a href="#time">time</a>
  * <a href="#tty">tty</a>
  * <a href="#unalias">unalias</a>
  * <a href="#unclutter">unclutter</a>
  * <a href="#view">view</a>
  * <a href="#visudo">visudo</a>
  * <a href="#yapf">yapf</a>
  * <a href="#yes">yes</a>
  * <a href="#zless">zless</a>

* <a href="#windows">Windows</a>
  * <a href="#cd">cd</a>
  * <a href="#dir">dir</a>
  * <a href="#find">find</a>
  * <a href="#rmdir">rmdir</a>
  * <a href="#shutdown">shutdown</a>


# Windows
{% raw %}
<h2 id="cd">
  <a href="/nl/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de naam van de huidige werkmap weer of wijzigt deze.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Ga naar een directory in dezelfde drive:
```shell
cd {{pad/naar/directory}}
```
#### Geef de naam van de huidige directory weer:
```shell
cd
```
#### Ga naar de ouder van de huidige directory:
```shell
cd ..
```
#### Ga naar een directory in een andere drive:
```shell
cd {{pad/naar/directory}} /d
```
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/nl/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de inhoud weer van een directory.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Geef de inhoud weer van de huidige map:
```shell
dir
```
#### Geef de inhoud weer van een gegeven directory:
```shell
dir {{pad/naar/directory}}
```
#### Geef de inhoud weer van de huidige directory, inclusief verborgen bestanden:
```shell
dir /A
```
#### Geef de inhoud weer van een gegeven directory, inclusief verborgen bestanden:
```shell
dir {{pad/naar/directory}} /A
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/nl/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vind een gespecificieerde string in een bestand.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Vind de lijnen dat een specifieke string bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}}
```
#### Laat lijnen zie die de string niet bevatten:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /v
```
#### Toon het aantal lijnen dat de string bevat:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /c
```
#### Laat het aantal lijnen zien samen met de lijnen:
```shell
find {{string}} {{pad/naar/bestand_of_directory}} /n
```
{% endraw %}{% raw %}
<h2 id="rmdir">
  <a href="/nl/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwijdert een directory en zijn inhoud.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/rmdir>.

#### Verwijder een lege directory:
```shell
rmdir {{pad/naar/directory}}
```
#### verwijder een directory en zen inhoud recursief:
```shell
rmdir {{pad/naar/directory}} /s
```
#### verwijder een directory en zen inhoud recursief zonder te vragen:
```shell
rmdir {{pad/naar/directory}} /s /q
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/nl/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een tool om een machine af te sluiten, her op te starten of af te melden.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/shutdown>.

#### Sluit de huidige machine af:
```shell
shutdown /s
```
#### Sluit de huidige machine af en sluit alle applicaties:
```shell
shutdown /s /f
```
#### Herstart de huidige machine:
```shell
shutdown /r /t 0
```
#### Zet de huidige machine in slaapstand:
```shell
shutdown /h
```
#### Log uit van de huidige machine:
```shell
shutdown /l
```
#### Zet een timer in aantal seconden voor het afsluiten van de huidige machine:
```shell
shutdown /s /t {{seconden}}
```
#### Breek een afsluit sequentie af vooraleer de timer was afgelopen:
```shell
shutdown /a
```
#### Sluit een machine af op afstand:
```shell
shutdown /m {{\\hostnaam}}
```
{% endraw %}# Common
{% raw %}
<h2 id="7z">
  <a href="/nl/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een bestandsarchiveerder met een hoge compressieratio.
> Meer informatie: <https://www.7-zip.org/>.

#### Archiveer een bestand of map:
```shell
7z a {{archief.7z}} {{pad/naar/bestand_of_map}}
```
#### Versleutel een bestaand archief (inclusief headers):
```shell
7z a {{versleuteld.7z}} -p{{wachtwoord}} -mhe=on {{archief.7z}}
```
#### Pak een bestaand 7z-bestand uit met de originele mappenstructuur:
```shell
7z x {{archief.7z}}
```
#### Pak een archief uit met een gebruiker-definieerd uitvoerpad:
```shell
7z x {{archief.7z}} -o{{pad/naar/uitvoer}}
```
#### Pak een archief naar stdout uit:
```shell
7z x {{archief.7z}} -so
```
#### Archiveer met een specifiek archieftype:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{archief.7z}} {{pad/naar/bestand_of_map}}
```
#### Geef een lijst van beschikbare archieftypen:
```shell
7z i
```
#### Geef een lijst met de inhoud van het archiefbestand:
```shell
7z l {{archief.7z}}
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/nl/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug-Brug: communiceer met een Android-emulator of een aangesloten Android-apparaat.
> Meer informatie: <https://developer.android.com/studio/command-line/adb>.

#### Controleer of het adb serverproces draait en start het:
```shell
adb start-server
```
#### Sluit het adb serverproces:
```shell
adb kill-server
```
#### Start een afstandshell voor de doelemulator of apparaatinstantie:
```shell
adb shell
```
#### Stuur een Android-applicatie naar de emulator/het apparaat:
```shell
adb install -r {{pad/naar/bestand.apk}}
```
#### Kopiëer een bestand/map van het doelapparaat:
```shell
adb pull {{pad/naar/extern/bestand_of_map}} {{pad/naar/lokaal/bestand_of_map}}
```
#### Kopiëer een bestand/map naar het doelapparaat:
```shell
adb push {{pad/naar/lokaal/bestand_of_map}} {{pad/naar/extern/bestand_of_map}}
```
#### Krijg een lijst met aangesloten apparaten:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/nl/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geef de naam van de systeemarchitectuur weer.
> Zie ook `uname`.
> Meer informatie: <https://www.gnu.org/software/coreutils/arch>.

#### Geef de architectuur van het systeem weer:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="autopep8">
  <a href="/nl/common/autopep8.html">autopep8</a> <a href="#autopep8"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Formatteer Python-code conform de PEP 8-stijlgids.
> Meer informatie: <https://github.com/hhatto/autopep8>.

#### Formateer een bestand naar stdout, met een ingestelde maximale toegestane regellengte:
```shell
autopep8 {{pad/naar/bestand.py}} --max-line-length {{lengte}}
```
#### Formateer een bestand, geef een diff weer met de wijzigingen:
```shell
autopep8 --diff {{pad/naar/bestand.py}}
```
#### Formatteer het bestand en sla de wijzigingen op:
```shell
autopep8 --in-place {{pad/naar/bestand.py}}
```
#### Formatteer de bestanden recursief in een map en sla deze wijzigingen op:
```shell
autopep8 --in-place --recursive {{pad/naar/map}}
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/nl/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codeer of decodeer bestand of standaardinvoer van/naar Base64 naar standaarduitvoer.
> Meer informatie: <https://www.gnu.org/software/coreutils/base64>.

#### Codeer een bestand:
```shell
base64 {{bestandsnaam}}
```
#### Decodeer een bestand:
```shell
base64 --decode {{bestandsnaam}}
```
#### Codeer stdin:
```shell
{{eencommando}} | base64
```
#### Decodeer stdin:
```shell
{{eencommando}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="bash">
  <a href="/nl/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> `sh`-ondersteunende commandoregel-interpreteerder.
> Meer informatie: <https://gnu.org/software/bash>.

#### Start interactieve shell:
```shell
bash
```
#### Voer een commando uit:
```shell
bash -c "{{commando}}"
```
#### Voer commando's van bestand uit:
```shell
bash {{bestand.sh}}
```
#### Voer commando's van bestand uit, en print alle uitgevoerde commando's naar de terminal:
```shell
bash -x {{bestand.sh}}
```
#### Voer commando's van bestand uit, en stop bij de eerste fout:
```shell
bash -e {{bestand.sh}}
```
#### Voer commando's van stdin uit:
```shell
bash -s
```
#### Print de versieinformatie van bash (gebruik `echo $BASH_VERSION` om alleen de versie te krijgen zonder licentie):
```shell
bash --version
```
{% endraw %}{% raw %}
<h2 id="cargo">
  <a href="/nl/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust pakketbeheerder.
> Beheer Rust projecten en hun afhankelijkheden (crates).
> Meer informatie: <https://crates.io/>.

#### Zoek naar crates:
```shell
cargo search {{zoekopdracht}}
```
#### Installeer een crate:
```shell
cargo install {{crate-naam}}
```
#### Geef een lijst van geïnstalleerde crates:
```shell
cargo install --list
```
#### Maak een nieuwe Rust-binary (bin) of -bibliotheek (lib) in de huidige map:
```shell
cargo init --{{bin|lib}}
```
#### Maak een nieuwe Rust-binary (bin) of -bibliotheek (lib) in de gegeven map:
```shell
cargo new {{pad/naar/map}} --{{bin|lib}}
```
#### Bouw het Rust-project in de huidige map:
```shell
cargo build
```
#### Bouw met een gegeven aantal taken. (Standaard is het aantal CPU-kernen):
```shell
cargo build -j {{taken}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/nl/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander de huidige map.
> Meer informatie: <https://man.archlinux.org/man/cd.n>.

#### Ga naar de gegeven map:
```shell
cd {{pad/naar/map}}
```
#### Ga naar de thuismap van de huidige gebruiker:
```shell
cd
```
#### Ga naar de ouder van de huidige map:
```shell
cd ..
```
#### Ga naar de vorige map:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="chgrp">
  <a href="/nl/common/chgrp.html">chgrp</a> <a href="#chgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander beheerdersgroep van bestanden en mappen.
> Meer informatie: <https://www.gnu.org/software/coreutils/chgrp>.

#### Verander beheerdergroep van een bestand of map:
```shell
chgrp {{groep}} {{pad/naar/bestand_of_map}}
```
#### Verander recursief de beheerdersgroep van een map en alle bestanden erin:
```shell
chgrp -R {{groep}} {{pad/naar/map}}
```
#### Verander beheerdersgroep van een symbolische link:
```shell
chgrp -h {{groep}} {{pad/naar/symlink}}
```
#### Verander de beheerdersgroep van een bestand/map naar de permissies van een referentiebestand:
```shell
chgrp --reference={{pad/naar/referentiebestand}} {{pad/naar/bestand_of_map}}
```
{% endraw %}{% raw %}
<h2 id="chmod">
  <a href="/nl/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander de toegangstoestemmingen van een bestand of map.
> Meer informatie: <https://www.gnu.org/software/coreutils/chmod>.

#### Geef een gebruiker ([u]ser) die het bestand beheert het recht om deze uit te voeren (e[x]ecute):
```shell
chmod u+x {{bestand}}
```
#### Geef de gebruiker ([u]ser) het recht om een bestand of map te lezen ([r]ead) en schrijven ([w]rite):
```shell
chmod u+rw {{bestand_of_map}}
```
#### Haal uitvoertoestemming (e[x]ecute) voor een bestand weg van de [g]roep:
```shell
chmod g-x {{bestand}}
```
#### Geef [a]lle gebruikers toegang om een bestand te lezen ([r]ead) en schrijven ([w]rite):
```shell
chmod a+rx {{bestand}}
```
#### Geef anderen ([o]thers) die niet in de groep van de beheerder zitten, dezelfde rechten als de [g]roep:
```shell
chmod o=g {{bestand}}
```
#### Haal alle rechten van de anderen ([o]thers) weg:
```shell
chmod o= {{bestand}}
```
#### Verander de toestemmingen recursief, waarbij de [g]roep en anderen ([o]thers) de mogelijkheid tot schrijven ([w]rite) krijgen:
```shell
chmod -R g+w,o+w {{map}}
```
{% endraw %}{% raw %}
<h2 id="chown">
  <a href="/nl/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander gebruiker- en groepsbeheer van bestanden en mappen.
> Meer informatie: <https://www.gnu.org/software/coreutils/chown>.

#### Verander gebruikkersbeheerder van een bestand/map:
```shell
chown {{gebruiker}} {{pad/naar/bestand_of_map}}
```
#### Verander de gebruikersbeheerder en -groep van een bestand of map:
```shell
chown {{gebruiker}}:{{groep}} {{pad/naar/bestand_of_map}}
```
#### Verander recursief de beheerder van een map en alle inhoud:
```shell
chown -R {{gebruiker}} {{pad/naar/bestand_of_map}}
```
#### Verander de gebruiker van een symbolische link:
```shell
chown -h {{gebruiker}} {{pad/naar/symlink}}
```
#### Verander de beheerder van een bestand of map naar dezelfde als een referentiebestand:
```shell
chown --reference={{pad/naar/referentiebestand}} {{pad/naar/bestand_of_map}}
```
{% endraw %}{% raw %}
<h2 id="chroot">
  <a href="/nl/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Voer commando of interactieve shell uit met een speciale hoofdmap.
> Meer informatie: <https://www.gnu.org/software/coreutils/chroot>.

#### Voer commando uit met gegeven hoofdmap:
```shell
chroot {{pad/naar/nieuwe/hoofdmap}} {{commando}}
```
#### Specificeer gebruiker en groep (ID of naam) om te gebruiken:
```shell
chroot --userspec={{gebruiker:groep}}
```
{% endraw %}{% raw %}
<h2 id="chsh">
  <a href="/nl/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wijzig de login-shell van de gebruiker.
> Meer informatie: <https://manned.org/chsh>.

#### Wijzig shell:
```shell
chsh -s {{pad/naar/shell_binary}} {{gebruikersnaam}}
```
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/nl/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft een afsluitcode van 1 terug.
> Meer informatie: <https://www.gnu.org/software/coreutils/false>.

#### Geeft een afsluitcode van 1 terug:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="git">
  <a href="/nl/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gedistribueerd versiebeheersysteem.
> Meer informatie: <https://git-scm.com/>.

#### Controleer de Git versie:
```shell
git --version
```
#### Toon algemene hulp:
```shell
git --help
```
#### Toon hulp bij een Git-subcommando (zoals `commit`, `log`, enz.):
```shell
git help {{subcommando}}
```
#### Voer een Git-subcommando uit:
```shell
git {{subcommando}}
```
#### Voer een Git-subcommando uit op een aangepast repository-rootpad:
```shell
git -C {{pad/naar/repo}} {{subcommando}}
```
#### Voer een Git-subcommando met een gegeven configuratieset:
```shell
git -c '{{config.sleutel}}={{waarde}}' {{subcommando}}
```
{% endraw %}{% raw %}
<h2 id="inkscape">
  <a href="/nl/common/inkscape.html">inkscape</a> <a href="#inkscape"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een SVG (Scalable Vector Graphics) bewerkingsprogramma.
> Voor Inkscape versies tot en met 0.92.x, gebruik -e in plaats van -o.
> Meer informatie: <https://inkscape.org>.

#### Open een SVG-bestand in de Inkscape GUI:
```shell
inkscape {{bestandsnaam.svg}}
```
#### Exporteer een SVG-bestand in een bitmap met het standaardformaat (PNG) en de standaardresolutie (96 DPI):
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}}
```
#### Exporteer een SVG-bestand in een bitmap van 600x400 pixels (vervorming van de aspectverhouding mogelijk):
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}} -w {{600}} -h {{400}}
```
#### Exporteer de tekening (selectiekader van alle objecten) van een SVG-bestand in een bitmap:
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}} -D
```
#### Exporteer een enkel object, gezien zijn ID, in een bitmap:
```shell
inkscape {{bestandsnaam.svg}} -i {{id}} -o {{object.png}}
```
#### Exporteer een SVG-document naar PDF, converteer alle teksten naar paden:
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.pdf}} --export-text-to-path
```
#### Dupliceer het object met id="pad123", roteer het duplicaat 90 graden, sla het bestand op, en sluit Inkscape af:
```shell
inkscape {{bestandsnaam.svg}} --select=path123 --verb="{{EditDuplicate;ObjectRotate90;FileSave;FileQuit}}"
```
{% endraw %}{% raw %}
<h2 id="logname">
  <a href="/nl/common/logname.html">logname</a> <a href="#logname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Toont de inlognaam van de gebruiker.
> Meer informatie: <https://www.gnu.org/software/coreutils/logname>.

#### Geef de momenteel aangemelde gebruikersnaam weer:
```shell
logname
```
{% endraw %}{% raw %}
<h2 id="magick">
  <a href="/nl/common/magick.html">magick</a> <a href="#magick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creër, bewerk, vorm, of converteer bitmapafbeeldingen.
> ImageMagick versie 7+. Bekijk `convert` versies 6 en lager.
> Meer informatie: <https://imagemagick.org/>.

#### Converteer bestandstype:
```shell
magick {{afbeelding.png}} {{afbeelding.jpg}}
```
#### Formaat van een afbeelding wijzigen, maak een nieuw kopie:
```shell
magick convert -resize {{100x100}} {{afbeelding.jpg}} {{afbeelding.jpg}}
```
#### Creër een GIF door middel van afbeeldingen:
```shell
magick {{*.jpg}} {{afbeelding.gif}}
```
#### Creër een dambordpatroon:
```shell
magick -size {{640x480}} pattern:checkerboard {{dambordpatroon.png}}
```
#### Converteer afbeeldingen naar individuele PDF-pagina's:
```shell
magick {{*.jpg}} +adjoin {{pagina-%d.pdf}}
```
{% endraw %}{% raw %}
<h2 id="source">
  <a href="/nl/common/source.html">source</a> <a href="#source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Voer opdrachten uit vanuit een bestand in de huidige shell.

#### Evalueer de inhoud van een bepaald bestand:
```shell
source {{pad/naar/bestand}}
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/nl/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kijk hoe lang een opdracht duurt.

#### Tijd "ls":
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="tty">
  <a href="/nl/common/tty.html">tty</a> <a href="#tty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de naam van de terminal terug.
> Meer informatie: <https://www.gnu.org/software/coreutils/tty>.

#### Druk de bestandsnaam van deze terminal af:
```shell
tty
```
{% endraw %}{% raw %}
<h2 id="unalias">
  <a href="/nl/common/unalias.html">unalias</a> <a href="#unalias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwijder aliassen.

#### Verwijder een alias:
```shell
unalias {{alias_naam}}
```
#### Verwijder alle aliassen:
```shell
unalias -a
```
{% endraw %}{% raw %}
<h2 id="unclutter">
  <a href="/nl/common/unclutter.html">unclutter</a> <a href="#unclutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verbergt de muiscursor.

#### Verbergt de muiscursor na 3 seconden:
```shell
unclutter -idle {{3}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/nl/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een alleen-lezen versie van `vim`.
> Dit is gelijk aan `vim -R`.

#### Open een bestand:
```shell
view {{bestand}}
```
{% endraw %}{% raw %}
<h2 id="visudo">
  <a href="/nl/common/visudo.html">visudo</a> <a href="#visudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bewerk veilig het sudoers-bestand.

#### Bewerk sudoers-bestand:
```shell
sudo visudo
```
#### Controleer sudoers-bestand op fouten:
```shell
sudo visudo -c
```
{% endraw %}{% raw %}
<h2 id="yapf">
  <a href="/nl/common/yapf.html">yapf</a> <a href="#yapf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python stijlgidschecker.
> Meer informatie: <https://github.com/google/yapf>.

#### Print de geformateerde diff die zal optreden uit:
```shell
yapf --diff {{pad/naar/bestand}}
```
#### Print de geformateerde diff uit en breng de wijzigingen aan in het bestand:
```shell
yapf --diff --in-place {{pad/naar/bestand}}
```
#### Formatteer alle Python-bestanden recursief in een map in parallel:
```shell
yapf --recursive --in-place --style {{pep8}} --parallel {{pad/naar/map}}
```
{% endraw %}{% raw %}
<h2 id="yes">
  <a href="/nl/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print herhaaldelijk iets op het scherm.
> Meer informatie: <https://www.gnu.org/software/coreutils/yes>.

#### Print herhaaldelijk "bericht":
```shell
yes {{bericht}}
```
#### Print herhaaldelijk "y":
```shell
yes
```
{% endraw %}{% raw %}
<h2 id="zless">
  <a href="/nl/common/zless.html">zless</a> <a href="#zless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bekijk gecomprimeerde bestanden.

#### Blader door een gecomprimeerd archief met `minder`:
```shell
zless {{bestand.txt.gz}}
```
{% endraw %}