---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#acpi">acpi</a>
* <a href="#add-apt-repository">add-apt-repository</a>
* <a href="#adduser">adduser</a>
* <a href="#apt">apt</a>
* <a href="#apt-add-repository">apt-add-repository</a>
* <a href="#apt-cache">apt-cache</a>
* <a href="#apt-file">apt-file</a>
* <a href="#apt-get">apt-get</a>
* <a href="#apt-key">apt-key</a>
* <a href="#apt-mark">apt-mark</a>
* <a href="#binwalk">binwalk</a>
* <a href="#cp">cp</a>
* <a href="#deluser">deluser</a>
* <a href="#dpkg">dpkg</a>
* <a href="#dpkg-deb">dpkg-deb</a>
* <a href="#dpkg-query">dpkg-query</a>
* <a href="#fsck">fsck</a>
* <a href="#halt">halt</a>
* <a href="#lsmod">lsmod</a>
* <a href="#lsusb">lsusb</a>
* <a href="#mkfs">mkfs</a>
* <a href="#modinfo">modinfo</a>
* <a href="#modprobe">modprobe</a>
* <a href="#pidof">pidof</a>
* <a href="#poweroff">poweroff</a>
* <a href="#tree">tree</a>

{% raw %}
<h2 id="acpi">
  <a href="/it/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra lo stato e le informazioni termiche della batteria.
> Maggiori informazioni: <https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### Mostra le informazioni sulla batteria:
```shell
acpi
```
#### Mostra le informazioni termiche:
```shell
acpi -t
```
#### Mostra le informazioni sul dispositivo di raffreddamento:
```shell
acpi -c
```
#### Mostra le informazioni termiche in gradi Fahrenheit:
```shell
acpi -tf
```
#### Mostra tutte le informazioni:
```shell
acpi -V
```
#### Estrae le informazioni da `/proc` invece che da `/sys`:
```shell
acpi -p
```
{% endraw %}{% raw %}
<h2 id="add-apt-repository">
  <a href="/it/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisce le definizioni di repository apt.

#### Aggiunge un nuovo repository apt:
```shell
add-apt-repository {{identificativo_del_repository}}
```
#### Rimuove un repository apt:
```shell
add-apt-repository --remove {{identificativo_del_repository}}
```
#### Aggiorna la cache dei pacchetti dopo aver aggiunto un repository:
```shell
add-apt-repository --update {{identificativo_del_repository}}
```
#### Attiva i pacchetti sorgente:
```shell
add-apt-repository --enable-source {{identificativo_del_repository}}
```
{% endraw %}{% raw %}
<h2 id="adduser">
  <a href="/it/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio per aggiungere utenti.
> Maggiori informazioni: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Crea un nuovo utente con una home directory predefinita e richiede all'utente di impostare una password:
```shell
adduser {{nome_utente}}
```
#### Crea un utente senza una home directory:
```shell
adduser --no-create-home {{nome_utente}}
```
#### Crea un utente con una home directory nel percorso specificato:
```shell
adduser --home {{percorso/all/home}} {{nome_utente}}
```
#### Crea un nuovo utente con l'interprete di comandi(shell) specificato come shell di accesso:
```shell
adduser --shell {{percorso/alla/shell}} {{nome_utente}}
```
#### Crea un nuovo utente appartenente al gruppo specificato:
```shell
adduser --ingroup {{gruppo}} {{nome_utente}}
```
#### Aggiunge un utente esistente al gruppo specificato:
```shell
adduser {{nome_utente}} {{gruppo}}
```
{% endraw %}{% raw %}
<h2 id="apt-add-repository">
  <a href="/it/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisce le definizioni di repository apt.
> Maggiori informazioni: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Aggiunge un nuovo repository apt:
```shell
apt-add-repository {{identificativo_del_repository}}
```
#### Rimuove un repository apt:
```shell
apt-add-repository --remove {{identificativo_del_repository}}
```
#### Aggiorna la cache dei pacchetti dopo aver aggiunto un repository:
```shell
apt-add-repository --update {{identificativo_del_repository}}
```
#### Attiva i pacchetti sorgente:
```shell
apt-add-repository --enable-source {{identificativo_del_repository}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/it/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumenti di Debian e Ubuntu per richiedere informazioni sui pacchetti.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Cerca un pacchetto nelle sorgenti attuali:
```shell
apt-cache search {{query}}
```
#### Mostra informazioni su un pacchetto:
```shell
apt-cache show {{pacchetto}}
```
#### Mostra se un pacchetto è installato ed aggiornato:
```shell
apt-cache policy {{pacchetto}}
```
#### Mostra le dipendenze di un pacchetto:
```shell
apt-cache depends {{pacchetto}}
```
#### Mostra i pacchetti che dipendono da un particolare pacchetto:
```shell
apt-cache rdepends {{pacchetto}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/it/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cerca un file dentro un pacchetto apt, includendo quelli non ancora installati.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Aggiorna il database dei metadati:
```shell
sudo apt update
```
#### Cerca i pacchetti che contengono un file o un percorso specificato:
```shell
apt-file search {{parte/del/filename}}
```
#### Elenca i contenuti di un pacchetto specifico:
```shell
apt-file list {{nome_del_pacchetto}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/it/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione dei pacchetti per Debian e Ubuntu.
> Cerca i pacchetti usando `apt-cache`.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Aggiorna la lista dei pacchetti e delle loro versioni disponibili (è consigliato eseguire questo comando prima di altri comandi `apt-get`):
```shell
apt-get update
```
#### Installa un pacchetto, o lo aggiorna all'ultima versione disponibile:
```shell
apt-get install {{pacchetto}}
```
#### Rimuove un pacchetto:
```shell
apt-get remove {{pacchetto}}
```
#### Rimuove un pacchetto ed i suoi file di configurazione:
```shell
apt-get purge {{pacchetto}}
```
#### Aggiorna tutti i pacchetti installati alla versione disponibile più recente:
```shell
apt-get upgrade
```
#### Pulisce gli archivi locali - rimuovendo i file (.deb) da scaricamenti interrotti che non possono più essere scaricati:
```shell
apt-get autoclean
```
#### Rimuove tutti i pacchetti che non sono più necessari:
```shell
apt-get autoremove
```
#### Aggiorna tutti i pacchetti installati (come `upgrade`), rimuovendo i pacchetti obsoleti ed installando ulteriori pacchetti per soddisfare le nuove dipendenze:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-key">
  <a href="/it/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione delle chiavi per il gestore di pacchetti APT su Debian ed Ubuntu.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Elenca le chiavi fidate:
```shell
apt-key list
```
#### Aggiunge una chiave al portachiavi delle chiavi fidate:
```shell
apt-key add {{file_chiave_pubblica.asc}}
```
#### Elimina una chiave dal portachiavi delle chiavi fidate:
```shell
apt-key del {{id_chiave}}
```
#### Aggiunge una chiave remota al portachiavi delle chiavi fidate:
```shell
wget -qO - {{https://indirizzo.tld/filename.key}} | apt-key add -
```
#### Aggiunge una chiave da un server di chiavi con il solo id della chiave:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{ID_DELLA_CHIAVE}}
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/it/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio per cambiare lo stato di un pacchetto installato.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Contrassegna un pacchetto come installato automaticamente:
```shell
sudo apt-mark auto {{nome_del_pacchetto}}
```
#### Mantiene un pacchetto alla sua versione attuale e ne previene l'aggiornamento:
```shell
sudo apt-mark hold {{nome_del_pacchetto}}
```
#### Consente ad un pacchetto di essere nuovamente aggiornato:
```shell
sudo apt-mark unhold {{nome_del_pacchetto}}
```
#### Mostra i pacchetti installati manualmente:
```shell
apt-mark showmanual
```
#### Visualizza i pacchetti mantenuti alla versione attuale che non sono stati aggiornati:
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/it/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione dei pacchetti per distribuzioni basate su Debian.
> Rimpiazzo raccomandato di apt-get quando usato interattivamente su Ubuntu 16.04 e versioni successive.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Aggiorna la lista dei pacchetti e delle loro versioni disponibili (è consigliato eseguire questo comando prima di altri comandi `apt`):
```shell
sudo apt update
```
#### Cerca per un dato pacchetto:
```shell
apt search {{pacchetto}}
```
#### Mostra le informazioni su un pacchetto:
```shell
apt show {{pacchetto}}
```
#### Installa un pacchetto, o lo aggiorna all'ultima versione disponibile:
```shell
sudo apt install {{pacchetto}}
```
#### Rimuove un pacchetto (usando `purge` rimuove anche i suoi file di configurazione):
```shell
sudo apt remove {{pacchetto}}
```
#### Aggiorna tutti i pacchetti installati alla versione disponibile più recente:
```shell
sudo apt upgrade
```
#### Elenca tutti i pacchetti:
```shell
apt list
```
#### Elenca i pacchetti installati:
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="binwalk">
  <a href="/it/linux/binwalk.html">binwalk</a> <a href="#binwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per l'analisi di file binari.
> Maggiori informazioni: <https://github.com/ReFirmLabs/binwalk>.

#### Scansiona un file binario:
```shell
binwalk {{percorso/a/file}}
```
#### Estrae file da un binario, specificando la cartella di output:
```shell
binwalk --extract --directory {{cartella_di_output}} {{percorso/a/file}}
```
#### Estrae file in maniera ricorsiva a partire da un binario, limitando la profondità di ricorsione a 2 livelli:
```shell
binwalk --extract --matryoshka --depth {{2}} {{percorso/a/file}}
```
#### Estrae file da un binario utilizzando una particolare firma (ad esempio il MIME Type):
```shell
binwalk --dd '{{png image:png}}' {{percorso/a/file}}
```
#### Analizza l'entropia di un binario e salva il grafico con lo stesso filename del binario, con l'estensione `.png` in fondo:
```shell
binwalk --entropy --save {{percorso/a/file}}
```
#### Combina analisi di entropia, firme e opcode in un unico comando:
```shell
binwalk --entropy --signature --opcodes {{percorso/a/file}}
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/it/linux/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia file e cartelle.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cp>.

#### Copia un file in un'altra posizione:
```shell
cp {{persorso/al/file_da_copiare.est}} {{percorso/al/file_di_destinazione.est}}
```
#### Copia un file all'interno di una cartella, mantenendone uguale il nome:
```shell
cp {{percorso/al/file_da_copiare.est}} {{percorso/alla/cartella}}
```
#### Copia ricorsivamente i contenuti di una cartella in un'altra posizione (se la destinazione esiste, la cartella è copiata al suo interno):
```shell
cp -r {{percorso/alla/cartella_da_copiare}} {{percorso/di/destinazione}}
```
#### Copia una cartella ricorsivamente in modalità prolissa (mostra i file mentre vengono copiati):
```shell
cp -vr {{percorso/alla/cartella_da_copiare}} {{percorso/di/destinazione}}
```
#### Copia i file di testo in un'altra posizione, in modalità interattiva (richiede conferma all'utente prima di sovrascrivere):
```shell
cp -i {{*.txt}} {{percorso/di/destinazione}}
```
#### Segue i collegamenti simbolici prima di copiare:
```shell
cp -L {{collegamento}} {{percorso/di/destinazione}}
```
#### Utilizza il percorso completo dei file originali, creando ogni cartella intermedia mancante mentre durante la copia:
```shell
cp --parents {{percorso/dei/file/da/copiare}} {{percorso/al/file/destinazione}}
```
{% endraw %}{% raw %}
<h2 id="deluser">
  <a href="/it/linux/deluser.html">deluser</a> <a href="#deluser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rimuovi un account utente o un utente da un gruppo.
> Maggiori informazioni: <https://manpages.debian.org/latest/adduser/deluser.html>.

#### Rimuovi un utente:
```shell
deluser {{nome}}
```
#### Rimuovi un utente insieme alla sua directory home e raccolta mail:
```shell
deluser -r {{nome}}
```
#### Rimuovi un utente da un gruppo:
```shell
deluser {{nome}} {{gruppo}}
```
{% endraw %}{% raw %}
<h2 id="dpkg-deb">
  <a href="/it/linux/dpkg-deb.html">dpkg-deb</a> <a href="#dpkg-deb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Impacchetta, spacchetta e fornisce informazioni su archivi Debian.
> Maggiori informazioni: <https://manpages.debian.org/buster/dpkg/dpkg-deb.1.en.html>.

#### Mostra le informazioni riguardo ad un pacchetto:
```shell
dpkg-deb --info {{percorso/al/file.deb}}
```
#### Mostra il nome e la versione del pacchetto in una singola riga:
```shell
dpkg-deb --show {{percorso/al/file.deb}}
```
#### Elenca i contenuti del pacchetto:
```shell
dpkg-deb --contents {{percorso/al/file.deb}}
```
#### Estrae i contenuti del pacchetto in una cartella:
```shell
dpkg-deb --extract {{percorso/al/file.deb}} {{percorso/alla/cartella}}
```
#### Crea una pacchetto a partire da una cartella specificata:
```shell
dpkg-deb --build {{percorso/alla/cartella}}
```
{% endraw %}{% raw %}
<h2 id="dpkg-query">
  <a href="/it/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno strumento che mostra informazioni sui pacchetti installati.

#### Elenca tutti i pacchetti installati:
```shell
dpkg-query -l
```
#### Elenca i pacchetti installati con nomi che combaciano con una data espressione:
```shell
dpkg-query -l '{{espressione_pattern}}'
```
#### Elenca tutti i file installati da una pacchetto:
```shell
dpkg-query -L {{nome_del_pacchetto}}
```
#### Mostra le informazioni riguardanti un pacchetto:
```shell
dpkg-query -s {{nome_del_pacchetto}}
```
{% endraw %}{% raw %}
<h2 id="dpkg">
  <a href="/it/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti Debian.
> Maggiori informazioni: <https://manpages.debian.org/buster/dpkg/dpkg.1.en.html>.

#### Installa un pacchetto:
```shell
dpkg -i {{percorso/al/file.deb}}
```
#### Rimuove un pacchetto:
```shell
dpkg -r {{nome_del_pacchetto}}
```
#### Elenca i pacchetti installati:
```shell
dpkg -l {{espressione_per_la_ricerca}}
```
#### Elenca i contenuti di un pacchetto:
```shell
dpkg -L {{nome_del_pacchetto}}
```
#### Elenca i contenuti di un file pacchetto locale:
```shell
dpkg -c {{percorso/al/file.deb}}
```
#### Trova a quale pacchetto appartiene un file:
```shell
dpkg -S {{filename}}
```
{% endraw %}{% raw %}
<h2 id="fsck">
  <a href="/it/linux/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Controlla l'integrità di un filesystem o lo ripara. Il filesystem non dev'essere montato al momento in cui il comando viene eseguito.

#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati:
```shell
fsck {{/dev/sdX}}
```
#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati e per ognuno consente all'utente di scegliere interattivamente se ripararlo:
```shell
fsck -r {{/dev/sdX}}
```
#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati e riparandoli automaticamente:
```shell
fsck -a {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="halt">
  <a href="/it/linux/halt.html">halt</a> <a href="#halt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arresta, spegne o riavvia la macchina.
> Maggiori informazioni: <https://www.freedesktop.org/software/systemd/man/halt.html>.

#### Arresta la macchina:
```shell
halt
```
#### Spegne la macchina:
```shell
halt --poweroff
```
#### Riavvia la macchina:
```shell
halt --reboot
```
{% endraw %}{% raw %}
<h2 id="lsmod">
  <a href="/it/linux/lsmod.html">lsmod</a> <a href="#lsmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra lo stato dei moduli del kernel Linux.
> Vedi anche `modprobe`, che carica i moduli del kernel.

#### Elenca tutti i moduli del kernel attualmente caricati:
```shell
lsmod
```
{% endraw %}{% raw %}
<h2 id="lsusb">
  <a href="/it/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualizza le informazioni su i bus USB e i dispositivi a loro connessi.

#### Elenca tutti i dispositivi USB disponibili:
```shell
lsusb
```
#### Visualizza la gerarchia USB come un albero:
```shell
lsusb -t
```
#### Elenca informazioni prolisse riguardo ai dispositivi USB:
```shell
lsusb --verbose
```
#### Elenca informazioni dettagliate riguardo ad un dispositivo USB:
```shell
lsusb -D {{dispositivo}}
```
#### Elenca solamente i dispositivi con un certo id fornitore e id prodotto:
```shell
lsusb -d {{fornitore}}:{{prodotto}}
```
{% endraw %}{% raw %}
<h2 id="mkfs">
  <a href="/it/linux/mkfs.html">mkfs</a> <a href="#mkfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Costruisce un filesystem Linux su una partizione del disco rigido.
> Questo comando è deprecato in favore degli strumenti specifici per filesystem: mkfs.<tipo>.

#### Costruisce un filesystem Linux ext2 su una partizione:
```shell
mkfs {{percorso/alla/partizione}}
```
#### Costruisce un filesystem del tipo specificato:
```shell
mkfs -t {{ext4}} {{percorso/alla/partizione}}
```
#### Costruisce un filesystem del specificato e controlla la presenza di settori danneggiati:
```shell
mkfs -c -t {{ntfs}} {{percorso/alla/partizione}}
```
{% endraw %}{% raw %}
<h2 id="modinfo">
  <a href="/it/linux/modinfo.html">modinfo</a> <a href="#modinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Estrae le informazioni riguardarti un modulo del kernel Linux.

#### Elenca tutti gli attributi di un modulo del kernel:
```shell
modinfo {{modulo_del_kernel}}
```
#### Elenca solamente gli attributi specificati:
```shell
modinfo -F {{author|description|license|parm|filename}} {{modulo_del_kernel}}
```
{% endraw %}{% raw %}
<h2 id="modprobe">
  <a href="/it/linux/modprobe.html">modprobe</a> <a href="#modprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aggiunge o rimuove moduli del kernel Linux.

#### Fa finta di carica un modulo nel kernel, ma non lo fa veramente:
```shell
sudo modprobe --dry-run {{nome_del_modulo}}
```
#### Carica un modulo nel kernel:
```shell
sudo modprobe {{nome_del_modulo}}
```
#### Rimuove un modulo dal kernel:
```shell
sudo modprobe --remove {{nome_del_modulo}}
```
#### Rimuove dal kernel un modulo e quelli che dipendono da quest'ultimo:
```shell
sudo modprobe --remove-dependencies {{nome_del_modulo}}
```
#### Mostra le dipendenza di un modulo del kernel:
```shell
sudo modprobe --show-depends {{nome_del_modulo}}
```
{% endraw %}{% raw %}
<h2 id="pidof">
  <a href="/it/linux/pidof.html">pidof</a> <a href="#pidof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ottiene l'ID di un processo a partire dal suo nome.

#### Elenca gli ID di tutti i processi con un dato nome:
```shell
pidof {{bash}}
```
#### Elenca un solo ID di processo con il nome specificato:
```shell
pidof -s {{bash}}
```
#### Elenca gli ID dei processi con un dato includendo anche gli script:
```shell
pidof -x {{script.py}}
```
#### Uccide tutti i processi con un dato nome:
```shell
kill "$(pidof {{nome}})" 
```
{% endraw %}{% raw %}
<h2 id="poweroff">
  <a href="/it/linux/poweroff.html">poweroff</a> <a href="#poweroff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chiude il sistema.

#### Spegne il sistema:
```shell
sudo poweroff
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/it/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra i contenuti della cartella corrente come un albero.
> Maggiori informazioni: <http://mama.indstate.edu/users/ice/tree/>.

#### Stampa file e cartella fino al 'num'-esimo livello di profondità (dove 1 significa la cartella corrente):
```shell
tree -L {{num}}
```
#### Stampa solamente le cartelle:
```shell
tree -d
```
#### Stampa anche i file nascosti con la colorazione attiva:
```shell
tree -a -C
```
#### Stampa l'albero senza linee di indentazione, mostrando invece il percorso completo (usa `-N` per non convertire caratteri non stampabili in sequenze di escape):
```shell
tree -i -f
```
#### Stampa la dimensione di ogni file e la dimensione totale di ogni cartella, in formato leggibile dall'utente:
```shell
tree -s -h --du
```
#### Stampa i file all'interno dell'albero gerarchico, utilizzando espressioni di metacaratteri (glob pattern) per escludere le cartelle che non contengono file corrispondenti alla ricerca:
```shell
tree -P '{{*.txt}}' --prune
```
#### Stampa le cartelle all'interno dell'albero gerarchico, utilizzando espressioni di metacaratteri (glob pattern) per escludere le cartelle che non sono progenitori di quelle desiderate:
```shell
tree -P {{nomi_di_cartelle}} --matchdirs --prune
```
#### Stampa l'albero ignorando le cartelle date:
```shell
tree -I '{{nome_cartella1|nome_cartella2}}'
```
{% endraw %}