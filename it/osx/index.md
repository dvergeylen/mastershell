---
layout: default
title: "osx"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#afinfo">afinfo</a>
* <a href="#afplay">afplay</a>
* <a href="#airport">airport</a>
* <a href="#apachectl">apachectl</a>
* <a href="#archey">archey</a>
* <a href="#as">as</a>
* <a href="#asr">asr</a>
* <a href="#base64">base64</a>
* <a href="#brew">brew</a>
* <a href="#brew-bundle">brew bundle</a>
* <a href="#brew-cask">brew cask</a>
* <a href="#caffeinate">caffeinate</a>
* <a href="#diskutil">diskutil</a>

{% raw %}
<h2 id="afinfo">
  <a href="/it/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizzatore dei metadata dei file audio per macOS.
> Comando integrato di macOS.

#### Mostra le informazioni relative ad un file audio specificato:
```shell
afinfo {{percorso/del/file}}
```
#### Mostra una breve descrizione del file audio:
```shell
afinfo -b {{percorso/del/file}}
```
#### Mostra i metadati ed i contenuti dell'InfoDictionary del file audio:
```shell
afinfo -i {{percorso/del/file}}
```
#### Mostra l'output in formato xml:
```shell
afinfo -x {{percorso/del/file}}
```
#### Mostra i problemi del file audio (se ce ne sono):
```shell
afinfo --warnings {{percorso/del/file}}
```
#### Mostra la pagina di aiuto:
```shell
afinfo -h
```
{% endraw %}{% raw %}
<h2 id="afplay">
  <a href="/it/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Riproduttore audio a riga di comando.

#### Riproduci un file audio (fino a quando non finisce la riproduzione):
```shell
afplay {{percorso/del/file}}
```
#### Riproduci un file audio al doppio della velocità:
```shell
afplay --rate 2 {{percorso/del/file}}
```
#### Riproduci un file audio alla metà della velocità:
```shell
afplay --rate 0.5 {{percorso/del/file}}
```
#### Riproduci i primi N secondi di un file audio:
```shell
afplay --time {{N}} {{percorso/del/file}}
```
{% endraw %}{% raw %}
<h2 id="airport">
  <a href="/it/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di configurazione delle reti senza fili.

#### Mostra le informazioni relative allo stato attuale delle connessioni senza fili:
```shell
airport -I
```
#### Intercetta il traffico delle connessioni senza fili sul primo canale:
```shell
airport sniff {{1}}
```
#### Ricerca le reti senza fili disponibili:
```shell
airport -s
```
#### Disassocia dalla rete airport corrente:
```shell
sudo airport -z
```
{% endraw %}{% raw %}
<h2 id="apachectl">
  <a href="/it/osx/apachectl.html">apachectl</a> <a href="#apachectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaccia di controllo del server HTTP Apache per macOS.

#### Avvia il demone `org.apache.httpd`:
```shell
apachectl start
```
#### Ferma il demone:
```shell
apachectl stop
```
#### Riavvia il demone:
```shell
apachectl restart
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/it/osx/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Semplice strumento per mostrare con stile le informazioni di sistema.

#### Mostra le informazioni di sistema:
```shell
archey
```
#### Mostra le informazioni di sistema (senza colorazione del testo):
```shell
archey --nocolor
```
#### Mostra le informazioni di sistema usando MacPorts invece di Homebrew:
```shell
archey --macports
```
#### Mostra le informazioni di sistema senza controllare l'indirizzo IP:
```shell
archey --offline
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/it/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Assembler GNU portabile.
> Progettato principalmente per assemblare l'output di `gcc` ed utilizzarlo con `ld`.

#### Assembla un file, scrivendo l'output su a.out:
```shell
as {{file.s}}
```
#### Assembla l'output nel file dato:
```shell
as {{file.s}} -o {{out.o}}
```
#### Genera l'output più velocemente saltando gli spazi e senza preprocessare i commenti. (Questo comando dovrebbe essere utilizzato solo con compilatori fidati):
```shell
as -f {{file.s}}
```
#### Includi un percorso dato alla lista delle cartelle in cui cercare i file specificati nelle direttive `.include`:
```shell
as -I {{path/to/directory}} {{file.s}}
```
{% endraw %}{% raw %}
<h2 id="asr">
  <a href="/it/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ripristina (copia) un'immagine disco dentro a un volume.
> Il nome del comando sta per Apple Software Restore (software di ripristino Apple).

#### Ripristina un'immagine disco su un volume specifico:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}}
```
#### Distruggi il volume specifico prima di ripristinare:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}} --erase
```
#### Salta la verifica dopo il ripristino:
```shell
sudo asr restore --source {{nome_immagine}}.dmg --target {{percorso/del/volume}} --noverify
```
#### Clona i volumi senza utilizzare un'immagine disco intermedia:
```shell
sudo asr restore --source {{percorso/del/volume}} --target {{percorso/del/volume/clonato}}
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/it/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica e decodifica utilizzando la rappresentazione in base64.

#### Codifica un file:
```shell
base64 -i {{file_da_codificare}}
```
#### Decodifica un file:
```shell
base64 --decode -i {{file_da_decodificare}}
```
#### Codifica da stdin:
```shell
echo -n {{testo_da_codificare}} | base64
```
#### Decodifica da stdin:
```shell
echo -n {{testo_da_decodificare}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="brew-bundle">
  <a href="/it/osx/brew-bundle.html">brew bundle</a> <a href="#brew-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundler per Homebrew, Homebrew Cask e per il Mac App Store.
> Maggiori informazioni: <https://github.com/Homebrew/homebrew-bundle>.

#### Installa un pacchetto da un Brewfile nel percorso corrente:
```shell
brew bundle
```
#### Installa pacchetti da un Brewfile specifico in un percorso specifico:
```shell
brew bundle --file={{percorso/del/file}}
```
#### Crea un Brewfile con tutti i pacchetti installati:
```shell
brew bundle dump
```
#### Disinstalla tutti i pacchetti non specificati nel Brewfile:
```shell
brew bundle cleanup --force
```
#### Controlla se c'è qualcosa da installare o da aggiornare nel Brewfile:
```shell
brew bundle check
```
#### Mostra una lista di tutte le righe presenti nel Brewfile:
```shell
brew bundle list --all
```
{% endraw %}{% raw %}
<h2 id="brew-cask">
  <a href="/it/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti per applicazioni macOS distribuite sotto forma di file binari.
> Maggiori informazioni: <https://github.com/Homebrew/homebrew-cask>.

#### Cerca formule e cask:
```shell
brew search {{testo}}
```
#### Installa un cask:
```shell
brew cask install {{nome_del_cask}}
```
#### Elenca tutti i cask installati:
```shell
brew cask list
```
#### Elenca i cask installati con versioni più nuove disponibili:
```shell
brew cask outdated
```
#### Aggiorna un cask installato (se non viene fornito il nome di nessun cask, tutti i cask saranno aggiornati):
```shell
brew cask upgrade {{nome_del_cask}}
```
#### Disinstalla un cask:
```shell
brew cask uninstall {{nome_del_cask}}
```
#### Disinstalla un cask e rimuovi i relativi file e impostazioni:
```shell
brew cask zap {{nome_del_cask}}
```
#### Mostra informazioni su uno specifico cask:
```shell
brew cask info {{nome_del_cask}}
```
{% endraw %}{% raw %}
<h2 id="brew">
  <a href="/it/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti per macOS.
> Maggiori informazioni: <https://brew.sh>.

#### Cerca formule e cask:
```shell
brew search {{testo}}
```
#### Installa l'ultima versione stabile di una formula (usa `--devel` per le versioni in sviluppo):
```shell
brew install {{formula}}
```
#### Mostra tutte le formule installate:
```shell
brew list
```
#### Mostra le formule installate che non sono dipendenze di un'altra formula installata:
```shell
brew leaves
```
#### Aggiorna una formula installata (se non viene fornito il nome di nessuna formula, tutte le formule installate verranno aggiornate):
```shell
brew upgrade {{formula}}
```
#### Trova la versione più aggiornata di Homebrew e di tutte le formule da GitHub:
```shell
brew update
```
#### Mostra le informazioni su una specifica formula (versione, percorso di installazione, dipendenze, ecc...):
```shell
brew info {{formula}}
```
#### Verifica se la versione installata di Homebrew presenta dei problemi:
```shell
brew doctor
```
{% endraw %}{% raw %}
<h2 id="caffeinate">
  <a href="/it/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Impedisci al mac di sospendersi.

#### Impedisci la sospensione per un'ora (3600 secondi):
```shell
caffeinate -u -t {{3600}}
```
#### Impedisci la sospensione fino al completamento dell'esecuzione di un comando:
```shell
caffeinate -s {{comando}}
```
#### Impedisci la sospensione fino alla pressione della combinazione di tasti Ctrl-C:
```shell
caffeinate -i
```
{% endraw %}{% raw %}
<h2 id="diskutil">
  <a href="/it/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per gestire i dischi locali e i volumi.

#### Mostra tutti i dischi correnti, le partizioni e i volumi montati:
```shell
diskutil list
```
#### Ripara le strutture dati del filesystem di un volume:
```shell
diskutil repairVolume {{/dev/diskX}}
```
#### Smonta un volume:
```shell
diskutil unmountDisk {{/dev/diskX}}
```
#### Estrai un CD/DVD (smontando prima dell'estrazione):
```shell
diskutil eject {{/dev/disk1}}
```
{% endraw %}