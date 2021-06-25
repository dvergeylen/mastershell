---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#alpine">alpine</a>
* <a href="#apt">apt</a>
* <a href="#apt-add-repository">apt-add-repository</a>
* <a href="#apt-get">apt-get</a>
* <a href="#certbot">certbot</a>
* <a href="#cfdisk">cfdisk</a>
* <a href="#dnf">dnf</a>
* <a href="#ip">ip</a>
* <a href="#ip-address">ip address</a>

{% raw %}
<h2 id="alpine">
  <a href="/de/linux/alpine.html">alpine</a> <a href="#alpine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein E-Mail und Usenet Client mit pico/nano-inspirierten Interface.
> Unterstützt die meisten modernen IMAP Server.

#### Öffne Apline:
```shell
alpine
```
#### Öffne alpine im Email-Editor um eine Email an eine bestimmte Adresse zu verfassen:
```shell
alpine {{email@example.net}}
```
#### Beende Alpine:
```shell
'q', dann 'y'
```
{% endraw %}{% raw %}
<h2 id="apt-add-repository">
  <a href="/de/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Editiere die Repository-Listen.
> Weitere Informationen: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Füge ein neues Repository hinzu:
```shell
apt-add-repository {{repository_spec}}
```
#### Entferne ein Repository:
```shell
apt-add-repository --remove {{repository}}
```
#### Aktualisiere den Cache nachdem das Repository hinzugefügt wurde:
```shell
apt-add-repository --update {{repository}}
```
#### Aktiviere Source Pakete:
```shell
apt-add-repository --enable-source {{repository}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/de/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian und Ubuntu Paket Management Tool.
> Suche mit `apt-cache` nach Paketen.
> Weitere Informationen: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Aktualisiere die Liste der Paketquellen (es wird empfohlen diesen Befehl zu Begin auszuführen):
```shell
apt-get update
```
#### Installiere ein Paket oder aktualisiere es zur neuesten Version:
```shell
apt-get install {{paket}}
```
#### Entferne ein Paket:
```shell
apt-get remove {{paket}}
```
#### Entferne ein Paket und die dazugehörigen Konfigurationen:
```shell
apt-get purge {{paket}}
```
#### Aktualisiere alle Pakete auf die neueste Version:
```shell
apt-get upgrade
```
#### Reinige das Repository
```shell
apt-get autoclean
```
#### Entferne alle Pakete, die nicht mehr benötigt werden:
```shell
apt-get autoremove
```
#### Aktualisiere alle Pakete (wie `upgrade`), aber entfernt alle obsoleten Pakete:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/de/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian und Ubuntu Paket Management Tool.
> Empfohlene Alternative zu apt-get seit Ubuntu 16.04.
> Weitere Informationen: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Aktualisiere die Liste der Paketquellen (es wird empfohlen, diesen Befehl zu Beginn auszuführen):
```shell
sudo apt update
```
#### Suche nach einem Paket:
```shell
apt search {{paket}}
```
#### Zeige Informationen über ein Paket:
```shell
apt show {{paket}}
```
#### Installiere ein Paket oder aktualisiere es zur neusten Version:
```shell
sudo apt install {{paket}}
```
#### Entferne ein Paket:
```shell
sudo apt remove {{paket}}
```
#### Aktualisiere alle installierten Pakete auf die neueste Version:
```shell
sudo apt upgrade
```
#### Liste alle Pakete auf:
```shell
apt list
```
#### Liste alle installierten Pakete auf:
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="certbot">
  <a href="/de/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Let's Encrypt Agent zum automatischen Erhalten und Erneuern von TLS-Zertifikaten.
> Nachfolger von `letsencrypt`.
> Weitere Informationen: <https://certbot.eff.org/docs/using.html>.

#### Beziehe ein neues Zertifikat über die webroot-Autorisierung, aber ohne dieses automatisch zu installieren:
```shell
sudo certbot certonly --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}}
```
#### Beziehe ein neues Zertifikat über die nginx-Autorisierung und automatische Installation des neuen Zertifikats:
```shell
sudo certbot --nginx --domain {{subdomain.beispiel.de}}
```
#### Beziehe ein neues Zertifikat über die apache-Autorisierung und automatische Installation des neuen Zertifikats:
```shell
sudo certbot --apache --domain {{subdomain.beispiel.de}}
```
#### Erneuere alle Let's Encrypt Zertifikate die in 30 Tagen oder weniger auslaufen (nicht vergessen alle Server, die diese nutzen, neu zu starten):
```shell
sudo certbot renew
```
#### Simuliere die Zertifikatserneuerung, ohne diese zu speichern:
```shell
sudo certbot --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}} --dry-run
```
#### Beziehe eine Test-Zertifikat:
```shell
sudo certbot --webroot --webroot-path {{pfad/zu/webroot}} --domain {{subdomain.beispiel.de}} --test-cert
```
{% endraw %}{% raw %}
<h2 id="cfdisk">
  <a href="/de/linux/cfdisk.html">cfdisk</a> <a href="#cfdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Programm zur Verwaltung von Partitionstabellen mittels einer Curses-basierten UI.
> Weitere Informationen: <https://manned.org/cfdisk>.

#### Öffne das Partitionierungsinterface für eine bestimmte Festplatte:
```shell
cfdisk {{/dev/sdX}}
```
#### Erzeuge und bearbeite eine neue Partitionierungstabelle für eine bestimmte Festplatte:
```shell
cfdisk --zero {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="dnf">
  <a href="/de/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Paketmanagement Tool für RHEL, Fedora, und CentOS (ersetzt yum).
> Weitere Informationen: <https://dnf.readthedocs.io/>.

#### Aktualisiere alle Pakete auf die neueste Version:
```shell
sudo dnf upgrade
```
#### Suche nach Paketen:
```shell
dnf search {{schlüsselwort}}
```
#### Zeige Daten über ein bestimmtes Paket an:
```shell
dnf info {{paket}}
```
#### Installiere ein neues Paket:
```shell
sudo dnf install {{paket}}
```
#### Installiere ein neues Paket und antworte "ja" auf alle Fragen:
```shell
sudo dnf -y install {{paket}}
```
#### Entferne ein Paket:
```shell
sudo dnf remove {{paket}}
```
#### Liste alle Pakete auf:
```shell
dnf list --installed
```
#### Zeige welches Paket eine Datei besitzt:
```shell
dnf provides {{pfad/zu/datei}}
```
{% endraw %}{% raw %}
<h2 id="ip-address">
  <a href="/de/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Adressen Management Unterbefehl.

#### Zeige Netzwerk-Interfaces mit ihren Adressen:
```shell
ip address
```
#### Zeige nur die aktiven Netzwerk-Interfaces:
```shell
ip address show up
```
#### Zeige Informationen über ein bestimmtes Interface:
```shell
ip address show dev {{eth0}}
```
#### Füge eine Adresse zu einem Interface hinzu:
```shell
ip address add {{ip_adresse}} dev {{eth0}}
```
#### Entferne eine Adresse von einem Interface:
```shell
ip address delete {{ip_adresse}} dev {{eth0}}
```
#### Entfernt alle IP Adressen in einem speziellen Bereich von einem Interface:
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}{% raw %}
<h2 id="ip">
  <a href="/de/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige und manipuliere routing, Geräte, Policy routing und Tunnel.

#### Zeige Interfaces mit detaillierten Informationen:
```shell
ip address
```
#### Zeige Interfaces mit kurzen Netzwerkinformationen:
```shell
ip -brief address
```
#### Zeige Interfaces mit kurzen link layer Informationen:
```shell
ip -brief link
```
#### Zeige die Routing Tabelle:
```shell
ip route
```
#### Zeige Nachbarn (ARP Tabelle):
```shell
ip neighbour
```
#### Schaltee ein bestimmten Interface ein oder aus:
```shell
ip link set {{interface}} {{up|down}}
```
#### Entferne oder füge eine IP zu einem Interface hinzu:
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Füge eine Standard Route hinzu:
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}