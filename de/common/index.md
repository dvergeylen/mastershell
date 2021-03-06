---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#aapt">aapt</a>
* <a href="#ab">ab</a>
* <a href="#age">age</a>
* <a href="#alacritty">alacritty</a>
* <a href="#alias">alias</a>
* <a href="#ansible">ansible</a>
* <a href="#ansible-galaxy">ansible-galaxy</a>
* <a href="#ansible-playbook">ansible-playbook</a>
* <a href="#ansible-vault">ansible-vault</a>
* <a href="#atom">atom</a>
* <a href="#avrdude">avrdude</a>
* <a href="#aws">aws</a>
* <a href="#aws-ec2">aws ec2</a>
* <a href="#aws-iam">aws iam</a>
* <a href="#aws-kinesis">aws kinesis</a>
* <a href="#aws-quicksight">aws quicksight</a>
* <a href="#aws-s3">aws s3</a>
* <a href="#aws-google-auth">aws-google-auth</a>
* <a href="#aws-vault">aws-vault</a>
* <a href="#awslogs">awslogs</a>
* <a href="#basename">basename</a>
* <a href="#bash">bash</a>
* <a href="#bat">bat</a>
* <a href="#borg">borg</a>
* <a href="#cargo">cargo</a>
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#chmod">chmod</a>
* <a href="#chown">chown</a>
* <a href="#chromium">chromium</a>
* <a href="#chroot">chroot</a>
* <a href="#chsh">chsh</a>
* <a href="#clear">clear</a>
* <a href="#cmake">cmake</a>
* <a href="#code">code</a>
* <a href="#compare">compare</a>
* <a href="#convert">convert</a>
* <a href="#cp">cp</a>
* <a href="#cradle">cradle</a>
* <a href="#cradle-deploy">cradle deploy</a>
* <a href="#cradle-elastic">cradle elastic</a>
* <a href="#cradle-install">cradle install</a>
* <a href="#cradle-package">cradle package</a>
* <a href="#cradle-sql">cradle sql</a>
* <a href="#csvsql">csvsql</a>
* <a href="#curl">curl</a>
* <a href="#cut">cut</a>
* <a href="#dd">dd</a>
* <a href="#diff">diff</a>
* <a href="#docker">docker</a>
* <a href="#dotnet">dotnet</a>
* <a href="#echo">echo</a>
* <a href="#emacs">emacs</a>
* <a href="#emacsclient">emacsclient</a>
* <a href="#exa">exa</a>
* <a href="#fdroid">fdroid</a>
* <a href="#fdroidcl">fdroidcl</a>
* <a href="#ffmpeg">ffmpeg</a>
* <a href="#ffprobe">ffprobe</a>
* <a href="#ffsend">ffsend</a>
* <a href="#fg">fg</a>
* <a href="#firefox">firefox</a>
* <a href="#fish">fish</a>
* <a href="#fortune">fortune</a>
* <a href="#fuck">fuck</a>
* <a href="#gcc">gcc</a>
* <a href="#gdb">gdb</a>
* <a href="#git">git</a>
* <a href="#git-add">git add</a>
* <a href="#git-am">git am</a>
* <a href="#git-apply">git apply</a>
* <a href="#git-archive">git archive</a>
* <a href="#git-bisect">git bisect</a>
* <a href="#git-blame">git blame</a>
* <a href="#git-branch">git branch</a>
* <a href="#git-clone">git clone</a>
* <a href="#git-commit">git commit</a>
* <a href="#git-fetch">git fetch</a>
* <a href="#git-help">git help</a>
* <a href="#git-ignore-io">git ignore-io</a>
* <a href="#git-init">git init</a>
* <a href="#git-log">git log</a>
* <a href="#git-pull">git pull</a>
* <a href="#git-push">git push</a>
* <a href="#git-remote">git remote</a>
* <a href="#git-rm">git rm</a>
* <a href="#git-status">git status</a>
* <a href="#git-switch">git switch</a>
* <a href="#git-tag">git tag</a>
* <a href="#gpg">gpg</a>
* <a href="#gpg2">gpg2</a>
* <a href="#gplusplus">gplusplus</a>
* <a href="#grep">grep</a>
* <a href="#latex">latex</a>
* <a href="#less">less</a>
* <a href="#lolcat">lolcat</a>
* <a href="#ls">ls</a>
* <a href="#minisign">minisign</a>
* <a href="#mv">mv</a>
* <a href="#nativefier">nativefier</a>
* <a href="#npm">npm</a>
* <a href="#pass">pass</a>
* <a href="#pdflatex">pdflatex</a>
* <a href="#pdftex">pdftex</a>
* <a href="#phpbu">phpbu</a>
* <a href="#plantuml">plantuml</a>
* <a href="#rev">rev</a>
* <a href="#ssh">ssh</a>
* <a href="#ssh-agent">ssh-agent</a>
* <a href="#ssh-copy-id">ssh-copy-id</a>
* <a href="#ssh-keygen">ssh-keygen</a>
* <a href="#ssh-keyscan">ssh-keyscan</a>
* <a href="#sshfs">sshfs</a>
* <a href="#sshpass">sshpass</a>
* <a href="#tar">tar</a>
* <a href="#tex">tex</a>
* <a href="#texdoc">texdoc</a>
* <a href="#texliveonfly">texliveonfly</a>
* <a href="#tlmgr">tlmgr</a>
* <a href="#whoami">whoami</a>
* <a href="#zsh">zsh</a>

{% raw %}
<h2 id="7z">
  <a href="/de/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Dateiarchivierer mit hoher Komprimierungsrate.
> Weitere Informationen: <https://www.7-zip.org/>.

#### Archiviere eine Datei oder ein Verzeichnis:
```shell
7z a {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Verschl??ssle ein vorhandenes Archiv (einschlie??lich der Dateinamen):
```shell
7z a {{verschluesseltes_archiv.7z}} -p{{passwort}} -mhe=on {{archiv.7z}}
```
#### Extrahiere eine vorhandene 7z-Datei mit der urspr??nglichen Verzeichnisstruktur:
```shell
7z x {{archiv.7z}}
```
#### Entpacke ein Archiv mit benutzerdefiniertem Ausgabepfad:
```shell
7z x {{archiv.7z}} -o{{pfad/zu/ausgabe}}
```
#### Entpacke ein Archiv nach stdout:
```shell
7z x {{archiv.7z}} -so
```
#### Archiviere mit einem bestimmten Archivtyp:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Gib den Inhalt einer Archivdatei aus:
```shell
7z l {{archiv.7z}}
```
#### Liste alle verf??gbaren Archivtypen auf:
```shell
7z i
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/de/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Dateiarchivierer mit hoher Kompressionsrate.
> Eine alleinstehende Version von `7z` mit Unterst??tzung f??r neuere Archivtypen.
> Weitere Informationen: <https://www.7-zip.org/>.

#### Archiviere eine Datei oder ein Verzeichnis:
```shell
7za a {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Extrahiere eine existierende 7z-Datei:
```shell
7za x {{archiv}}
```
#### Archiviere mit einem bestimmten Archivtyp:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{archiv}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Gib den Inhalt einer Archivdatei aus:
```shell
7za l {{archiv}}
```
#### Liste alle verf??gbaren Archivtypen auf:
```shell
7za i
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/de/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Dateiarchivierer mit hoher Kompressionsrate.
> Eine alleinstehende Version von `7z`, die nur .7z Dateien unterst??tzt.
> Weitere Informationen: <https://www.7-zip.org/>.

#### Archiviere eine Datei oder ein Verzeichnis:
```shell
7zr a {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Extrahiere eine existierende 7z-Datei:
```shell
7zr x {{archiv.7z}}
```
#### Gib den Inhalt einer Archivdatei aus:
```shell
7zr l {{archiv}}
```
{% endraw %}{% raw %}
<h2 id="aapt">
  <a href="/de/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Asset Packaging Tool.
> Kompiliere und verpacke die Resourcen einer Android App.
> Weitere Informationen: <https://elinux.org/Android_aapt>.

#### Liste alle Dateien eines APK Archivs auf:
```shell
aapt list {{pfad/zu/app.apk}}
```
#### Zeige die Metadaten einer App an (Version, Berechtigungen, usw.):
```shell
aapt dump badging {{pfad/zu/app.apk}}
```
#### Erstelle ein neues APK Archiv mit den Dateien eines bestimmten Verzeichnisses:
```shell
aapt package -F {{pfad/zu/app.apk}} {{pfad/zu/verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="ab">
  <a href="/de/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP server Benchmarking Tool.
> Weitere Informationen: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Sende 100 HTTP GET Anfragen an eine URL:
```shell
ab -n {{100}} {{url}}
```
#### Sende 100 HTTP GET Anfragen an eine URL, wovon bis zu 10 gleichzeitig bearbeitet werden:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Wach halten:
```shell
ab -k {{url}}
```
#### Lege die maximale Anzahl an Sekunden fest, die das Benchmarking dauern darf:
```shell
ab -t {{60}} {{url}}
```
#### Sende 100 HTTP POST Anfragen an eine URL, wobei eine JSON Belastung aus einer Datei verwendet wird:
```shell
ab -n {{100}} -T {{application/json}} -p {{pfad/zu/datei.json}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="age">
  <a href="/de/common/age.html">age</a> <a href="#age"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein einfaches, modernes und sicheres Dateiverschl??sselungswerkzeug.
> Weitere Informationen: <https://age-encryption.org>.

#### Generiere eine verschl??sselte Datei, die mit einer Passphrase entschl??sselt werden kann:
```shell
age --passphrase --output {{pfad/zu/verschl??sselter_datei}} {{pfad/zu/unverschl??sselter_datei}}
```
#### Generiere ein Schl??sselpaar, speichere dabei den privaten Schl??ssel in einer unverschl??sselten Datei und gib den ??ffentlichen Schl??ssel zu stdout aus:
```shell
age-keygen --output {{pfad/zu/datei}}
```
#### Verschl??ssle eine Datei mit einem oder mehr ??ffentlichen Schl??sseln, die als Zeichenketten eingegeben werden:
```shell
age --recipient {{??ffentlicher_schl??ssel_1}} --recipient {{??ffentlicher_schl??ssel_2}} {{pfad/zu/unverschl??sselter_datei}} --output {{pfad/zu/verschl??sselter_datei}}
```
#### Verschl??ssle eine Datei mit einem oder mehr ??ffentlichen Schl??sseln, die in einer Empf??ngerdatei angegeben sind:
```shell
age --recipients-file {{pfad/zu/empf??ngerdatei}} {{pfad/zu/unverschl??sselter_datei}} --output {{pfad/zu/verschl??sselter_datei}}
```
#### Entschl??ssle eine Datei mit einer Passphrase:
```shell
age --decrypt --output {{pfad/zu/entschl??sselter_datei}} {{pfad/zu/verschl??sselter_datei}}
```
#### Entschl??ssle eine Datei mit einer privaten Schl??sseldatei:
```shell
age --decrypt --identity {{pfad/zu/privater_schl??sseldatei}} --output {{pfad/zu/entschl??sselter_datei}} {{pfad/zu/verschl??sselter_datei}}
```
{% endraw %}{% raw %}
<h2 id="alacritty">
  <a href="/de/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattform??bergreifender, GPU-beschleunigter Terminalemulator.
> Weitere Informationen: <https://github.com/alacritty/alacritty>.

#### ??ffne ein neues Alacritty-Fenster:
```shell
alacritty
```
#### Starte Alacritty in einem bestimmten Arbeitsverzeichnis:
```shell
alacritty --working-directory {{pfad/zu/verzeichnis}}
```
#### F??hre einen Befehl in einem neuen Alacritty-Fenster aus:
```shell
alacritty -e {{befehl}}
```
#### Gib eine alternative Konfigurations-Datei an (ist standardm????ig `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{pfad/zu/konfiguration.yml}}
```
#### Starte mit aktiviertem Live-Konfigurations-Neuladen (kann auch standardm????ig in `alacritty.yml` eingestellt werden):
```shell
alacritty --live-config-reload --config-file {{pfad/zu/konfiguration.yml}}
```
{% endraw %}{% raw %}
<h2 id="alias">
  <a href="/de/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstellt Aliasse - Alterative Namen f??r Befehle.
> Aliasse laufen mit der aktuellen Shell-Sitzung ab, es sei denn, sie werden in der Konfigurationsdatei der Shell definiert, z.B. `~/.bashrc`.
> Weitere Informationen: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listet alle Aliasse auf:
```shell
alias
```
#### Erstellt einen Alias:
```shell
alias {{alias}}="{{befehl}}"
```
#### Zeigt den mit einem bestimmten Alias verkn??pften Befehl an:
```shell
alias {{alias}}
```
#### Entferne einen Alias:
```shell
unalias {{alias}}
```
#### Macht `rm` zu einem interaktiven Befehl:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Erstellt den Alias `la` f??r `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="ansible-galaxy">
  <a href="/de/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> M??gliche Rollen erstellen und verwalten.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### Installiere eine Rolle:
```shell
ansible-galaxy install {{benutzername.rollenname}}
```
#### Entferne eine Rolle:
```shell
ansible-galaxy remove {{benutzername.rollenname}}
```
#### Installierte Rollen auflisten:
```shell
ansible-galaxy list
```
#### Suche nach einer bestimmten Rolle:
```shell
ansible-galaxy search {{rollenname}}
```
#### Erstelle eine neue Rolle:
```shell
ansible-galaxy init {{rollenname}}
```
{% endraw %}{% raw %}
<h2 id="ansible-playbook">
  <a href="/de/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> In Playbook definierte Aufgaben auf entfernten Rechnern ??ber SSH ausf??hren.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### F??hre Aufgaben im Playbook aus:
```shell
ansible-playbook {{playbook}}
```
#### F??hre Aufgaben im Playbook mit benutzerdefiniertem Host-Bestand aus:
```shell
ansible-playbook {{playbook}} -i {{inventory_datei}}
```
#### F??hre Aufgaben im Playbook aus, wobei zus??tzliche Variablen ??ber die Befehlszeile definiert werden:
```shell
ansible-playbook {{playbook}} -e "{{variable1}}={{wert1}} {{variable2}}={{wert2}}"
```
#### F??hre Aufgaben in Playbook mit zus??tzlichen Variablen aus, die in einer JSON-Datei definiert sind:
```shell
ansible-playbook {{playbook}} -e "@{{variablen.json}}"
```
#### F??hre Aufgaben im Playbook f??r die angegebenen Tags aus:
```shell
ansible-playbook {{playbook}} --tags {{tag1,tag2}}
```
#### F??hre Aufgaben in einem Playbook aus, die mit einer bestimmten Aufgabe beginnen:
```shell
ansible-playbook {{playbook}} --start-at {{aufgabenname}}
```
{% endraw %}{% raw %}
<h2 id="ansible-vault">
  <a href="/de/common/ansible-vault.html">ansible-vault</a> <a href="#ansible-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verschl??sselt und entschl??sselt Werte, Datenstrukturen und Dateien innerhalb von Ansible-Projekten.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/user_guide/vault.html>.

#### Erstelle eine neue verschl??sselte Vault-Datei mit einer Eingabeaufforderung f??r ein Passwort:
```shell
ansible-vault create {{vault_datei}}
```
#### Erstelle eine neue verschl??sselte Vault-Datei mit einer Vault-Schl??sseldatei, um sie zu verschl??sseln:
```shell
ansible-vault create --vault-password-file={{schl??sseldatei}} {{vault_datei}}
```
#### Verschl??ssle eine vorhandene Datei mit einer optionalen Schl??sseldatei:
```shell
ansible-vault encrypt --vault-password-file={{schl??sseldatei}} {{vault_file}}
```
#### Verschl??ssle eine Zeichenfolge mit dem verschl??sselten Zeichenfolgenformat von Ansible, wobei interaktive Eingabeaufforderungen angezeigt werden:
```shell
ansible-vault encrypt_string
```
#### Zeige eine verschl??sselten Datei an, wobei eine Kennwortdatei zum Entschl??sseln verwendet wird:
```shell
ansible-vault view --vault-password-file={{schl??sseldatei}} {{vault_datei}}
```
#### Verschl??ssle eine bereits verschl??sselte Vault Datei mit einer neuen Kennwortdatei neu:
```shell
ansible-vault rekey --vault-password-file={{alte_schl??sseldatei}} --new-vault-password-file={{neue_schl??sseldatei}} {{vault_datei}}
```
{% endraw %}{% raw %}
<h2 id="ansible">
  <a href="/de/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Computergruppen per Fernzugriff ??ber SSH.
> Verwende die Datei `/etc/ansible/hosts`, um neue Gruppen/Hosts hinzuzuf??gen.
> Weitere Informationen: <https://www.ansible.com/>.

#### Liste Hosts auf, die zu einer Gruppe geh??ren:
```shell
ansible {{gruppe}} --list-hosts
```
#### Pinge eine Gruppe von Hosts an:
```shell
ansible {{gruppe}} -m ping
```
#### Zeige Informationen ??ber eine Gruppe von Hosts an:
```shell
ansible {{gruppe}} -m setup
```
#### F??hre einen Befehl auf einer Gruppe von Hosts aus:
```shell
ansible {{gruppe}} -m command -a '{{befehl}}'
```
#### F??hre einen Befehl mit administrativen Privilegien aus:
```shell
ansible {{gruppe}} --become --ask-become-pass -m command -a '{{befehl}}'
```
#### F??hre einen Befehl mit einer benutzerdefinierten Inventardatei aus:
```shell
ansible {{Gruppe}} -i {{inventardatei}} -m command -a '{{befehl}}'
```
#### Liste alle Gruppen eines Inventars auf:
```shell
ansible localhost -m debug -a '{{var=groups.keys()}}'
```
{% endraw %}{% raw %}
<h2 id="atom">
  <a href="/de/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein plattform??bergreifender erweiterbarer Texteditor.
> Erweiterungen werden durch `apm` verwaltet.
> Weitere Informationen: <https://atom.io/>.

#### ??ffne eine Datei oder ein Verzeichnis:
```shell
atom {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ffne eine Datei oder ein Verzeichnis in einem neuen Fenster:
```shell
atom -n {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ffne eine Datei oder ein Verzeichnis in einem vorhandenen Fenster:
```shell
atom --add {{pfad/zu/datei_oder_verzeichnis}}
```
#### Starte Atom im sicheren Modus (Es werden keine zus??tzlichen Pakete geladen):
```shell
atom --safe
```
#### Verhindert, dass sich Atom in den Hintergrund absetzt und h??lt es mit dem Terminal verbunden:
```shell
atom --foreground
```
#### Wartet, bis Atom geschlossen wurde, bevor die Eingabeaufforderung wieder aktiv wird (N??tzlich als `git commit` Editor):
```shell
atom --wait
```
{% endraw %}{% raw %}
<h2 id="avrdude">
  <a href="/de/common/avrdude.html">avrdude</a> <a href="#avrdude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Treiberprogramm f??r Atmel AVR Mikrocontroller-Programmierung.
> Weitere Informationen: <https://www.nongnu.org/avrdude/>.

#### Schreibt den Speicherinhalt eines AVR-Mikrocontrollers in eine Datei:
```shell
avrdude -p {{avr_ger??t}} -c {{programmer}} -U flash:r:{{pfad/zu/datei.hex}}:i
```
#### Schreibt den Inhalt einer Datei in einen AVR-Mikrocontroller:
```shell
avrdude -p {{avr_ger??t}} -c {{programmer}} -U flash:w:{{pfad/zu/datei.hex}}
```
#### Liste alle verf??gbaren AVR-Ger??te auf:
```shell
avrdude -p \?
```
#### Liste alle verf??gbaren AVR-Programmer auf:
```shell
avrdude -c \?
```
{% endraw %}{% raw %}
<h2 id="aws-ec2">
  <a href="/de/common/aws-ec2.html">aws ec2</a> <a href="#aws-ec2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI f??r AWS EC2.
> AWS EC2 stellt eine sichere und skalierbare Einheit in der AWS Cloud zur Verf??gung um ein schnelleres Entwickeln und Ausrollen von Software zu erm??glichen.
> Weitere Informationen: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

#### Liste alle verf??gbaren EC2 Befehle auf:
```shell
aws ec2 help
```
#### Zeige Hilfe f??r bestimmte EC2 Unterbefehle an:
```shell
aws ec2 {{unterbefehl}} help
```
#### Liste Informationen zu einer bestimmten Instanz auf:
```shell
aws ec2 describe-instances --instance-ids {{instanz_id}}
```
#### Liste Informationen zu allen Instanzen auf:
```shell
aws ec2 describe-instances
```
#### Liste Informationen zu allen EC2 Volumen auf:
```shell
aws ec2 describe-volumes
```
#### Liste Informationen zu einem bestimmten EC2 Volumen auf:
```shell
aws ec2 describe-volume --volume-id {{volumen_id}}
```
#### Erstelle einen Snapshot, basierend auf einem EC2 Volumen:
```shell
aws ec2 create-snapshot --volume-id {{volumen_id}}
```
#### Liste alle verf??gbaren AMIs (Amazon Machine Images) auf:
```shell
aws ec2 describe-images
```
{% endraw %}{% raw %}
<h2 id="aws-google-auth">
  <a href="/de/common/aws-google-auth.html">aws-google-auth</a> <a href="#aws-google-auth"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI, um tempor??re AWS credentials (STS) ??ber Google Apps als Single Sign-On Dienstleister zu erhalten.
> Weitere Informationen: <https://github.com/cevoaustralia/aws-google-auth>.

#### Einloggen mit Google SSO ??ber IDP- und SP-Kennung f??r die Dauer einer Stunde:
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}}
```
#### Einloggen mit der Option eine Rolle auszuw??hlen (im Falle mehrerer verf??gbarer SAML Rollen):
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a
```
#### L??se Aliasse von AWS Accounts auf:
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a --resolve-aliases
```
#### Zeige Hilfs-Informationen:
```shell
aws-google-auth -h
```
{% endraw %}{% raw %}
<h2 id="aws-iam">
  <a href="/de/common/aws-iam.html">aws iam</a> <a href="#aws-iam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI f??r AWS IAM.
> Weitere Informationen: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/iam/index.html>.

#### Zeige die AWS IAM Hilfeseite (beinhaltet auch Hinweise f??r alle Unterbefehle):
```shell
aws iam help
```
#### Liste aller Benutzer auf:
```shell
aws iam list-users
```
#### Liste aller Richtlinien auf:
```shell
aws iam list-policies
```
#### Liste aller Gruppen auf:
```shell
aws iam list-groups
```
#### Liste aller Benutzer zu einer Gruppe auf:
```shell
aws iam get-group --group-name {{gruppe}}
```
#### Liste einer IAM Richtlinie detailliert auf:
```shell
aws iam get-policy --policy-arn arn:aws:iam::aws:policy/{{richtlinie}}
```
#### Liste alle Zugriffsschl??ssel auf:
```shell
aws iam list-access-keys
```
#### Liste alle Zugriffsschl??ssel f??r einen Benutzer auf:
```shell
aws iam list-access-keys --user-name {{benutzername}}
```
{% endraw %}{% raw %}
<h2 id="aws-kinesis">
  <a href="/de/common/aws-kinesis.html">aws kinesis</a> <a href="#aws-kinesis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Offizielles AWS CLI f??r die Amazon Kinesis-Streaming-Datenplattform.
> Weitere Informationen: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>.

#### Liste alle Streams auf:
```shell
aws kinesis list-streams
```
#### Schreibe einen Datensatz in einen Kinesis Stream:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{schl??ssel}} --data {{base64_codierte_nachricht}}
```
#### Schreibe einen Datensatze in einen Kinesis Stream mit base64 inline Encodierung:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{schl??ssel}} --data "$( echo "{{meine nachricht}}" | base64 )"
```
#### Liste alle verf??gbaren Shards in einem Stream auf:
```shell
aws kinesis list-shards --stream-name {{name}}
```
#### Rufe einen Shard Iterators auf, um diesen beginnend mit der ??ltesten Nachricht auszulesen:
```shell
aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}
```
#### Lies einen Datensatz aus einem Shard ??ber einen Shard Iterator:
```shell
aws kinesis get-records --shard-iterator {{iterator}}
```
{% endraw %}{% raw %}
<h2 id="aws-quicksight">
  <a href="/de/common/aws-quicksight.html">aws quicksight</a> <a href="#aws-quicksight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI f??r AWS QuickSight.
> Weitere Informationen: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>.

#### Liste alle Datens??tze auf:
```shell
aws quicksight list-data-sets --aws-account-id {{aws_account_id}}
```
#### Liste alle Benutzer auf:
```shell
aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default
```
#### Liste alle Gruppen auf:
```shell
aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default
```
#### Liste alle Dashboards auf:
```shell
aws quicksight list-dashboards --aws-account-id {{aws_account_id}}
```
#### Liste eine Datensatz detailliert aus:
```shell
aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{datensatz_id}}
```
#### Liste Zugangsberechtungen zu einem Datensatz auf:
```shell
aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{datensatz_id}}
```
{% endraw %}{% raw %}
<h2 id="aws-s3">
  <a href="/de/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI f??r AWS S3. AWS S3 stellt Speicherplatz in der Cloud zur Verf??gung.
> Weitere Informationen: <https://aws.amazon.com/cli>.

#### Liste alle Objekte in einem Bucket auf:
```shell
aws s3 ls {{bucket_name}}
```
#### Synchronisiere Dateien und Verzeichnissen zu einem Bucket:
```shell
aws s3 sync {{pfad/zu/datei_oder_verzeichnis}} s3://{{bucket_name}}
```
#### Synchronisiere Dateien und Verzeichnissen von einem Bucket:
```shell
aws s3 sync s3://{{bucket_name}} {{pfad/zu/ziel}}
```
#### Synchronisiere Dateien und Verzeichnissen mit Ausnahmen:
```shell
aws s3 sync {{pfad/zu/datei_oder_verzeichnis}} s3://{{bucket_name}} --exclude {{pfad/zu/datei}} --exclude {{pfad/zu/verzeichnis}}/*
```
#### Entferne ein Objekt von einem Bucket:
```shell
aws s3 rm s3://{{bucket}}/{{pfad/zu/datei}}
```
#### Probelauf eines angegeben Kommandos ohne diesen auszuf??hren:
```shell
aws s3 {{befehl}} --dryrun
```
{% endraw %}{% raw %}
<h2 id="aws-vault">
  <a href="/de/common/aws-vault.html">aws-vault</a> <a href="#aws-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Tresor f??r Entwicklungsumgebungen um AWS Sicherheitsschl??ssel sicher speichern und abrufen zu k??nnen.
> Weitere Informationen: <https://github.com/99designs/aws-vault>.

#### F??ge einen Sicherheitsschl??ssel als Profil zu einem Tresor hinzu:
```shell
aws-vault add {{profil}}
```
#### F??hre einen Befehl mit AWS Sicherheitsschl??sseln aus dem angegebenen Profil aus:
```shell
aws-vault exec {{profil}} -- {{aws s3 ls}}
```
#### ??ffne ein Browserfenster f??r den Login in die AWS Konsole:
```shell
aws-vault login {{profil}}
```
#### Liste alle Profile zusammen mit deren Sicherheitsschl??sseln und Sitzungen auf:
```shell
aws-vault list
```
#### Rotiere die AWS Sicherheitsschl??ssel f??r ein Profil:
```shell
aws-vault rotate {{profil}}
```
#### Entferne Sicherheitsschl??sseln eines Profils aus dem Tresor:
```shell
aws-vault remove {{profil}}
```
{% endraw %}{% raw %}
<h2 id="aws">
  <a href="/de/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Das offizielle CLI f??r Amazon Web Services.
> Ausf??hrungssassistent, SSO, Autovervollst??ndigung von Ressourcen sowie YAML Optionen sind nur unter Version v2 verf??gbar.
> Weitere Informationen: <https://aws.amazon.com/cli>.

#### Konfiguriere die AWS Kommandozeile:
```shell
aws configure wizard
```
#### Konfiguriere die AWS Kommandozeile mit Hilfe von SSO:
```shell
aws configure sso
```
#### Zeige Hilfe f??r ein Kommando an:
```shell
aws {{befehl}} help
```
#### Zeige Informationen ??ber die eigene angenomme Identit??t (h??ufig benutzt zur Fehlersuche):
```shell
aws sts get-caller-identity
```
#### Liste alle AWS Ressourcen in einer Region mit YAML Formatierung auf:
```shell
aws dynamodb list-tables --region {{us-east-1}} --output yaml
```
#### Erstelle einen IAM Benutzer mit Ausf??hrungsassistent:
```shell
aws iam create-user --cli-auto-prompt
```
#### ??ffne einen Assitenten f??r eine AWS Ressource:
```shell
aws dynamodb wizard {{neue_tabelle}}
```
#### Erstelle einen JSON CLI-Aufbau (hilfreich f??r Infrastruktur-Automation):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}{% raw %}
<h2 id="awslogs">
  <a href="/de/common/awslogs.html">awslogs</a> <a href="#awslogs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI um Log-Gruppen, Streams und Events von Amazon CloudWatch Logs abzurufen.
> Weitere Informationen: <https://github.com/jorgebastida/awslogs>.

#### Liste alle Log-Gruppen auf:
```shell
awslogs groups
```
#### Liste alle bestehenden Streams einer angegebenen Log Gruppe auf:
```shell
awslogs streams {{/var/log/syslog}}
```
#### Rufe alle logs f??r jegliche Streams in der angegebenen Log-Gruppe f??r die letzten 1 bis 2 Stunden ab:
```shell
awslogs get {{/var/log/syslog}} --start='{{2h ago}}' --end='{{1h ago}}'
```
#### Rufe alle Logs f??r einen bestimmten CloudWatch-Logs Filter-Ausdruck ab:
```shell
awslogs get {{/aws/lambda/meine_lambda_gruppe}} --filter-pattern='{{ERROR}}'
```
#### Beobachte Logs f??r jegliche Streams in der angegebenen Log-Gruppe:
```shell
awslogs get {{/var/log/syslog}} ALL --watch
```
{% endraw %}{% raw %}
<h2 id="basename">
  <a href="/de/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Entfernt f??hrende Verzeichniskomponenten in einem Pfad.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/basename>.

#### Ermittle den Dateinamen in einem Pfad:
```shell
basename {{pfad/zu/datei}}
```
#### Ermittle den rechtesten Verzeichnisnamen in einem Pfad:
```shell
basename {{pfad/zu/verzeichnis/}}
```
#### Ermittle den Dateinamen in einem Pfad und entferne den angegebenen Suffix aus diesem:
```shell
basename {{pfad/zu/datei}} {{suffix}}
```
{% endraw %}{% raw %}
<h2 id="bash">
  <a href="/de/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> `sh`-kompatibler Kommandozeilen-Interpreter.
> Weitere Informationen: <https://gnu.org/software/bash>.

#### Interaktive Shell starten:
```shell
bash
```
#### F??hre einen Befehl aus:
```shell
bash -c "{{befehl}}"
```
#### F??hre Befehle aus einer Datei aus:
```shell
bash {{pfad/zu/datei.sh}}
```
#### F??hre Befehle aus einer Datei aus and protokolliere alle ausgef??hrten Befehle an das Terminal:
```shell
bash -x {{pfad/zu/datei.sh}}
```
#### F??hre Befehle aus einer Datei aus und stoppe beim ersten Fehler:
```shell
bash -e {{pfad/zu/datei.sh}}
```
#### F??hre Befehle von stdin aus:
```shell
bash -s
```
#### Gib die Version von bash aus (verwende `echo $BASH_VERSION`, um nur die Versionszeichenkette anzuzeigen):
```shell
bash --version
```
{% endraw %}{% raw %}
<h2 id="bat">
  <a href="/de/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ausgabe und Verkettung von einzelnen Dateien.
> Ein `cat`-Ersatz mit Syntax-Hervorhebung und Git-Integration.

#### Gib den Inhalt einer Datei in stdout aus:
```shell
bat {{pfad/zu/datei}}
```
#### Verkette mehrere Dateien zu eine Zieldatei:
```shell
bat {{pfad/zu/datei1}} {{pfad/zu/datei2}} > {{pfad/zu/ziel_datei}}
```
#### H??nge mehrere Dateien an eine Zieldatei an:
```shell
bat {{pfad/zu/datei1}} {{pfad/zu/datei2}} >> {{pfad/zu/ziel_datei}}
```
#### Nummeriere alle ausgegebenen Zeilen:
```shell
bat -n {{pfad/zu/datei}}
```
#### Hebe den Syntax einer JSON-Datei hervor:
```shell
bat --language {{json}} {{pfad/zu/datei.json}}
```
#### Zeige alle unterst??zten Sprachen an:
```shell
bat --list-languages
```
{% endraw %}{% raw %}
<h2 id="borg">
  <a href="/de/common/borg.html">borg</a> <a href="#borg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deduplizierendes Sicherungswerkzeug.
> Erstellt lokale oder entfernte Sicherungen, die als Dateisysteme einh??ngbar sind.
> Weitere Informationen: <https://borgbackup.readthedocs.io/en/stable/usage/general.html>.

#### Initialisiere ein lokales Repository:
```shell
borg init {{pfad/zu/repo_verzeichnis}}
```
#### Sichere ein Verzeichnis in das Repository und erstelle ein Archiv mit dem Namen "Montag":
```shell
borg create --progress {{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/quell_verzeichnis}}
```
#### Liste alle Archive in einem Repository auf:
```shell
borg list {{pfad/zu/repo_verzeichnis}}
```
#### Extrahiere ein bestimmtes Verzeichnis aus dem "Montag"-Archiv in einem entfernten Repository, unter Ausschluss aller `*.ext`-Dateien:
```shell
borg extract {{benutzer}}@{{host}}:{{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/ziel_verzeichnis} --exclude '{{*.ext}}'
```
#### Bereinige ein Repository, indem alle Archive gel??scht werden, die ??lter als 7 Tage sind und ??nderungen aufweisen:
```shell
borg prune --keep-within {{7d}} --list {{pfad/zu/repo_verzeichnis}}
```
#### H??nge ein Repository als FUSE-Dateisystem ein:
```shell
borg mount {{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/mountpoint}}
```
#### Zeige Hilfe zur Erstellung von Archiven an:
```shell
borg create --help
```
{% endraw %}{% raw %}
<h2 id="cargo">
  <a href="/de/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust Paketmanager.
> Verwalte Rust-Projekte und deren Abh??ngigkeiten (crates).
> Weitere Informationen: <https://crates.io/>.

#### Suche nach Abh??ngigkeiten (crates):
```shell
cargo search {{suche}}
```
#### Installiere eine Abh??ngigkeit (crate):
```shell
cargo install {{abh??ngigkeit}}
```
#### Liste alle installierten Abh??ngigkeiten (crates) auf:
```shell
cargo install --list
```
#### Erzeuge ein neues Rust-Projekt als Anwendung oder Bibliothek im aktuellen Verzeichnis:
```shell
cargo init --{{bin|lib}}
```
#### Erzeuge ein neues Rust-Projekt als Anwendung oder Bibliothek im angegebenen Verzeichnis:
```shell
cargo new {{pfad/zu/verzeichnis}} --{{bin|lib}}
```
#### Erstelle (bzw. kompiliere) ein Rust-Projekt im aktuellen Verzeichnis:
```shell
cargo build
```
#### Erstelle (bzw. kompiliere) ein Rust-Projekt mit einer bestimmten Anzahl an Threads (standardm????ig die Anzahl der CPU-Kerne):
```shell
cargo build -j {{thread_anzahl}}
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/de/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verkette und gib einzelne oder mehrere Dateien aus.
> Mehrere Informationen: <https://www.gnu.org/software/coreutils/cat>.

#### Gib den Inhalt einer Datei aus:
```shell
cat {{pfad/zu/datei}}
```
#### Verkette mehrere Dateien und speichere das Ergebnis in einer neuen Datei:
```shell
cat {{pfad/zu/datei1}} {{pfad/zu/datei2}} > {{pfad/zu/ziel_datei}}
```
#### Verkette mehrere Dateien und h??nge des Ergebnis an eine Datei an:
```shell
cat {{pfad/zu/datei1}} {{pfad/zu/datei2}} >> {{pfad/zu/ziel_datei}}
```
#### Nummeriere alle ausgegebenen Zeilen:
```shell
cat -n {{pfad/zu/datei}}
```
#### Gib eine Datei inklusive aller unsichtbaren Leerzeichen aus (mit `M-` Pr??fix wenn sie nicht ASCII sind):
```shell
cat -v -t -e {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/de/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ndere das aktuelle Arbeitsverzeichnis.
> Weitere Informationen: <https://man.archlinux.org/man/cd.n>.

#### Wechsle in das angegebene Verzeichnis:
```shell
cd {{pfad/zu/verzeichnis}}
```
#### Wechsle in das Home-Verzeichnis des aktuellen Benutzers:
```shell
cd
```
#### Wechsle zum Verzeichnis ??ber dem aktuellen Verzeichnis:
```shell
cd ..
```
#### Wechsle zum zuletzt gew??hlten Verzeichnis:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="chmod">
  <a href="/de/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ndere die Zugriffsberechtigungen einer Datei oder eines Verzeichnisses.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chmod>.

#### Gib dem Besitzer einer Datei ([u]ser) das Recht, sie auszuf??hren (e[x]ecute):
```shell
chmod u+x {{pfad/zu/datei}}
```
#### Gib dem Besitzer ([u]ser) Rechte zum Lesen ([r]ead) und Schreiben ([w]rite) einer Datei / einem Verzeichnis:
```shell
chmod u+rw {{pfad/zu/datei_oder_verzeichnis}}
```
#### Entferne die Ausf??hrrechte (e[x]ecute) der Besitzer[g]ruppe:
```shell
chmod g-x {{pfad/zu/datei}}
```
#### Gib [a]llen Benutzern Rechte zum Lesen ([r]ead) und Ausf??hren (e[x]ecute) einer Datei:
```shell
chmod a+rx {{pfad/zu/datei}}
```
#### Gib anderen ([o]thers) (nicht in der Besitzer[g]ruppe) die gleichen Rechte wie der Besitzer[g]ruppe:
```shell
chmod o=g {{pfad/zu/datei}}
```
#### Entferne alle Rechte der anderen ([o]thers):
```shell
chmod o= {{pfad/zu/datei}}
```
#### ??ndere Rechte rekursiv, indem der Besitzer[g]ruppe und anderen ([o]thers) die Rechte zum Schreiben ([w]rite) geben werden:
```shell
chmod -R g+w,o+w {{pfad/zu/verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="chown">
  <a href="/de/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ndere den Besitzer und die Besitzergruppe von Dateien und Verzeichnissen.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chown>.

#### ??ndere den Besitzer einer Datei/eines Verzeichnisses:
```shell
chown {{benutzer}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ndere den Besitzer und die Besitzergruppe einer Datei/eines Verzeichnisses:
```shell
chown {{benutzer}}:{{gruppe}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ndere den Besitzer eines Verzeichnisses rekursiv:
```shell
chown -R {{benutzer}} {{pfad/zu/verzeichnis}}
```
#### ??ndere den Besitzer eines symbolischen Links:
```shell
chown -h {{benutzer}} {{pfad/zu/symlink}}
```
#### ??ndere den Besitzer einer Datei/eines Verzeichnisses, damit sie/es mit einer Referenzdatei ??bereinstimmt:
```shell
chown --reference={{pfad/zu/referenzdatei_oder_verzeichnis}} {{pfad/zu/datei_oder_verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="chromium">
  <a href="/de/common/chromium.html">chromium</a> <a href="#chromium"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-Source-Webbrowser von Google.
> Weitere Informationen: <https://chromium.org>.

#### ??ffne eine html-Datei:
```shell
chromium {{pfad/zu/datei.html}}
```
#### ??ffne eine bestimmte URL:
```shell
chromium {{beispiel.com}}
```
#### ??ffne eine URL im Inkognito-Modus:
```shell
chromium --incognito {{beispiel.com}}
```
#### ??ffne eine URL in einem neuen Fenster:
```shell
chromium --new-window {{beispiel.com}}
```
#### ??ffne eine URL im Anwendungsmodus (ohne Symbolleisten, Suchleiste, Schaltfl??chen usw.):
```shell
chromium --app='{{https://beispiel.com}}'
```
#### ??ffne eine URL und verwende einen Proxy-Server:
```shell
chromium --proxy-server="{{socks5://hostname:66}}" {{beispiel.com}}
```
{% endraw %}{% raw %}
<h2 id="chroot">
  <a href="/de/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F??hre einen Befehl oder eine interaktive Shell mit einem speziellen root-Verzeichnis aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chroot>.

#### F??hre einen Befehl mit einem neuen root-Verzeichnis aus:
```shell
chroot {{pfad/zu/root_verzeichnis}} {{befehl}}
```
#### Lege einen Benutzer und eine Gruppe (ID oder Name) fest, der benutzt werden soll:
```shell
chroot --userspec={{benutzer:gruppe}}
```
{% endraw %}{% raw %}
<h2 id="chsh">
  <a href="/de/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ndere die Login-Shell eines Benutzers.
> Weitere Informationen: <https://manned.org/chsh>.

#### ??ndere die Login-Shell eines Benutzers:
```shell
chsh -s {{pfad/zu/shell}} {{benutzername}}
```
{% endraw %}{% raw %}
<h2 id="clear">
  <a href="/de/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Leert den Bildschirm eines Terminals.
> Weitere Informationen: <https://manned.org/clear>.

#### Leere den Bildschirm (??quivalent zu Strg+L in einer Bash Shell):
```shell
clear
```
#### Leere den Bildschirm, aber erhalte den R??ckscroll-Puffer des Terminals:
```shell
clear -x
```
#### Lege den Typ des zu leerenden Terminals fest (Standardwert ist die Umgebungsvariable $TERM):
```shell
clear -T {{typ_des_terminals}}
```
#### Zeige die Version von `ncurses` an, die von `clear` benutzt wird:
```shell
clear -V
```
{% endraw %}{% raw %}
<h2 id="cmake">
  <a href="/de/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattform??bergreifndes Build-Automatisierungs-System, das Vorlagen f??r native Build-Systeme erzeugt.
> Weitere Informationen: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Erzeuge eine Build-Vorlage im aktuellen Verzeichnis mit `CMakeLists.txt` eines Projektordners:
```shell
cmake {{pfad/zu/projektordner}}
```
#### Erzeuge eine Build-Vorlage mit der Build-Art `Release`:
```shell
cmake {{pfad/zu/projektordner}} -D {{CMAKE_BUILD_TYPE=Release}}
```
#### Benutze eine generierte Vorlage, um Artifakte zu erzeugen:
```shell
cmake --build {{pfad/zu/build_verzeichnis}}
```
#### Installiere die Build-Artifakte in `/usr/local/` und enferne Debugsymbole:
```shell
cmake --install {{pfad/zu/build_verzeichnis}} --strip
```
#### Installiere die Build-Artifakte mit einem eigenen Pr??fix f??r Pfade:
```shell
cmake --install {{pfad/zu/build_verzeichnis}} --strip --prefix {{pfad/zu/verzeichnis}}
```
#### F??hre ein bestimmtes Build-Ziel aus:
```shell
cmake --build {{pfad/zu/build_verzeichnis}} --target {{zielname}}
```
{% endraw %}{% raw %}
<h2 id="code">
  <a href="/de/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> Weitere Informationen: <https://github.com/microsoft/vscode>.

#### ??ffne VS Code:
```shell
code
```
#### ??ffne das aktuelle Verzeichnis in VS Code:
```shell
code .
```
#### ??ffne eine bestimmte Datei oder Verzeichnis in VS Code:
```shell
code {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ffne eine Datei oder ein Verzeichnis im aktuell ge??ffnetem VS Code Fenster:
```shell
code --reuse-window {{pfad/zu/datei_oder_verzeichnis}}
```
#### ??ffne mehrere Dateien in VS Code:
```shell
code -d {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### ??ffne VS Code root:
```shell
sudo code {{pfad/zu/datei_oder_verzeichnis}} --user-data-dir
```
{% endraw %}{% raw %}
<h2 id="compare">
  <a href="/de/common/compare.html">compare</a> <a href="#compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Unterschiede von zwei Bildern.
> Weitere Informationen: <https://imagemagick.org/script/compare.php>.

#### Vergleiche 2 Bilder:
```shell
compare {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/diff.png}}
```
#### Vergleiche 2 Bilder mit einer bestimmten Metrik (standardm????ig NCC):
```shell
compare -verbose -metric {{PSNR}} {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/diff.png}}
```
{% endraw %}{% raw %}
<h2 id="convert">
  <a href="/de/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ImageMagick Bildkonvertierungswerkzeug.
> Weitere Informationen: <https://imagemagick.org/script/convert.php>.

#### Konvertiere ein Bild von JPG nach PNG:
```shell
convert {{pfad/zu/bild.jpg}} {{pfad/zu/bild.png}}
```
#### Skaliere ein Bild auf 50% seiner Originalgr????e:
```shell
convert {{pfad/zu/bild.png}} -resize 50% {{pfad/zu/bild2.png}}
```
#### Skaliere ein Bild unter Beibehaltung des urspr??nglichen Seitenverh??ltnisses auf eine maximale Gr????e von 640x480:
```shell
convert {{pfad/zu/bild.png}} -resize 640x480 {{pfad/zu/bild2.png}}
```
#### H??nge Bilder horizontal aneinader:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} +append {{pfad/zu/bild123.png}}
```
#### H??nge Bilder vertikal aneinander:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} -append {{pfad/zu/bild123.png}}
```
#### Erstelle ein animiertes GIF aus einer Serie von Bildern mit einer Verz??gerung von 100 ms zwischen den Bildern:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} -delay {{10}} {{pfad/zu/animation.gif}}
```
#### Erstelle ein Bild mit nichts als einem festen Hintergrund:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{pfad/zu/bild.png}}
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/de/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kopiere Dateien und Verzeichnisse.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/cp>.

#### Kopiere eine Datei an einen anderen Ort:
```shell
cp {{pfad/zu/datei}} {{pfad/zu/kopie}}
```
#### Kopiere eine Datei an einen anderen Ort und behalte den Dateinamen:
```shell
cp {{pfad/zu/datei}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere ein Verzeichnis rekursiv (falls der Zielort bereits existiert, wird das Verzeichnis in das Zielverzeichnis kopiert):
```shell
cp -r {{pfad/zu/verzeichnis}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere ein Verzeichnis rekursiv und gib alle Dateien aus, w??hrend sie kopiert werden:
```shell
cp -vr {{pfad/zu/verzeichnis}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere alle Textdateien in einem Verzeichnis und warte auf eine Best??tigung, falls eine Datei ??berschrieben werden soll:
```shell
cp -i {{/pfad/zu/*.txt}} {{pfad/zu/zielverzeichnis}}
```
#### Folge symbolischen Links vor dem Kopieren:
```shell
cp -L {{link}} {{pfad/zu/zielverzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="cradle-deploy">
  <a href="/de/common/cradle-deploy.html">cradle deploy</a> <a href="#cradle-deploy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Cradle Implementierungen.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#deploy>.

#### Implementiere Cradle auf einem Server:
```shell
cradle deploy production
```
#### Implementiere statische Anlagen zu Amazon S3:
```shell
cradle deploy s3
```
#### Implementiere statische Anlagen inklusive den Yarn Komponenten:
```shell
cradle deploy s3 --include-yarn
```
#### Implementiere statische Anlagen inklusive dem "upload" Verzeichnis:
```shell
cradle deploy s3 --include-upload
```
{% endraw %}{% raw %}
<h2 id="cradle-elastic">
  <a href="/de/common/cradle-elastic.html">cradle elastic</a> <a href="#cradle-elastic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte ElasticSearch Instanzen einer Cradle Instanz.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#elastic>.

#### Entleere den ElasticSearch Index:
```shell
cradle elastic flush
```
#### Entleere den ElasticSearch Index f??r ein bestimmtes Paket:
```shell
cradle elastic flush {{paket}}
```
#### Sende ein ElasticSearch Schema ab:
```shell
cradle elastic map
```
#### Sende ein ElasticSearch Schema f??r ein bestimmtes Paket ab:
```shell
cradle elastic map {{paket}}
```
#### Bef??lle die ElasticSearch Indizes f??r alle Pakete:
```shell
cradle elastic populate
```
#### Bef??lle die ElasticSearch Indizes f??r ein bestimmtes Paket:
```shell
cradle elastic populate {{paket}}
```
{% endraw %}{% raw %}
<h2 id="cradle-install">
  <a href="/de/common/cradle-install.html">cradle install</a> <a href="#cradle-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere Cradle PHP Framework Komponenten.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#install>.

#### Installiere Cradle Komponenten mithilfe eines Dialogs:
```shell
cradle install
```
#### Installiere Cradle Komponenten gewaltsam:
```shell
cradle install --force
```
#### ??berspringe SQL Migrationen:
```shell
cradle install --skip-sql
```
#### ??berspringe Paket-Aktualisierungen:
```shell
cradle install --skip-versioning
```
#### Zeige Details ??ber eine benutzer-spezifische Datenbank:
```shell
cradle install -h {{hostname}} -u {{benutzer}} -p {{passwort}}
```
{% endraw %}{% raw %}
<h2 id="cradle-package">
  <a href="/de/common/cradle-package.html">cradle package</a> <a href="#cradle-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Pakete f??r Cradle Instanzen.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#package>.

#### Liste aller verf??gbaren Pakete auf:
```shell
cradle package list
```
#### Suche nach einem Paket:
```shell
cradle package search {{paket}}
```
#### Installiere ein Paket von Packagist:
```shell
cradle package install {{paket}}
```
#### Installiere eine bestimmte Version eines Pakets:
```shell
cradle package install {{paket}} {{version}}
```
#### Aktualisiere eine Paket:
```shell
cradle package update {{paket}}
```
#### Aktualisiere ein Paketes zu einer bestimmten Paket-Version:
```shell
cradle package update {{paket}} {{version}}
```
#### Entferne eine Paket:
```shell
cradle package remove {{paket}}
```
{% endraw %}{% raw %}
<h2 id="cradle-sql">
  <a href="/de/common/cradle-sql.html">cradle sql</a> <a href="#cradle-sql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Cradle SQL Datenbanken.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#sql>.

#### Generiere ein neues Datenbank-Schema:
```shell
cradle sql build
```
#### Generiere ein neues Datenbank-Schema f??r ein bestimmtes Paket:
```shell
cradle sql build {{paket}}
```
#### Entleere die gesamte Datenbank:
```shell
cradle sql flush
```
#### Entleere die Datenbank f??r ein bestimmtes Paket:
```shell
cradle sql flush {{paket}}
```
#### Bef??lle die Tabellen f??r alle Pakete:
```shell
cradle sql populate
```
#### Bef??lle die Tabellen f??r ein bestimmtes Paket:
```shell
cradle sql populate {{paket}}
```
{% endraw %}{% raw %}
<h2 id="cradle">
  <a href="/de/common/cradle.html">cradle</a> <a href="#cradle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Das Cradle PHP Framework.
> Siehe `cradle-install`, `cradle-deploy`, etc. f??r zus??tzliche Informationen.
> Weitere Informationen: <https://cradlephp.github.io>.

#### Stelle eine Verbindung zu einem Server her:
```shell
cradle connect {{server}}
```
#### Zeige die Hilfe-Seite an:
```shell
cradle help
```
#### Zeige die Hilfe-Seite f??r einen bestimmten Befehl:
```shell
cradle {{befehl}} help
```
#### F??hre einen Cradle-Befehl aus:
```shell
cradle {{befehl}}
```
{% endraw %}{% raw %}
<h2 id="csvsql">
  <a href="/de/common/csvsql.html">csvsql</a> <a href="#csvsql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiere SQL-Anweisungen f??r eine CSV-Datei oder f??hre diese Anweisungen direkt in einer Datenbank aus.
> Teil von csvkit.
> Weitere Informationen: <https://csvkit.readthedocs.io/en/latest/scripts/csvsql.html>.

#### Generiere eine `CREATE TABLE`-SQL-Anweisung f??r eine CSV-Datei:
```shell
csvsql {{pfad/zu/datei.csv}}
```
#### Importiere eine CSV-Datei in eine SQL-Datenbank:
```shell
csvsql --insert --db "{{mysql://benutzer:passwort@host/datenbank}}" {{pfad/zu/datei.csv}}
```
#### F??hre eine SQL-Abfrage auf einer CSV-Datei aus:
```shell
csvsql --query "{{select * from 'datei'}}" {{datei.csv}}
```
{% endraw %}{% raw %}
<h2 id="curl">
  <a href="/de/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??bertr??gt Daten von oder zu einem Server.
> Unterst??tzt die meisten Protokolle, inklusive HTTP, FTP und POP3.
> Weitere Informationen: <https://curl.se>.

#### Lade den Inhalt einer URL in eine Datei:
```shell
curl {{http://beispiel.de}} --output {{pfad/zu/datei}}
```
#### Lade eine Datei von einer URL herunter:
```shell
curl --remote-name {{http://beispiel.de/datei}}
```
#### Lade eine Datei herunter, folge Weiterleitungen und setze vergangene Dateitransfers automatisch fort:
```shell
curl --remote-name --location --continue-at - {{http://beispiel.de/datei}}
```
#### Sende formular-codierte Daten (POST Anfragen des Typs `application/x-www-form-urlencoded`). Benutze `--data @dateiname` oder `--data @'-'`, um von STDIN zu lesen:
```shell
curl --data {{'name=karl-dieter'}} {{http://beispiel.de/formular}}
```
#### Sende eine Anfrage mit einem extra Header mit einer eigenen HTTP-Methode:
```shell
curl --header {{'X-Mein-Header: 123'}} --request {{PUT}} {{http://beispiel.de}}
```
#### Sende Daten im JSON-Format und lege den geeigneten Inhaltstyp-Header fest:
```shell
curl --data {{'{"name":"karl-dieter"}'}} --header {{'Content-Type: application/json'}} {{http://beispiel.de/benutzer/1234}}
```
#### ??bergib einen Benutzernamen und Passwort f??r die Server-Authentifizierung:
```shell
curl --user benutzername:passwort {{http://beispiel.de}}
```
#### ??bergib Client-Zertifikat und -Schl??ssel f??r eine Resource und ??berspringe die Zertifikats??berpr??fung:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://beispiel.de}}
```
{% endraw %}{% raw %}
<h2 id="cut">
  <a href="/de/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Schneide Felder von stdin oder einer Datei aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/cut>.

#### Schneide die ersten 16 Zeichen jeder Zeile von stdin aus:
```shell
cut -c {{1-16}}
```
#### Schneide die ersten 16 Zeichen jeder Zeile der angegebenen Datei aus:
```shell
cut -c {{1-16}} {{pfad/zu/datei}}
```
#### Schneide alles ab dem dritten Zeichen bis zum Ende der Zeile aus:
```shell
cut -c {{3-}}
```
#### Schneide das f??nfte Feld jeder Zeile aus und nutze den Doppelpunkt als Trennzeichen (standardm????ig Tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Schneide das 2. und 10. Feld jeder Zeile aus und nutze Semikolon als Trennzeichen:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Schneide alles ab dem dritten Zeichen bis zum Ende der Zeile aus und nutze Leerzeichen als Trennzeichen:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}{% raw %}
<h2 id="dd">
  <a href="/de/common/dd.html">dd</a> <a href="#dd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konvertiere und kopiere eine Datei.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/dd>.

#### Erstelle ein bootbares USB-Laufwerk von einer isohybriden Datei (wie `archlinux-xxxx.iso`) und zeige den Fortschritt an:
```shell
dd if={{pfad/zu/datei.iso}} of=/dev/{{usb_drive}} status=progress
```
#### Klone ein USB-Laufwerk in ein anderes in 4MiB Bl??cken, ignoriere Fehler und zeige den Fortschritt an:
```shell
dd if=/dev/{{quell_laufwerk}} of=/dev/{{ziel_laufwerk}} bs=4M conv=noerror status=progress
```
#### Erstelle eine Datei mit 100 zuf??lligen Bytes mithilfe des Zufall-Treibers des Kernels:
```shell
dd if=/dev/urandom of={{pfad/zu/datei}} bs=100 count=1
```
#### Teste die Schreibgeschwindigkeit eines Laufwerks:
```shell
dd if=/dev/zero of={{pfad/zu/1GB_datei}} bs=1024 count=1000000
```
#### ??berpr??fe den Fortschritt eines laufenden dd-Prozsses (F??hre diesen Befehl von einer anderen Shell aus):
```shell
kill -USR1 $(pgrep ^dd)
```
{% endraw %}{% raw %}
<h2 id="diff">
  <a href="/de/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vergleiche Dateien und Verzeichnisse.
> Weitere Informationen: <https://man7.org/linux/man-pages/man1/diff.1.html>.

#### Vergleiche Dateien (Listet jene Ver??nderungen auf, mit denen `datei1` zu `datei2` wird):
```shell
diff {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und ignoriere Leerzeichen:
```shell
diff -w {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und zeige Unterschiede nebeneinander:
```shell
diff -y {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und zeige Unterschiede in vereinheitlichtem Format (wie in `git diff`):
```shell
diff -u {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Verzeichnisse rekursiv (zeigt sowohl Namen von unterschiedlichen Dateien/Verzeichnissen, als auch Unterschiede zwischen Dateien):
```shell
diff -r {{altes_verzeichnis}} {{neues_verzeichnis}}
```
#### Vergleiche Verzeichnisse und zeige nur die Namen der Dateien, die unterschiedlich sind:
```shell
diff -rq {{altes_verzeichnis}} {{neues_verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/de/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Docker Container und Images.
> Weitere Informationen: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Liste zur Zeit laufende Container auf:
```shell
docker ps
```
#### Liste laufende und gestoppte Container auf:
```shell
docker ps -a
```
#### Erzeuge einen Container aus einem Image und benenne ihn:
```shell
docker run --name {{container_name}} {{pfad/zu/image}}
```
#### Stoppe oder starte einen existierenden Container:
```shell
docker {{start|stop}} {{container_name}}
```
#### Lade ein Image herunter:
```shell
docker pull {{pfad/zu/image}}
```
#### ??ffne eine Konsole innerhalb eines bereits laufenden Containers:
```shell
docker exec -it {{container_name}} {{sh}}
```
#### L??sche einen gestoppten Container:
```shell
docker rm {{container_name}}
```
#### Zeige die Logs eines Containers an und aktualisiere sie automatisch:
```shell
docker logs -f {{container_name}}
```
{% endraw %}{% raw %}
<h2 id="dotnet">
  <a href="/de/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattform??bergreifende Kommandozeilenandwendungen f??r .NET Core.
> Weitere Informationen: <https://docs.microsoft.com/dotnet/core/tools/>.

#### Initialisiere ein neues .NET Projekt:
```shell
dotnet new {{vorlagen_name}}
```
#### Stelle nuget-Pakete wieder her:
```shell
dotnet restore
```
#### Baue des .NET Projekt im aktuellen Ordner und f??hre es aus:
```shell
dotnet run
```
#### F??hre eine gebaute dotnet-Applikation aus (Ben??tigt nur die Laufzeitumgebung. Die anderen Befehle ben??tigen auch den Entwicklungsteil):
```shell
dotnet {{pfad/zu/anwendung.dll}}
```
{% endraw %}{% raw %}
<h2 id="echo">
  <a href="/de/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib angegebene Argumente aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/echo>.

#### Gib einen Text aus. (Hinweis: Anf??hrungszeichen sind optional):
```shell
echo "{{Hallo Welt}}"
```
#### Gib einen Text mit Umgebungsvariablen aus:
```shell
echo "{{Liste aller Systempfade: $PATH}}"
```
#### Gib einen Text ohne darauffolgenden Zeilenumbruch aus:
```shell
echo -n "{{Hallo Welt}}"
```
#### F??ge einen Text in eine Datei ein:
```shell
echo "{{Hallo Welt}}" >> {{datei.txt}}
```
#### Erm??gliche Interpretation von Fluchtsymbolen (backslash escape):
```shell
echo -e "{{Spalte 1\tSpalte 2}}"
```
{% endraw %}{% raw %}
<h2 id="emacs">
  <a href="/de/common/emacs.html">emacs</a> <a href="#emacs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Der erweiterbare, ver??nderbare und selbst-dokumentierende Echtzeit Text Editor.
> Siehe auch `emacsclient`.
> Weitere Informationen: <https://www.gnu.org/software/emacs>.

#### ??ffne eine Datei in Emacs:
```shell
emacs {{pfad/zu/datei}}
```
#### ??ffne eine Datei in einer bestimmten Zeile:
```shell
emacs +{{zeilennummer}} {{pfad/zu/datei}}
```
#### Starte Emacs in der Konsole (ohne X-Fenster):
```shell
emacs --no-window-system
```
#### Starte einen Emacs-Server im Hintergrund (aufrufbar mit `emacsclient`):
```shell
emacs --daemon
```
#### Beende einen laufenden Emacs-Server und alle Instanzen und frage nach Best??tigung f??r ungespeicherte Dateien:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
#### Tastenkombination zum Speichern einer Datei:
```shell
Ctrl + X, Ctrl + S
```
#### Tastenkombination zum Beenden von Emacs:
```shell
Ctrl + X, Ctrl + C
```
{% endraw %}{% raw %}
<h2 id="emacsclient">
  <a href="/de/common/emacsclient.html">emacsclient</a> <a href="#emacsclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ffnet Dateien in einem laufenden Emacs-Server.
> Siehe auch `emacs`.
> Weitere Informationen: <https://www.emacswiki.org/emacs/EmacsClient>.

#### ??ffne eine Datei in einem laufenden Emacs-Server (mit GUI wenn m??glich):
```shell
emacsclient {{pfad/zu/datei}}
```
#### ??ffne eine Datei in der Konsole (ohne X-Fenster):
```shell
emacsclient --no-window-system {{pfad/zu/datei}}
```
#### ??ffne eine Datei in einem neuen Emacs Fenster:
```shell
emacsclient --create-frame {{pfad/zu/datei}}
```
#### F??hre einen Befehl aus und schreibe das Ergebnis in stdout:
```shell
emacsclient --eval '({{befehl}})'
```
#### Gib einen alternativen Editor an f??r den Fall, dass kein Emacs-Server l??uft:
```shell
emacsclient --alternate-editor {{editor}} {{pfad/zu/datei}}
```
#### Beende einen laufenden Emacs-Server und alle Instanzen und frage nach Best??tigung f??r ungespeicherte Dateien:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
{% endraw %}{% raw %}
<h2 id="exa">
  <a href="/de/common/exa.html">exa</a> <a href="#exa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein moderner Ersatz f??r `ls` (Verzeichnisinhalte auflisten).
> Weitere Informationen: <https://the.exa.website>.

#### Liste eine Datei pro Zeile auf:
```shell
exa --oneline
```
#### Liste alle Dateien auf, einschlie??lich versteckter Dateien:
```shell
exa --all
```
#### Liste alle Dateien im langen Format auf (Berechtigungen, Eigent??mer, Gr????e und ??nderungsdatum):
```shell
exa --long --all
```
#### Liste Dateien nach Gr????e absteigend sortiert auf:
```shell
exa --reverse --sort={{size}}
```
#### Zeige Dateien in einer Baumstruktur an, die drei Ebenen tief ist:
```shell
exa --long --tree --level={{3}}
```
#### Liste Dateien nach ??nderungsdatum aufsteigend sortiert auf:
```shell
exa --long --sort={{modified}}
```
{% endraw %}{% raw %}
<h2 id="fdroid">
  <a href="/de/common/fdroid.html">fdroid</a> <a href="#fdroid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid Build Tool.
> F-Droid ist ein installierbarer Katalog mit FOSS (Freie Open Source Software) Apps f??r Android.
> Weitere Informationen: <https://f-droid.org/>.

#### Kompiliere eine bestimmte App:
```shell
fdroid build {{app_id}}
```
#### Kompiliere eine bestimmte App in einer Build-Server-VM:
```shell
fdroid build {{app_id}} --server
```
#### Ver??ffentliche die App im lokalen Repository:
```shell
fdroid publish {{app_id}}
```
#### Installiere die App auf jedem verbundenen Ger??t:
```shell
fdroid install {{app_id}}
```
#### ??berpr??fe, ob die Metadaten korrekt formatiert sind:
```shell
fdroid lint --format {{app_id}}
```
#### Korrigiere die Formatierung automatisch (wenn m??glich):
```shell
fdroid rewritemeta {{app_id}}
```
{% endraw %}{% raw %}
<h2 id="fdroidcl">
  <a href="/de/common/fdroidcl.html">fdroidcl</a> <a href="#fdroidcl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid CLI (Command-line Interface) Client.
> Weitere Informationen: <https://github.com/mvdan/fdroidcl>.

#### Aktualisiere den Index:
```shell
fdroidcl update
```
#### Zeige Informationen ??ber eine App:
```shell
fdroidcl show {{app_id}}
```
#### Lade eine apk-Datei herunter:
```shell
fdroidcl download {{app_id}}
```
#### Suche nach einer App im Index:
```shell
fdroidcl search {{suchmuster}}
```
#### Installiere eine App auf einem verbundenen Ger??t:
```shell
fdroidcl install {{app_id}}
```
{% endraw %}{% raw %}
<h2 id="ffmpeg">
  <a href="/de/common/ffmpeg.html">ffmpeg</a> <a href="#ffmpeg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programm zum konvertieren von Videos.
> Weitere Informationen: <https://ffmpeg.org>.

#### Extrahiere den Ton eines Videos und speichere ihn als MP3:
```shell
ffmpeg -i {{pfad/zu/video.mp4}} -vn {{pfad/zu/audio.mp3}}
```
#### Konvertiere Frames eines Videos oder Gifs zu individuellen, numerierten Bildern:
```shell
ffmpeg -i {{video.mpg|video.gif}} {{pfad/zu/frame_%d.png}}
```
#### Kombiniere numerierte Bilder (`frame_1.jpg`, `frame_2.jpg`, etc) in ein Video oder Gif:
```shell
ffmpeg -i {{pfad/zu/frame_%d.jpg}} -f bild2 {{video.mpg|video.gif}}
```
#### Extrahiere einen einzelnen Frame von einem Video bei mm:ss and speichere als 128x128 Bild:
```shell
ffmpeg -ss {{mm:ss}} -i {{pfad/zu/video.mp4}} -frames 1 -s {{128x128}} -f bild2 {{pfad/zu/bild.png}}
```
#### Trimme ein Video von mm:ss bis mm2:ss2 (Ohne -to bis zum Ende des Videos):
```shell
ffmpeg -ss {{mm1:ss1}} -to {{mm2:ss2}} -i {{video.mp4}} -codec copy {{pfad/zu/output.mp4}}
```
#### Konvertiere ein AVI Video zu MP4. AAC Audio @ 128kbit, h264 Video @ CRF 23:
```shell
ffmpeg -i {{pfad/zu/input_video}}.avi -codec:audio aac -b:audio 128k -codec:video libx264 -crf 23 {{pfad/zu/output_video}}.mp4
```
#### Remuxe ein MKV Video zu MP4 ohne Audio oder Video streams neu zu codieren:
```shell
ffmpeg -i {{pfad/zu/input_video}}.mkv -codec copy {{pfad/zu/output_video}}.mp4
```
#### Konvertiere ein MP4 video zu VP9. F??r beste Qualit??t, nutze einen CRF Wert von 15 bis 35 und -b:video MUSS 0 sein:
```shell
ffmpeg -i {{pfad/zu/input_video}}.mp4 -codec:video libvpx-vp9 -crf {{30}} -b:video 0 -codec:audio libopus -vbr on -threads {{thread_anzahl}} {{pfad/zu/output_video}}.webm
```
{% endraw %}{% raw %}
<h2 id="ffprobe">
  <a href="/de/common/ffprobe.html">ffprobe</a> <a href="#ffprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multimedia Stream Analysierer.
> Weitere Informationen: <https://ffmpeg.org/ffprobe.html>.

#### Zeige alle verf??gbaren Stream-Informationen einer Medien-Datei an:
```shell
ffprobe -v error -show_entries {{datei.mp4}}
```
#### Zeige Spieldauer an:
```shell
ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die Bildfrequenz eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=avg_frame_rate -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die Breite (width) oder H??he (height) eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream={{width|height}} -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die durchschnittliche Bitrate eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=bit_rate -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
{% endraw %}{% raw %}
<h2 id="ffsend">
  <a href="/de/common/ffsend.html">ffsend</a> <a href="#ffsend"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Teile Dateien einfach und sicher in der Command-line.
> Weitere Informationen: <https://gitlab.com/timvisee/ffsend>.

#### Lade eine Datei hoch:
```shell
ffsend upload {{datei}}
```
#### Lade eine Datei herunter:
```shell
ffsend download {{url}}
```
#### Lade eine Datei mit Passwort hoch:
```shell
ffsend upload {{datei}} -p {{passwort}}
```
#### Lade eine passwortgesch??tzte Datei herunter:
```shell
ffsend download {{datei}} -p {{passwort}}
```
#### Lade eine Datei hoch und erlaube maximal 4 Downloads:
```shell
ffsend upload {{datei}} -d {{4}}
```
{% endraw %}{% raw %}
<h2 id="fg">
  <a href="/de/common/fg.html">fg</a> <a href="#fg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bringt Prozesse in den Vordergrund.
> Weitere Informationen: <https://manned.org/fg>.

#### Bringe zuletzt suspendierten Prozess in den Vordergrund:
```shell
fg
```
#### Bringe einen bestimmten Prozess in den Vordergrund:
```shell
fg %{{prozess_id}}
```
{% endraw %}{% raw %}
<h2 id="firefox">
  <a href="/de/common/firefox.html">firefox</a> <a href="#firefox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein gratis Open Source Internet Browser.
> Weitere Informationen: <https://developer.mozilla.org/en-US/docs/Mozilla/Command_Line_Options>.

#### Starte Firefox und ??ffne eine Website:
```shell
firefox {{https://www.duckduckgo.com}}
```
#### ??ffne ein neues Fenster:
```shell
firefox --new-window {{https://www.duckduckgo.com}}
```
#### ??ffne ein privates (Icognito) Fenster:
```shell
firefox --private-window
```
#### Suche nach "wikipedia" mit der Standard-Suchmaschine:
```shell
firefox --search "{{wikipedia}}"
```
#### Starte Firefox im sicheren Modus (alle Erweiterungen sind deaktiviert):
```shell
firefox --safe-mode
```
#### Erstelle eine Bildschirmaufnahme einer Website, ohne die GUI zu starten:
```shell
firefox --headless --screenshot {{pfad/zu/ausgabedatei.png}} {{https://beispiel.de/}}
```
#### Verwende ein bestimmtes Profil um mehrere einzelne Instanzen gleichzeitig laufen zu lassen:
```shell
firefox --profile {{pfad/zu/verzeichnis}} {{https://beispiel.de/}}
```
#### Lege Firefox als Standard-Browser fest:
```shell
firefox --setDefaultBrowser
```
{% endraw %}{% raw %}
<h2 id="fish">
  <a href="/de/common/fish.html">fish</a> <a href="#fish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Friendly Interactive SHell.
> Eine benutzerfreundliche Eingabeaufforderung.
> Weitere Informationen: <https://fishshell.com>.

#### Starte eine interaktive Shell-Sitzung:
```shell
fish
```
#### F??hre einen Befehl aus:
```shell
fish -c "{{befehl}}"
```
#### F??hre ein Skript aus:
```shell
fish {{pfad/zu/skript.fish}}
```
#### ??berpr??fe ein Skript auf Syntaxfehler:
```shell
fish --no-execute {{pfad/zu/skript.fish}}
```
#### Starte eine private interaktive Shell-Sitzung, in der `fish` weder auf die Shell-History zugreift, noch diese ver??ndert:
```shell
fish --private
```
#### Gib die Version von fish aus:
```shell
fish --version
```
#### Setze und exportiere eine permanente Umgebungsvariable (nur innerhalb der Shell):
```shell
set -Ux {{variablenname}} {{variablenwert}}
```
{% endraw %}{% raw %}
<h2 id="fortune">
  <a href="/de/common/fortune.html">fortune</a> <a href="#fortune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib ein zuf??lliges Gl??ckskeks-Zitat aus.
> Weitere Informationen: <https://man.archlinux.org/man/fortune.6>.

#### Gib ein Zitat aus:
```shell
fortune
```
#### Gib ein beleidigendes Zitat aus:
```shell
fortune -o
```
#### Gib ein langes Zitat aus:
```shell
fortune -l
```
#### Gib ein kurzes Zitat aus:
```shell
fortune -s
```
#### Gib alle verf??gbaren Zitat-Datenbank-Dateien aus:
```shell
fortune -f
```
#### Gib ein Zitat von einer durch `fortune -f` aufgelisteten Datenbank-Dateien aus:
```shell
fortune {{dateiname}}
```
{% endraw %}{% raw %}
<h2 id="fuck">
  <a href="/de/common/fuck.html">fuck</a> <a href="#fuck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Korrigiert den zuletzt ausgef??hrten Befehl.
> Weitere Informationen: <https://github.com/nvbn/thefuck>.

#### Lege den `fuck` alias f??r `thefuck` fest:
```shell
eval "$(thefuck --alias)"
```
#### Versuche den zuletzt ausgef??hrten Befehl zu korrigieren:
```shell
fuck
```
{% endraw %}{% raw %}
<h2 id="gplusplus">
  <a href="/de/common/g++.html">gplusplus</a> <a href="#gplusplus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere C++ Quelldateien.
> Teil der GCC (GNU Compiler Collection).
> Weitere Informationen: <https://gcc.gnu.org>.

#### Kompiliere eine Quelldatei in eine ausf??hrbare Bin??rdatei:
```shell
g++ {{quelldatei.cpp}} -o {{output_datei}}
```
#### Zeige (fast) alle Fehler und Warnungen an:
```shell
g++ {{quelldatei.cpp}} -Wall -o {{output_datei}}
```
#### W??hle einen Sprachstandard f??r das Kompilieren:
```shell
g++ {{quelldatei.cpp}} -std={{C++98|C++11|C++14|C++17}} -o {{output_datei}}
```
#### Binde Bibliotheken, die sich an einem anderen Pfad als die Quelldatei befinden mit ein:
```shell
g++ {{quelldatei.cpp}} -o {{output_datei}} -I{{header_pfad}} -L{{bibliotheks_pfad}} -l{{bibliotheks_name}}
```
{% endraw %}{% raw %}
<h2 id="gcc">
  <a href="/de/common/gcc.html">gcc</a> <a href="#gcc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pr??prozessiert und kompiliert C und C++ Quellcodedateien und linkt diese anschlie??end zusammen.
> Weitere Informationen: <https://gcc.gnu.org>.

#### Kompiliere mehrere Quellcodedateien zu einer ausf??hrbaren Datei:
```shell
gcc {{pfad/zu/datei1.c}} {{pfad/zu/datei2.c}} -o {{pfad/zu/bin??rdatei}}
```
#### Erlaube Warnungen und debug-Symbole in der Ausgabedatei:
```shell
gcc {{pfad/zu/datei.c}} -Wall -Og -o {{pfad/zu/bin??rdatei}}
```
#### Inkludiere Bibliotheken aus anderen Verzeichnissen:
```shell
gcc {{pfad/zu/datei.c}} -o {{pfad/zu/bin??rdatei}} -I{{pfad/zu/headerdatei}} -L{{pfad/zu/bibliothek1}} -l{{pfad/zu/bibliothek2}}
```
#### Kompiliere Quellcodedateien zu Assemblerinstruktionen:
```shell
gcc -S {{pfad/zu/datei.c}}
```
#### Kompiliere eine oder mehrere Quellcodedateien ohne diese zu linken:
```shell
gcc -c {{pfad/zu/datei.c}}
```
{% endraw %}{% raw %}
<h2 id="gdb">
  <a href="/de/common/gdb.html">gdb</a> <a href="#gdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Der GNU Debugger.
> Weitere Informationen: <https://www.gnu.org/software/gdb>.

#### Debugge eine ausf??hrbare Datei:
```shell
gdb {{ausf??hrbare_datei}}
```
#### Binde einen Prozess an gdb:
```shell
gdb -p {{prozess_ID}}
```
#### Debugge mit einer Kerndatei:
```shell
gdb -c {{kerndatei}} {{ausf??hrbare_datei}}
```
#### F??hre angegebene Befehle beim Start von gdb aus:
```shell
gdb -ex "{{befehle}}" {{ausf??hrbare_datei}}
```
#### Starte gdb und ??bergib Argumente an die ausf??hrbare Datei:
```shell
gdb --args {{ausf??hrbare_datei}} {{argument1}} {{argument2}}
```
{% endraw %}{% raw %}
<h2 id="git-add">
  <a href="/de/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F??ge Dateien zum Index/Stage hinzu.
> Weitere Informationen: <https://git-scm.com/docs/git-add>.

#### F??ge eine bestimmte Datei zum Index hinzu:
```shell
git add {{pfad/zu/datei}}
```
#### F??ge alle Dateien zum Index hinzu (nachverfolgte und nicht nachverfolgte):
```shell
git add -A
```
#### F??ge nur nachverfolgte Dateien zum Index hinzu (Updaten des Index):
```shell
git add -u
```
#### F??ge auch Dateien, welche ignoriert werden (`.gitignore`) hinzu:
```shell
git add -f
```
#### F??ge Teile von Dateien zum Index interaktiv hinzu:
```shell
git add -p
```
#### F??ge Teile einer bestimmten Datei interaktiv hinzu:
```shell
git add -p {{pfad/zu/datei}}
```
#### F??ge Dateien zum Index interaktiv hinzu:
```shell
git add -i
```
{% endraw %}{% raw %}
<h2 id="git-am">
  <a href="/de/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Patch-Dateien integrieren. N??tzlich beim Empfang von Commits per E-Mail.
> Siehe auch `git format-patch` zur Erzeugung von Patch-Dateien.
> Weitere Informationen: <https://git-scm.com/docs/git-am>.

#### Integriere eine Patch-Datei:
```shell
git am {{pfad/zu/datei.patch}}
```
#### Brich das Integrieren einer Patch-Datei ab:
```shell
git am --abort
```
#### Integriere so viele Patch-Dateien wie m??glich und speichere fehlgeschlagene Teile:
```shell
git am --reject {{pfad/zu/datei.patch}}
```
{% endraw %}{% raw %}
<h2 id="git-apply">
  <a href="/de/common/git-apply.html">git apply</a> <a href="#git-apply"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Integriere eine Patch-Datei und/oder f??ge sie zum Index hinzu.
> Weitere Informationen: <https://git-scm.com/docs/git-apply>.

#### Gib Informationen ??ber gepatchte Dateien aus:
```shell
git apply --verbose {{pfad/zu/datei}}
```
#### Integriere die Patch-Datei und f??ge sie zum Index hinzu:
```shell
git apply --index {{pfad/zu/datei}}
```
#### Integriere eine externe Patch-Datei:
```shell
curl {{https://beispiel.de/datei.patch}} | git apply
```
#### Gib diffstat des Inputs aus und integriere die Patch-Datei:
```shell
git apply --stat --apply {{pfad/zu/datei}}
```
#### Integriere eine Patch-Datei in umgekehrter Reihenfolge:
```shell
git apply --reverse {{pfad/zu/datei}}
```
#### Speichere das Ergebnis einer Patch-Datei im Index, ohne den Arbeitsbaum zu ver??ndern:
```shell
git apply --cache {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="git-archive">
  <a href="/de/common/git-archive.html">git archive</a> <a href="#git-archive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle ein Archiv von Dateien.
> Weitere Informationen: <https://git-scm.com/docs/git-archive>.

#### Erstelle ein tar-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:
```shell
git archive --verbose HEAD
```
#### Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:
```shell
git archive --verbose --format=zip HEAD
```
#### Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und speichere dieses in eine Datei:
```shell
git archive --verbose --output={{pfad/zu/datei.zip}} HEAD
```
#### Erstelle ein tar-Archiv aus dem Inhalt des letzten Commits eines bestimmten Branches:
```shell
git archive --output={{pfad/zu/datei.tar}} {{branch_name}}
```
#### Erstelle ein tar-Archiv aus dem Inhalt eines bestimmten Verzeichnisses:
```shell
git archive --output={{pfad/zu/datei.tar}} HEAD:{{pfad/zu/verzeichnis}}
```
#### Stelle jeder Datei einen Pfad voran, um sie in einem bestimmten Verzeichnis zu archivieren:
```shell
git archive --output={{pfad/zu/datei.tar}} --prefix={{pfad/zu/verzeichnis}}/ HEAD
```
{% endraw %}{% raw %}
<h2 id="git-bisect">
  <a href="/de/common/git-bisect.html">git bisect</a> <a href="#git-bisect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Benuzt bin??re Suche um den commit ausfindig zu machen, welcher einen Fehler beinhaltet.
> Git springt im Commit-Graph automatisch vor und zur??ck, um den fehlerhaften Commit schrittweise einzugrenzen zu k??nnen.
> Weitere Informationen: <https://git-scm.com/docs/git-bisect>.

#### Starte eine Bisect-Session in einem Commit-Bereich, der durch einen bekannten fehlerhaften Commit und einen sauberen Commit begrenzt wird:
```shell
git bisect start {{fehlerhafter_commit}} {{sauberer_commit}}
```
#### Pr??fe jeden Commit, den `git bisect` ausw??hlt, und kennzeichne ihn mit "gut" oder "schlecht":
```shell
git bisect {{good|bad}}
```
#### Wechsle zum vorherigen Branch zur??ck, nachdem der fehlerhafte Commit lokalisiert wurde:
```shell
git bisect reset
```
#### ??berspringe einen Commit w??hrend der Bisect-Session (z.B. einen, der die Tests aufgrund eines anderen Problems nicht bestanden hat):
```shell
git bisect skip
```
{% endraw %}{% raw %}
<h2 id="git-blame">
  <a href="/de/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige den Commit-Hash und den letzten Autor jeder Zeile einer Datei.
> Weitere Informationen: <https://git-scm.com/docs/git-blame>.

#### Gib die Commit-Hashes und dem Autor jeder Zeile einer Datei aus:
```shell
git blame {{pfad/zu/datei}}
```
#### Gib die Commit-Hashes und dem Autor (inklusive Email) jeder Zeile einer Datei aus:
```shell
git blame -e {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="git-branch">
  <a href="/de/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte und Arbeite mit Git Branches.
> Weitere Informationen: <https://git-scm.com/docs/git-branch>.

#### Liste alle lokalen Branches auf. Der momentan aktive (ausgecheckte) Branch wird mit `*` markiert:
```shell
git branch
```
#### Liste alle Branches auf (Lokal und Remote):
```shell
git branch -a
```
#### Zeige den Namen des aktuellen Branches:
```shell
git branch --show-current
```
#### Erstelle einen neuen Branch auf Basis des letzten Commits:
```shell
git branch {{branch_name}}
```
#### Erstelle einen neuen Branch auf Basis eines bestimmten Commits:
```shell
git branch {{branch_name}} {{commit_hash}}
```
#### Benenne einen Branches um (der Branch muss nicht ausgecheckt sein):
```shell
git branch -m {{alter_branch_name}} {{neuer_branch_name}}
```
#### L??sche einen lokalen Branch (der Branch muss nicht ausgecheckt sein):
```shell
git branch -d {{branch_name}}
```
#### L??sche einen remote-Branch:
```shell
git push {{remote_name}} --delete {{remote_branch_name}}
```
{% endraw %}{% raw %}
<h2 id="git-clone">
  <a href="/de/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Klone ein existierendes Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-clone>.

#### Klone ein existierendes Repository:
```shell
git clone {{url_zu_repository}}
```
#### Klone ein existierendes Repository in ein bestimmtes Verzeichnis:
```shell
git clone {{url_zu_repository}} {{pfad/zu/verzeichnis}}
```
#### Klone ein existierendes Repository und seine Submodule:
```shell
git clone --recursive {{url_zu_repository}}
```
#### Klone ein lokales Repository:
```shell
git clone -l {{pfad/zu/lokalem_repository}}
```
#### Klone ohne Meldungen:
```shell
git clone -q {{url_zu_repository}}
```
#### Klone ein existierendes Repository und rufe nur die neuesten 10 Commits im Standard-Branch ab (spart Zeit):
```shell
git clone --depth {{10}} {{url_zu_repository}}
```
#### Klone ein existierendes Repository, aber lade nur einen bestimmten Branch herunter:
```shell
git clone --branch {{name}} --single-branch {{url_zu_repository}}
```
{% endraw %}{% raw %}
<h2 id="git-commit">
  <a href="/de/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Committe Dateien in ein Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-commit>.

#### Committe gestagten Dateien zum Repository mit einer Nachricht:
```shell
git commit -m "{{nachricht}}"
```
#### Committe alle gestagten Dateien zum Repository mit einer Nachricht aus einer Datei:
```shell
git commit --file {{pfad/zu/commit_nachricht_datei}}
```
#### Stage alle modifizierten Dateien und committe sie mit einer Nachricht:
```shell
git commit -a -m "{{nachricht}}"
```
#### Ersetze den letzten Commit mit den gerade auf dem Stage liegenden ??nderungen:
```shell
git commit --amend
```
#### Comitte nur spezifische Dateien (die Dateien m??ssen schon auf dem Stage liegen):
```shell
git commit {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
{% endraw %}{% raw %}
<h2 id="git-fetch">
  <a href="/de/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade Objekte und Referenzen (refs) von einem entfernten Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-fetch>.

#### Hole die neuesten ??nderungen von dem standardm????igen Repository im Upstream (wenn gesetzt):
```shell
git fetch
```
#### Hole neue Branches von einem bestimmten Repository im Upstream:
```shell
git fetch {{name_des_upstream_repository}}
```
#### Hole die neuesten ??nderungen von allen Repositories im Upstream:
```shell
git fetch --all
```
#### Lade auch die Tags des Repository im Upstream:
```shell
git fetch --tags
```
#### L??sche lokale Referenzen auf entfernte Branches, die im Upstream-Repository nicht mehr existieren:
```shell
git fetch --prune
```
{% endraw %}{% raw %}
<h2 id="git-help">
  <a href="/de/common/git-help.html">git help</a> <a href="#git-help"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Hilfe f??r Git an.
> Weitere Informationen: <https://git-scm.com/docs/git-help>.

#### Zeige Hilfe f??r einen bestimmten Git-Unterbefehl an:
```shell
git help {{unterbefehl}}
```
#### Zeige Hilfe f??r einen bestimmten Git-Unterbefehl im Web-Browser an:
```shell
git help --web {{unterbefehl}}
```
#### Zeige eine Liste von allen verf??gbaren Git-Unterbefehlen an:
```shell
git help --all
```
#### Liste die verf??gbaren Handb??cher auf:
```shell
git help --guide
```
#### Liste alle Konfigurationsvariablen auf:
```shell
git help --config
```
{% endraw %}{% raw %}
<h2 id="git-ignore-io">
  <a href="/de/common/git-ignore-io.html">git ignore-io</a> <a href="#git-ignore-io"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle `.gitignore` Dateien aus vorgefertigten Vorlagen.
> Weitere Informationen: <https://github.com/tj/git-extras/blob/master/Commands.md#git-ignore-io>.

#### Liste alle verf??gbaren Vorlagen auf:
```shell
git ignore-io list
```
#### Erstelle eine `.gitignore` Vorlage:
```shell
git ignore-io {{eintrag_a,eintrag_b,eintrag_n}}
```
{% endraw %}{% raw %}
<h2 id="git-init">
  <a href="/de/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle eine neues lokales Git-Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-init>.

#### Erstelle eine neues lokales Repository:
```shell
git init
```
#### Erstelle ein neues Repository, welches SHA256 f??r Objekt-Hashes verwendet (ben??tigt Git 2.29+):
```shell
git init --object-format={{sha256}}
```
#### Erstelle eine neues minimales Repository, welches sich f??r die Verwendung als Remote-Repository ??ber SSH eignet:
```shell
git init --bare
```
{% endraw %}{% raw %}
<h2 id="git-log">
  <a href="/de/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeigt die Commit-Historie an.
> Weitere Informationen: <https://git-scm.com/docs/git-log>.

#### Zeige die Sequenz der Commits des Git-Repository im aktuellen Verzeichnis, beginnend mit dem aktuellen, an.
```shell
git log
```
#### Zeige die Historie einer bestimmten Datei oder eines Verzeichnisses, inklusive Unterschiede, an:
```shell
git log -p {{pfad/zu/datei_oder_verzeichnis}}
```
#### Zeige einen ??berblick der Commits an und welche Dateien jeweils ver??ndert wurden:
```shell
git log --stat
```
#### Zeige einen Graphen von Commits im aktuellen Branch, wobei jeweils nur die erste Zeile der Commit-Nachricht angezeigt wird:
```shell
git log --oneline --graph
```
#### Zeige einen Graphen von allen Commits, Tags und Branches im gesamten Repository:
```shell
git log --oneline --decorate --all --graph
```
#### Zeige nur Commits, deren Commit-Nachricht einen bestimmten Text enthalten (Ohne Beachtung von Gro??- und Kleinschreibung):
```shell
git log -i --grep {{text}}
```
#### Zeige die letzten N Commits eines bestimmten Autors:
```shell
git log -n {{anzahl}} --author={{autor}}
```
#### Zeige alle Commits zwischen zwei Zeitpunkten an:
```shell
git log --before={{datum}} --after={{datum}}
```
{% endraw %}{% raw %}
<h2 id="git-pull">
  <a href="/de/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hole Branches von einem entfernten Repository und binde sie in das lokale Repository ein.
> Weitere Informationen: <https://git-scm.com/docs/git-pull>.

#### Lade ??nderungen vom Standard-Repository herunter und f??hre diese zusammen:
```shell
git pull
```
#### Lade ??nderungen vom Standard-Repository herunter und wende einen Rebase an:
```shell
git pull --rebase
```
#### Lade ??nderungen vom Standard-Repository herunter und f??hre diese in den HEAD zusammen:
```shell
git pull {{remote_name}} {{branch}}
```
{% endraw %}{% raw %}
<h2 id="git-push">
  <a href="/de/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade Commits in ein Remote-Repository hoch.
> Weitere Informationen: <https://git-scm.com/docs/git-push>.

#### Sende lokale ??nderungen des aktuellen Branches zu seinem entfernten Repository (Remote Branch):
```shell
git push
```
#### Sende lokale ??nderungen des angegebenen Branches zu seinem entfernten Repository:
```shell
git push {{remote_name}} {{lokaler_branch}}
```
#### Lade den aktuellen Branches in ein entferntes Repository mit Angabe des Namens des entfernten Branches hoch:
```shell
git push {{remote_name}} -u {{remote_branch}}
```
#### Lade ??nderungen aller lokalen Branches zu ihrem entfernten Repository hoch:
```shell
git push --all {{remote_name}}
```
#### L??sche einen Branches in einem entfernten Repository:
```shell
git push {{remote_name}} --delete {{remote_branch}}
```
#### Entferne alle remote Branches, welche kein lokales Gegenst??ck besitzen:
```shell
git push --prune {{remote_name}}
```
#### Ver??ffentliche Tags, welche noch nicht im entfernten Repository vorhanden sind:
```shell
git push --tags
```
{% endraw %}{% raw %}
<h2 id="git-remote">
  <a href="/de/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte eine gewisse Anzahl an Repositories (remotes).
> Weitere Informationen: <https://git-scm.com/docs/git-remote>.

#### Liste alle existierenden Remotes, ihre Namen und ihre URLs auf:
```shell
git remote -v
```
#### Zeige Informationen ??ber ein Remote an:
```shell
git remote show {{remote_name}}
```
#### F??ge ein neues Remote hinzu:
```shell
git remote add {{remote_name}} {{remote_url}}
```
#### ??ndere die URL eines Remotes (benutze `--add` um die existierende URL zu behalten):
```shell
git remote set-url {{remote_name}} {{remote_url}}
```
#### Entferne ein Remote:
```shell
git remote remove {{remote_name}}
```
#### Benenne ein Remote um:
```shell
git remote rename {{alter_name}} {{neuer_name}}
```
{% endraw %}{% raw %}
<h2 id="git-rm">
  <a href="/de/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Entferne Dateien aus dem Index des Repositories und vom lokalen Dateisystem.
> Weitere Informationen: <https://git-scm.com/docs/git-rm>.

#### Entferne eine Datei aus dem Index und vom lokalen Dateisystem:
```shell
git rm {{pfad/zu/datei}}
```
#### Entferne ein Verzeichnis:
```shell
git rm -r {{pfad/zu/verzeichnis}}
```
#### Entferne eine Datei aus dem Index des Repositories, aber behalte sie lokal:
```shell
git rm --cached {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="git-status">
  <a href="/de/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige die ??nderungen an Dateien in einem Git-Repository an.
> Weitere Informationen: <https://git-scm.com/docs/git-status>.

#### Zeige ver??nderte Dateien an, die noch nicht f??r den Commit hinzugef??gt wurden:
```shell
git status
```
#### Zeige eine kurze Version an:
```shell
git status -s
```
#### Zeige nur verfolgte (getrackte) Dateien an:
```shell
git status --untracked-files=no
```
#### Zeige eine kurze Version mit zus??tzlichen Informationen ??ber den Branch an:
```shell
git status -sb
```
{% endraw %}{% raw %}
<h2 id="git-switch">
  <a href="/de/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wechsle zwischen Branches. Verf??gbar ab Git Version 2.23+.
> Siehe auch `git checkout`.
> Weitere Informationen: <https://git-scm.com/docs/git-switch>.

#### Wechsle zu einem existierenden Branch:
```shell
git switch {{branche_name}}
```
#### Erstelle einen neuen Branch und wechsele zu diesem:
```shell
git switch --create {{branch_name}}
```
#### Erstelle einen neuen Branch basierend auf einem existierenden Commit und wechsele zu diesem:
```shell
git switch --create {{branch_name}} {{commit}}
```
#### Wechsele zum vorherigen Branch:
```shell
git switch -
```
#### Wechsele zu einem Branch und aktualisiere alle Submodule entsprechend:
```shell
git switch --recurse-submodules {{branch_name}}
```
#### Wechsele zu einem Branch und merge automatisch den aktuellen Branch und alle ??nderungen, die nicht committed wurden:
```shell
git switch --merge {{branch_name}}
```
{% endraw %}{% raw %}
<h2 id="git-tag">
  <a href="/de/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle, l??sche, ??berpr??fe und liste Tags auf.
> Weitere Informationen: <https://git-scm.com/docs/git-tag>.

#### Liste alle Tags auf:
```shell
git tag
```
#### Erstelle einen Tag mit Namen, welcher auf den aktuellen Commit zeigt:
```shell
git tag {{tag_name}}
```
#### Erstelle einen Tag mit Namen, welcher auf einen bestimmten Commit zeigt:
```shell
git tag {{tag_name}} {{commit}}
```
#### Erstelle einen Tag mit Anmerkung:
```shell
git tag {{tag_name}} -m {{anmkerung}}
```
#### L??sche einen Tag mit bestimmten Namen:
```shell
git tag -d {{tag_name}}
```
#### Lade die aktualisierten Tags aus dem Upstream:
```shell
git fetch --tags
```
#### Liste alle Tags auf, bei denen sich in den vorangegangenen Commits ein bestimmter Commit findet:
```shell
git tag --contains {{commit}}
```
{% endraw %}{% raw %}
<h2 id="git">
  <a href="/de/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verteiltes Versionskontrollsystem.
> Weitere Informationen: <https://git-scm.com/>.

#### Gib die installierte Git Version aus:
```shell
git --version
```
#### Zeige die generelle Hilfsseite an:
```shell
git --help
```
#### Zeige die Hilfsseite eines Unterbefehls an:
```shell
git help {{unterbefehl}}
```
#### F??hre einen Git-Unterbefehl aus:
```shell
git {{unterbefehl}}
```
#### F??hre einen Git-Unterbefehl auf einem benutzerdefinierten Repository aus:
```shell
git -C {{pfad/zu/repository}} {{unterbefehl}}
```
#### F??hre einen Git-Unterbefehl mit der angegebenen Konfiguration aus:
```shell
git -c '{{config.key}}={{wert}}' {{unterbefehl}}
```
{% endraw %}{% raw %}
<h2 id="gpg">
  <a href="/de/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard.
> Weitere Informationen: <https://gnupg.org>.

#### Signiere `doc.txt` ohne Verschl??sselung (Ausabe nach `doc.txt.asc`):
```shell
gpg --clearsign {{doc.txt}}
```
#### Verschl??ssle `doc.txt` f??r alice@beispiel.de (Ausgabe nach `doc.txt.gpg`):
```shell
gpg --encrypt --recipient {{alice@beispiel.de}} {{doc.txt}}
```
#### Verschl??ssle `doc.txt` nur mit Passwort (Ausgabe nach `doc.txt.gpg`):
```shell
gpg --symmetric {{doc.txt}}
```
#### Entschl??ssle `doc.txt.gpg` (Ausgabe nach stdout):
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### Importiere einen ??ffentlichen Schl??ssel:
```shell
gpg --import {{schl??ssel.gpg}}
```
#### Exportiere den ??ffentlichen Schl??ssel von alice@beispiel.de (Ausgabe nach stdout):
```shell
gpg --export --armor {{alice@beispiel.de}}
```
#### Exportiere den privaten Schl??ssel von alice@beispiel.de (Ausgabe nach stdout):
```shell
gpg --export-secret-keys --armor {{alice@beispiel.de}}
```
{% endraw %}{% raw %}
<h2 id="gpg2">
  <a href="/de/common/gpg2.html">gpg2</a> <a href="#gpg2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard 2.
> Siehe `gpg` f??r GNU Privacy Guard 1.
> Weitere Informationen: <https://docs.releng.linuxfoundation.org/en/latest/gpg.html>.

#### Liste alle importierten Schl??ssel auf:
```shell
gpg2 --list-keys
```
#### Verschl??ssle eine bestimme Datei f??r einen bestimmten Empf??nger und schreibe den Output in eine neue `.gpg` Datei:
```shell
gpg2 --encrypt --recipient {{hans@beispiel.de}} {{pfad/zu/datei.txt}}
```
#### Verschl??ssle eine bestimmte Datei nur mit einem Passwort und schreibe den Output in eine neue `.gpg` Datei:
```shell
gpg2 --symmetric {{pfad/zu/datei.txt}}
```
#### Verschl??ssle eine bestimmte Datei und schreibe des Ergebnis auf STDOUT:
```shell
gpg2 --decrypt {{pfad/zu/datei.txt.gpg}}
```
#### Importiere einen ??ffentlichen Schl??ssel:
```shell
gpg2 --import {{pfad/zu/??ffentlichem_schl??ssel.gpg}}
```
#### Exportiere den ??ffentlichen Schl??ssel einer bestimmten Email-Adresse nach STDOUT:
```shell
gpg2 --export --armor {{hans@beispiel.de}}
```
#### Exportiere den privaten Schl??ssel einer bestimmten Email-Adresse nach STDOUT:
```shell
gpg2 --export-secret-keys --armor {{hans@beispiel.de}}
```
{% endraw %}{% raw %}
<h2 id="grep">
  <a href="/de/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Findet Ausdr??cke in einem Eingabetext.
> Unterst??tzt einfache Muster und regul??re Ausdr??cke.
> Weitere Informationen: <https://www.gnu.org/software/grep/manual/grep.html>.

#### Suche nach einem Ausdruck in einer Datei:
```shell
grep {{ausdruck}} {{pfad/zu/datei}}
```
#### Suche nach einem exakten Ausdruck:
```shell
grep -F {{exakter_ausdruck}} {{pfad/zu/datei}}
```
#### Suche nach Ausdr??cken [R]ekursiv im aktuellen Verzeichnis, zeige zugeh??rige Zeilen[n]ummern und [I]gnoriere Bin??rdateien:
```shell
grep -RIn {{ausdruck}} .
```
#### Benutze erweiterte regul??re Ausdr??cke (unterst??tzt `?`, `+`, `{}`, `()` und `|`) ohne Beachtung der Gro??-, Kleinschreibung:
```shell
grep -Ei {{ausdruck}} {{pfad/zu/datei}}
```
#### Zeige 3 Zeilen Kontext um [C], vor [B] oder nach [A] jedem Ergebnis:
```shell
grep -{{C|B|A}} 3 {{ausdruck}} {{pfad/zu/datei}}
```
#### Gib den Dateinamen mit zugeh??riger Zeilennummer f??r jedes Ergebnis aus:
```shell
grep -Hn {{ausdruck}} {{pfad/zu/datei}}
```
#### Benutze STDIN, anstatt einer Datei:
```shell
echo "input" | grep {{ausdruck}}
```
#### In[v]ertiere das Ergebnis um bestimmte Ausdr??cke auszuschlie??en:
```shell
grep -v {{ausdruck}}
```
{% endraw %}{% raw %}
<h2 id="latex">
  <a href="/de/common/latex.html">latex</a> <a href="#latex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine LaTeX Quelldatei in ein DVI Dokument.
> Weitere Informationen: <https://www.latex-project.org>.

#### Kompiliere ein DVI Dokument:
```shell
latex {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
latex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und stoppe bei jedem Fehler:
```shell
latex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}{% raw %}
<h2 id="less">
  <a href="/de/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ffne eine Datei f??r interaktives lesen, erlaubt scrollen und suchen.

#### ??ffne eine Datei:
```shell
less {{pfad/zu/datei}}
```
#### Scrolle eine Seite runter / hoch:
```shell
<Leertaste> (runter), b (hoch)
```
#### Springe zum Ende / Anfang der Datei:
```shell
G (Ende), g (Anfang)
```
#### Suche nach einer Zeichenkette forw??rts (n/N um zur n??chsten/vorherigen ??bereinstimmung zu springen):
```shell
/{{suche}}
```
#### Suche nach einer Zeichenkette r??ckw??rts (n/N um zur n??chsten/vorherigen ??bereinstimmung zu springen):
```shell
?{{suche}}
```
#### Folge der Ausgabe des ge??ffeten Buffers:
```shell
F
```
#### ??ffne die Datei in einem Editor:
```shell
v
```
#### Beende `less`:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="lolcat">
  <a href="/de/common/lolcat.html">lolcat</a> <a href="#lolcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F??rbe Text in Regenbogenfarben ein.
> Weitere Informationen: <https://github.com/busyloop/lolcat>.

#### Gib den Inhalt einer Datei in Regenbogenfarben in der Konsole aus:
```shell
lolcat {{pfad/zu/datei}}
```
#### Gib die Ausgabe eines Befehls in Regenbogenfarben in der Konsole aus:
```shell
{{fortune}} | lolcat
```
#### Gib den Inhalt einer Datei in animierten Regenbogenfarben in der Konsole aus:
```shell
lolcat -a {{pfad/zu/datei}}
```
#### Gib den Inhalt einer Datei in 24-bit (truecolor) Regenbogenfarben in der Konsole aus:
```shell
lolcat -t {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/de/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Liste den Inhalt eines Verzeichnisses auf.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/ls>.

#### Liste den Inhalt in einer Datei pro Zeile auf:
```shell
ls -1
```
#### Liste alle Dateien inklusive versteckter Dateien auf:
```shell
ls -a
```
#### Liste alle Dateien mit einem abschlie??enden `/` bei Verzeichnis-Namen auf:
```shell
ls -F
```
#### Liste alle Dateien mit Berechtigungen, Besitzer, Gr????e und ??nderungsdatum auf:
```shell
ls -la
```
#### Liste alle Dateien mit Dateigr????e in f??r Menschen lesbaren Einheiten (KiB, MiB, GiB):
```shell
ls -lh
```
#### Liste Dateien nach sortiert nach Dateigr????e mit gr????ter beginnend auf:
```shell
ls -lS
```
#### Liste alle Dateien sortiert nach dem ??nderungsdatum mit ??ltester beginnend auf:
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="minisign">
  <a href="/de/common/minisign.html">minisign</a> <a href="#minisign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein denkbar einfaches Werkzeug um Dateien zu signieren und Signaturen zu verifizieren.
> Weitere Informationen: <https://jedisct1.github.io/minisign/>.

#### Generiere ein neues Schl??sselpaar im Standardpfad:
```shell
minisign -G
```
#### Signiere eine Datei:
```shell
minisign -Sm {{pfad/zu/datei}}
```
#### Signiere eine Datei und f??ge dabei einen vertrauensw??rdigen (signierten) und einen nicht vertrauensw??rdigen (unsignierten) Kommentar in der Signatur an:
```shell
minisign -Sm {{pfad/zu/datei}} -c "{{Nicht vertrauensw??rdiger Kommentar}}" -t "{{Vertrauensw??rdiger Kommentar}}"
```
#### Verifiziere eine Datei und die vertrauensw??rdigen Kommentare in ihrer Signatur gegen die angegebene Datei mit dem ??ffentlichen Schl??ssel:
```shell
minisign -Vm {{pfad/zu/datei}} -p {{pfad/zu/??ffentlicher_schl??ssel.pub}}
```
#### Verifiziere eine Datei und die vertrauensw??rdigen Kommentare in ihrer Signatur gegen den angegebenen, in Base64 codierten ??ffentlichen Schl??ssel:
```shell
minisign -Vm {{pfad/zu/datei}} -P "{{??ffentlicher_schl??ssel_base64}}"
```
{% endraw %}{% raw %}
<h2 id="mv">
  <a href="/de/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verschiebe Dateien oder Verzeichnisse oder benenne diese um.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/mv>

#### Verschiebe eine Dateien an einen beliebigen Ort:
```shell
mv {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### ??berschreibe bereits existierende Dateien ohne vorherige Best??tigung:
```shell
mv -f {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### ??berschreibe bereits existierende Dateien nach Best??tigung (unabh??ngig von Dateirechten):
```shell
mv -i {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Verhindere das ??berschreiben existierender Dateien am Zielort:
```shell
mv -n {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Liste Dateien und deren Details auf w??hrend sie verschoben werden:
```shell
mv -v {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
{% endraw %}{% raw %}
<h2 id="nativefier">
  <a href="/de/common/nativefier.html">nativefier</a> <a href="#nativefier"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Befehlszeilen-Tool zum Erstellen einer Desktop-Anwendung f??r jede Website mit minimaler Konfiguration.
> Weitere Informationen: <https://github.com/jiahaog/nativefier>.

#### Erstelle einer Desktop-Anwendung f??r eine Website:
```shell
nativefier {{url}}
```
#### Erstelle eine Desktop-Anwendung mit einem benutzerdefinierten Namen:
```shell
nativefier --name {{name}} {{url}}
```
#### Verwende ein benutzerdefiniertes Icon:
```shell
nativefier --icon {{pfad/zu/icon.png}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="npm">
  <a href="/de/common/npm.html">npm</a> <a href="#npm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Kommandozeilenwerkzeug f??r die Verwaltung von JavaScript und Node.js Paketen (Packages).
> Weitere Informationen: <https://www.npmjs.com>.

#### Erstelle eine `package.json` Datei interaktiv:
```shell
npm init
```
#### Installiere alle in der `package.json` Datei gelisteten Abh??ngigkeiten:
```shell
npm install
```
#### Installiere eine spezifische Version eines Packages und f??ge es automatisch der `package.json` Datei hinzu:
```shell
npm install {{package_name}}@{{version}}
```
#### Installiere ein Package und f??ge es als Entwicklungs-Abh??ngigkeit der `package.json` Datei hinzu:
```shell
npm install {{package_name}} --save-dev
```
#### Installiere ein Package global:
```shell
npm install --global {{package_name}}
```
#### Deinstalliere ein Package und entferne es automatisch aus der `package.json` Datei:
```shell
npm uninstall {{package_name}}
```
#### Gib eine Liste aller lokal installierten Packages aus:
```shell
npm list
```
#### Gib eine Liste aller global installierten Packages aus:
```shell
npm list --global --depth={{0}}
```
{% endraw %}{% raw %}
<h2 id="pass">
  <a href="/de/common/pass.html">pass</a> <a href="#pass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programm zum Speichern und Lesen von Passw??rtern und anderen sensiblen Daten.
> Die Daten sind mit GPG verschl??sselt und werden mit einem Git repository verwaltet.
> Weitere Informationen: <https://www.passwordstore.org>.

#### Initialisiere oder verschl??ssle einen neuen oder bestehenden Speicher mit einer oder mehreren GPG IDs neu:
```shell
pass init {{gpg_id_1}} {{gpg_id_2}}
```
#### Speichere das Passwort und zus??tzliche Informationen (Str + D auf neuer Zeile zum abschlie??en):
```shell
pass insert --multiline {{pfad/zu/datei}}
```
#### Bearbeite einen bestimmten Eintrag:
```shell
pass edit {{pfad/zu/datei}}
```
#### Kopiere das Passwort (die erste Zeile des Eintrags) in die Zwischenablage:
```shell
pass -c {{pfad/zu/datei}}
```
#### Zeige die Baumstruktur des Passwort-Stores an:
```shell
pass
```
#### Generiere ein neues, zuf??lliges Passwort mit L??nge n und kopiere is in die Zwischenablage:
```shell
pass generate -c {{pfad/zu/datei}} {{n}}
```
#### Initialisiere ein Git Repository (Alle durch pass durchgef??hrten ??nderungen werden automatisch committed):
```shell
pass git init
```
{% endraw %}{% raw %}
<h2 id="pdflatex">
  <a href="/de/common/pdflatex.html">pdflatex</a> <a href="#pdflatex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine LaTeX Quelldatei in ein PDF Dokument.
> Weitere Informationen: <https://manned.org/pdflatex>.

#### Kompiliere ein PDF Dokument:
```shell
pdflatex {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
pdflatex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und stoppe bei jedem Fehler:
```shell
pdflatex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}{% raw %}
<h2 id="pdftex">
  <a href="/de/common/pdftex.html">pdftex</a> <a href="#pdftex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine TeX Quelldatei in ein PDF Dokument.
> Weitere Informationen: <https://www.tug.org/applications/pdftex/>.

#### Kompiliere ein PDF Dokument:
```shell
pdftex {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
pdftex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und stoppe bei jedem Fehler:
```shell
pdftex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}{% raw %}
<h2 id="phpbu">
  <a href="/de/common/phpbu.html">phpbu</a> <a href="#phpbu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Backup framework f??r PHP.
> Weitere Informationen: <https://phpbu.de>.

#### F??hre ein Backup mit der Standard `phpbu.xml` Konfigurationsdatei aus:
```shell
phpbu
```
#### F??hre ein Backup mit einer bestimmten Konfigurationsdatei aus:
```shell
phpbu --configuration={{pfad/zu/konfiguration.xml}}
```
#### F??hre nur die angegebenen Backups aus:
```shell
phpbu --limit={{backup_art}}
```
#### Simuliere Aktionen die ausgef??hrt werden w??rden:
```shell
phpbu --simulate
```
{% endraw %}{% raw %}
<h2 id="plantuml">
  <a href="/de/common/plantuml.html">plantuml</a> <a href="#plantuml"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle UML-Diagramme aus einer reinen Textsprache und rendere sie in verschiedenen Formaten.
> Weitere Informationen: <https://plantuml.com/en/command-line>.

#### Rendere Diagramme im Standardformat (PNG):
```shell
plantuml {{pfad/zu/diagramm1.puml}} {{pfad/zu/diagramm2.puml}}
```
#### Rendere eine Diagramm im vorgegebenen Format (z.B. `png`, `pdf`, `svg`, `txt`):
```shell
plantuml -t {{format}} {{pfad/zu/diagramm.puml}}
```
#### Rendere alle Diagramme eines Verzeichnisses:
```shell
plantuml {{pfad/zu/verzeichnis}}
```
#### Rendere ein Diagramm in ein bistimmtes Ausgabeverzeichnis:
```shell
plantuml -o {{pfad/zu/verzeichnis}} {{pfad/zu/diagramm.puml}}
```
#### Rendere ein Diagramm mit einer bestimmten Konfigurationsdatei:
```shell
plantuml -config {{pfad/zu/konfig.cfg}} {{pfad/zu/diagramm.puml}}
```
#### Zeige Hilfe an:
```shell
plantuml -help
```
{% endraw %}{% raw %}
<h2 id="rev">
  <a href="/de/common/rev.html">rev</a> <a href="#rev"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kehre die Reihenfolge von Text um.

#### Kehre die Reihenfolge des Textes "Hallo" um:
```shell
echo "Hallo" | rev
```
#### Kehre die Reihenfolge einer Datei um:
```shell
rev {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="ssh-agent">
  <a href="/de/common/ssh-agent.html">ssh-agent</a> <a href="#ssh-agent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle einen SSH Agenten-Prozess.
> Ein SSH Agent beh??lt die hinzugef??gten SSH Schl??ssel solange verschl??sselt im Arbeitsspeicher, bis diese entfernt werden oder der Agenten-Prozess beendet wird.
> Siehe auch `ssh-add`, um Schl??ssel zu verwalten.

#### Starte einen SSH Agenten-Prozesses f??r die aktuelle Shell:
```shell
eval $(ssh-agent)
```
#### Beende den aktuell laufenden SSH Agenten-Prozesses:
```shell
ssh-agent -k
```
{% endraw %}{% raw %}
<h2 id="ssh-copy-id">
  <a href="/de/common/ssh-copy-id.html">ssh-copy-id</a> <a href="#ssh-copy-id"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere den ??ffentlichen Teil eines SSH Schl??ssels in der `authorized_keys` Datei auf einem externen Server.

#### Kopiere den eigenen ??ffentlichen SSH Schl??ssels zu einem externen Server:
```shell
ssh-copy-id {{benutzer}}@{{externer_server}}
```
#### Kopiere den angegebenen ??ffentlichen SSH Schl??ssels zu einem externen Server:
```shell
ssh-copy-id -i {{pfad/zu/??ffentlichem_schl??ssel}} {{benutzer}}@{{externer_server}}
```
#### Kopiere den angegeben ??ffentlichen SSH Schl??ssels zu einem externen Server unter Angabe eines bestimmten SSH Ports:
```shell
ssh-copy-id -i {{pfad/zu/??ffentlichem_schl??ssel}} -p {{port}} {{benutzer}}@{{externer_server}}
```
{% endraw %}{% raw %}
<h2 id="ssh-keygen">
  <a href="/de/common/ssh-keygen.html">ssh-keygen</a> <a href="#ssh-keygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiert ssh Schl??ssel f??r Authentifizierung, Passwort-lose Logins und mehr.

#### Erstelle ein SSH Schl??ssel-Paar interaktiv:
```shell
ssh-keygen
```
#### Erstelle ein Schl??ssel-Paar unter einem bestimmten Dateinamen:
```shell
ssh-keygen -f ~/.ssh/{{datei}}
```
#### Generiere ein ed25519 Schl??ssel-Paar mit 100 Schl??ssel-Ableitungs-Iterationen:
```shell
ssh-keygen -t ed25519 -a 100
```
#### Generiere ein 4096 Bit langen RSA Schl??ssel-Paar mit der Email im Kommentarfeld:
```shell
ssh-keygen -t rsa -b 4096 -C "{{email}}"
```
#### Rufe den Schl??ssel-Fingerabdruck von einem Server ab (hilfreich um die Authentizit??t eines Servers beim ersten Verbinden zu ??berpr??fen):
```shell
ssh-keygen -l -F {{externer_server}}
```
#### Entferne den Schl??ssel eines Servers aus der `known_hosts` Datei (hilfreich wenn ein Server seinen Schl??ssel aktualisiert hat und der alte somit nicht mehr gilt):
```shell
ssh-keygen -R {{externer_server}}
```
#### Rufe den Fingerabdrucks eines Schl??ssels im MD5 Hex Format ab:
```shell
ssh-keygen -l -E md5 -f ~/.ssh/{{datei}}
```
#### ??ndere das Passwort eines privaten Schl??ssels:
```shell
ssh-keygen -p -f ~/.ssh/{{datei}}
```
{% endraw %}{% raw %}
<h2 id="ssh-keyscan">
  <a href="/de/common/ssh-keyscan.html">ssh-keyscan</a> <a href="#ssh-keyscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rufe ??ffentliche SSH Schl??ssel eines externen Servers ab.

#### Rufe alle ??ffentlichen SSH Schl??ssel eines Servers ab:
```shell
ssh-keyscan {{server}}
```
#### Rufe alle ??ffentlichen SSH Schl??ssel unter einem bestimmten Port ab:
```shell
ssh-keyscan -p {{port}} {{server}}
```
#### Rufe bestimmte SSH Sch??ssel-Typen ab:
```shell
ssh-keyscan -t {{rsa,dsa,ecdsa,ed25519}} {{server}}
```
#### Aktualisiere die `known_hosts` SSH Datei mit dem Fingerabdruck eines bestimmten Servers:
```shell
ssh-keyscan -H {{server}} >> ~/.ssh/known_hosts
```
{% endraw %}{% raw %}
<h2 id="ssh">
  <a href="/de/common/ssh.html">ssh</a> <a href="#ssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure Shell ist ein Protokoll f??r das sichere einloggen auf einem externen System.
> Es kann daf??r eingesetzt werden um Befehle auf externen Systemen auszuf??hren.

#### Stelle eine Verbindung zu einem externen Server her:
```shell
ssh {{benutzer}}@{{externer_server}}
```
#### Stelle eine Verbindung zu einem externen Server mit spezifischer Identit??t her (privater SSH Schl??ssel):
```shell
ssh -i {{pfad/zu/schl??ssel_datei}} {{benutzer}}@{{externer_server}}
```
#### Stelle eine Verbindung zu einem externen Server unter einem spezifischen Port her:
```shell
ssh {{benutzer}}@{{externer_server}} -p {{2222}}
```
#### F??hren einen Befehl auf einem externen Server aus:
```shell
ssh {{externer_server}} {{befehl}}
```
#### SSH Tunneln: Leite Ports dynamische Port weiter (SOCKS proxy auf localhost:1080):
```shell
ssh -D {{1080}} {{benutzer}}@{{externer_server}}
```
#### SSH Tunneln: Leite einen spezifischen Ports (localhost:9999 zu example.org:80) weiter zusammen mit deaktivierter pseudy-tty Provisionierung f??r die Ausf??hrung eines Befehls:
```shell
ssh -L {{9999}}:{{example.org}}:{{80}} -N -T {{benutzer}}@{{externer_server}}
```
#### SSH Springen: Verbinde ??ber einen Spring-Server zu einem externen Server (Es k??nnen auch mehrere Spring-Server ??ber eine Komma-separierte Liste angegeben werden):
```shell
ssh -J {{benutzer@sring_server}} {{benutzer}}@{{externer_server}}
```
#### Agenten Weiterleitung: Leite ie eigenen Authentifizierungs-Information an den externen Server weiter (siehe `man ssh_config` f??r mehr Optionen):
```shell
ssh -A {{benutzer}}@{{externer_server}}
```
{% endraw %}{% raw %}
<h2 id="sshfs">
  <a href="/de/common/sshfs.html">sshfs</a> <a href="#sshfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dateisystem Client f??r SSH.
> Weitere Informationen: <https://github.com/libfuse/sshfs>.

#### H??nge ein externes Verzeichnis ein:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} {{lokales_einh??nge_verzeichnis}}
```
#### H??nge ein externes Verzeichnis aus:
```shell
umount {{lokaler_einh??nge_verzeichnis}}
```
#### H??nge ein externes Verzeichnis unter einem bestimmten Port ein:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} -p {{2222}}
```
#### Verwende Komprimierung:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} -C
```
#### Folge symbolischen Links:
```shell
sshfs -o follow_symlinks {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} {{lokaler_einh??nge_verzeichnis}}
```
{% endraw %}{% raw %}
<h2 id="sshpass">
  <a href="/de/common/sshpass.html">sshpass</a> <a href="#sshpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stelle SSH Passw??rtern bereit.

#### Stelle eine Verbindung zu einem externen Server ??ber ein Passwort aus einem Datei-Objekt her (in diesem Fall stdin):
```shell
sshpass -d {{0}} ssh {{benutzer}}@{{server}}
```
#### Stelle eine Verbindung zu einem externen Server mit Hilfe eines Passworts bei automatischer Akzeptierung von unbekannten SSH Schl??sseln her:
```shell
sshpass -p {{passwort}} ssh -o StrictHostKeyChecking=no {{benutzer}}@{{server}}
```
#### Stelle eine Verbindung zu einem externen Server mit Hilfe eines Passworts aus der ersten Zeile einer Datei bei automatischer Akzeptierung von unbekannten SSH Schl??sseln mit anschlie??ender Ausf??hrung eines Befehls her:
```shell
sshpass -f {{pfad/zu/datei}} ssh -o StrictHostKeyChecking=no {{benutzer}}@{{server}} "{{befehl}}"
```
{% endraw %}{% raw %}
<h2 id="tar">
  <a href="/de/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archivierungs Tool.
> H??ufig kombiniert mit anderen Methoden zur Komprimierung, wie gzip oder bzip2.
> Weitere Informationen: <https://www.gnu.org/software/tar>.

#### Erstelle ein Archiv von Datein:
```shell
tar cf {{pfad/zu/ziel.tar}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### Erstelle ein mit gzip komprimiertes Archiv:
```shell
tar czf {{ziel.tar.gz}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### Erstelle ein mit gzip komprimiertes Archiv mit relativen Pfaden:
```shell
tar czf {{pfad/zu/ziel.tar.gz}} -C {{pfad/zu/verzeichniss/}} .
```
#### Extrahiere ein (komprimiertes) Archiv in das derzeitige Verzeichniss:
```shell
tar xf {{pfad/zu/quelle.tar[.gz|.bz2|.xz]}}
```
#### Extrahiere ein Archiv in ein Verzeichniss:
```shell
tar xf {{pfad/zu/quelle.tar}} -C {{verzeichniss}}
```
#### Erstelle ein komprimiertes Archiv und benutze den Archiv Suffix um die Kompressionsmethode zu w??hlen:
```shell
tar caf {{ziel.tar.xz}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### F??hre die Inhalte eines tar Archivs auf:
```shell
tar tvf {{pfad/zu/quelle.tar}}
```
#### Extrahiere Dateien die mit einem Muster ??bereinstimmen:
```shell
tar xf {{pfad/zu/quelle.tar}} --wildcards "{{*.html}}"
```
{% endraw %}{% raw %}
<h2 id="tex">
  <a href="/de/common/tex.html">tex</a> <a href="#tex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine TeX Quelldatei in ein DVI Dokument.
> Weitere Informationen: <https://www.tug.org/begin.html>.

#### Kompiliere ein DVI Dokument:
```shell
tex {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
tex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und stoppe bei jedem Fehler:
```shell
tex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}{% raw %}
<h2 id="texdoc">
  <a href="/de/common/texdoc.html">texdoc</a> <a href="#texdoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Suche nach passenden Dokumentationen f??r (La)TeX Befehle oder Packages.
> Weitere Informationen: <https://texdoc.org/index.html>.

#### ??ffne das erste Suchergebnis im Standard-PDF-Viewer:
```shell
texdoc {{suche}}
```
#### Liste die besten Suchergebnisse auf:
```shell
texdoc --list {{suche}}
```
#### ??ffne die vollst??ndige Dokumentation von `texdoc`:
```shell
texdoc {{texdoc}}
```
{% endraw %}{% raw %}
<h2 id="texliveonfly">
  <a href="/de/common/texliveonfly.html">texliveonfly</a> <a href="#texliveonfly"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade fehlende TeX Live Packages w??hrend dem Kompilieren einer `.tex` Datei herunter.
> Weitere Informationen: <https://ctan.org/pkg/texliveonfly>.

#### Lade fehlende Packages w??hrend dem Kompilieren herunter:
```shell
texliveonfly {{quelldatei.tex}}
```
#### Verwende einen bestimmten Compiler (standardm????ig `pdflatex`):
```shell
texliveonfly --compiler={{compiler}} {{quelldatei.tex}}
```
#### Verwende ein bestimmtes Tex Live `bin` Verzeichnis:
```shell
texliveonfly --texlive_bin={{pfad/zu/texlive_bin}} {{quelldatei.tex}}
```
{% endraw %}{% raw %}
<h2 id="tlmgr">
  <a href="/de/common/tlmgr.html">tlmgr</a> <a href="#tlmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Packages und Konfigurationen einer existierenden TeX Live Installation.
> Weitere Informationen: <https://www.tug.org/texlive/tlmgr.html>.

#### Installiere ein Package und seine Abh??ngigkeiten:
```shell
tlmgr install {{package}}
```
#### Entferne ein Package und seine Abh??ngigkeiten:
```shell
tlmgr remove {{package}}
```
#### Zeige Informationen ??ber ein Pagkage an:
```shell
tlmgr info {{package}}
```
#### Aktualisiere alle Packages:
```shell
tlmgr update --all
```
#### Zeige m??gliche Aktualisierungen an, ohne ??nderungen vorzunehmen:
```shell
tlmgr update --list
```
#### Starte die graphische Oberfl??che von tlmgr:
```shell
tlmgr gui
```
#### Liste alle Tex Live Konfigurationen auf:
```shell
tlmgr conf
```
{% endraw %}{% raw %}
<h2 id="whoami">
  <a href="/de/common/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib den Benutzernamen des aktuellen Benutzers aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/whoami>.

#### Gib den aktiven Benutzernamen aus:
```shell
whoami
```
#### gib den Benutzernamen nach einer ??nderung der Benutzeridentit??t aus:
```shell
sudo whoami
```
{% endraw %}{% raw %}
<h2 id="zsh">
  <a href="/de/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell.
> Mit `bash` und `sh` kompatible Eingabeaufforderung.
> Weitere Informationen: <https://www.zsh.org>.

#### Starte eine interaktive Eingabeaufforderung:
```shell
zsh
```
#### F??hre Parameter als Befehl aus:
```shell
zsh -c {{befehl}}
```
#### F??hre Befehle aus einem Skript aus:
```shell
zsh {{pfad/zu/skript}}
```
#### F??hre Befehle aus einem Skript aus und schreibe die Befehle in die Konsole:
```shell
zsh --xtrace {{pfad/zu/skript}}
```
#### Starte eine interaktive Eingabeaufforderung, in der jeder Befehl ausgegeben wird, bevor er ausgef??hrt wird:
```shell
zsh --verbose
```
{% endraw %}